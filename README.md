# lit-builder

Pull ML conference paper lists, filter for the [Sutro Group](https://github.com/cybertronai/SutroYaro) lens (energy-efficient training + broader training-efficiency), and produce an annotated, browsable literature base.

Source: [papercopilot/paperlists](https://github.com/papercopilot/paperlists). Starts with ICLR 2026 (~20K records); generalizes to NeurIPS, ICML, etc.

## Pipeline

```
fetch  →  ingest  →  filter (keywords)  →  score (LLM)  →  deepen (on demand)  →  render
```

Each stage is a CLI subcommand and writes to a SQLite database (`data/db/lit.sqlite`). The markdown / MkDocs site is generated from the DB.

## LLM provider — pick one

The scoring stage uses an LLM. Two providers are supported, controlled by `LIT_PROVIDER`:

```bash
# Anthropic (default)
export LIT_PROVIDER=anthropic
export ANTHROPIC_API_KEY=sk-ant-...
# default model: claude-haiku-4-5-20251001 (override with LIT_MODEL)

# Ollama Cloud (gpt-oss, deepseek, etc.)
export LIT_PROVIDER=ollama
export OLLAMA_API_KEY=...
# default model: gpt-oss:120b
# override:  export LIT_MODEL=deepseek-v4-pro:cloud

# Ollama local (no key needed)
export LIT_PROVIDER=ollama
export OLLAMA_HOST=http://localhost:11434
export LIT_MODEL=llama3.1:8b
```

## Quickstart

```bash
pip install -e .
# or with uv: uv sync && uv run lit ...

lit fetch  iclr2026
lit ingest iclr2026
lit filter iclr2026                       # keyword pre-filter
lit score  iclr2026 --limit 200           # LLM triage on survivors (0–3 + reason)
lit list   iclr2026 --min-score 2         # browse high-relevance
lit deepen iclr2026 <paper_id>            # structured digest on demand
lit render iclr2026                       # write markdown + mkdocs nav
lit serve                                 # local mkdocs preview
```

## Real example output

Scoring 5 ICLR 2026 candidates on `gpt-oss:120b` (Ollama Cloud), ~5s per paper:

| score | title | reason |
|---|---|---|
| 2 | PersonalQ: Select, Quantize, and Serve Personalized Diffusion | Quantization technique for personalized diffusion models that reduces inference memory, aligning with low-precision research. |
| 2 | Reassessing Layer Pruning in LLMs | Layer pruning to reduce computation, directly addressing efficiency and model compression. |
| 1 | Toward Unifying Group Fairness Evaluation from a Sparsity Perspective | References sparsity but only as a lens for fairness evaluation, not as a contribution to training efficiency. |
| 1 | Early Layer Readouts for Robust Knowledge Distillation | Domain generalization via adaptive distillation, only tangential efficiency link. |
| 0 | Concept Alignment for Autonomous Distillation | Robustness and bias mitigation, not energy-efficient training. |

## CLI as a tool

The CLI is designed to be called by other coding agents (Codex, Claude Code). Every command takes positional args, exits non-zero on error, and prints structured key=value output. See `lit --help`.

## Layout

```
src/lit_builder/
  models.py        # shared dataclasses + SQLite DDL
  config.py        # paths, venue registry
  data/            # papercopilot fetch + SQLite ingest
  filter/          # keyword matcher
  score/           # LLM scorer + deepener (Anthropic / Ollama)
  render/          # markdown + mkdocs export
  cli/             # typer commands
configs/keywords.yaml   # editable keyword groups
```

## Status

| Stage | iclr2026 |
|---|---|
| fetch | done — 19,814 raw records (93 MB) |
| ingest | done — 19,814 in DB; 5,358 accepted (Poster + Oral + Conditional*) |
| filter | done — 4,842 keyword candidates |
| score | partial (5 / 4,842 scored) — provider-agnostic, runs against either Anthropic or Ollama |
| deepen | implemented; on-demand per paper |
| render | implemented; not yet written for iclr2026 |

## Tests

```bash
pip install pytest
PYTHONPATH=src python3 -m pytest tests -q       # 33 tests, all mocked LLM
```
