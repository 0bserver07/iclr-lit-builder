# ENERGYLLM-BENCH:AREPRODUCIBLEBENCHMARKFORENERGYAND CARBONFOOTPRINTOFLARGELANGUAGEMODELS

**Venue:** iclr2026 (Desk Reject)
**Authors:** youla yang
**OpenReview:** [https://openreview.net/forum?id=0FbhKezdBK](https://openreview.net/forum?id=0FbhKezdBK)

## Relevance

**LLM score:** 3/3 — The paper introduces a reproducible benchmark for energy-efficient LLM evaluation, including low-precision, hardware comparison, and FLOPs-based efficiency prediction, directly supporting the group's focus on energy-efficient AI and hardware-aware analysis.
**Keyword hits:** `flops`

## TLDR
(none provided)

## Abstract
Therapidgrowthoflargelanguagemodels(LLMs)hasraisedurgentconcernsabouttheirenergyfootprintduring
 trainingandinference.Existingtools,suchasMLPerfandCodeCarbon,provideonlycoarseestimatesandlack
 reproducibleprotocolsforsystem-levelevaluationofLLMefficiency.
 WeintroduceEnergyLLM-Bench,anopen-sourceframeworkthatunifiesin-looppowermeasurement,FLOPs
basedprediction,andstandardizedJSONLloggingintoasinglereproduciblebenchmark.Allmeasurementsare
 releasedthroughanextensiblepublicleaderboard,enablingtransparentcomparisonacrossmodels,hardware,and
 softwareconfigurations.
 Our evaluation spans dense andmixture-of-experts architectures, CPUs andGPUs, andmultiple opti
mizer/precisionsettings.Resultsrevealseveralkeyinsights: (i)scalingGPTmodelsraisesper-tokenenergyby
 morethan3×;(ii)GPUsconsistentlydeliver4–6×higherinferenceefficiencythanCPUs;(iii)BF16precision
 reducesenergyconsumptionby10–15%relativetoFP32;and(iv)despitelowerFLOPs,mixture-of-experts
 modelscanincurorders-of-magnitudehigherrealizedcostsduetoroutingoverhead.FLOPs-basedpredictors,
 especiallygradientboosting,capturetheseefficiencytrendswithtightererrorboundsthanlinearbaselines.
 Byconsolidatingprotocol,predictors,andanopenleaderboard,EnergyLLM-Benchestablishesthefirstrepro
duciblefoundationforanalyzingtheenergy–qualityfrontierofLLMs.Wehopeitservesasaprincipledtoolfor
 MLandsystemsresearchersworkingtowardsustainablemodeldesignanddeployment

## Keywords
LLM, energy footprint
