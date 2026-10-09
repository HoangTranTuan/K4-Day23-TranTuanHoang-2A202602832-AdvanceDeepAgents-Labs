# Survey on Efficient Inference and Small Language Models

## TL;DR
- Small language models support local deployment by trading model capacity against memory, latency, and task accuracy [13][12].
- Compact architectures, model compression, and adaptive edge-cloud routing address different deployment constraints [11][10].
- Efficient training and subnetwork selection complement inference optimization but require separate evaluation [9][8].
- Hardware-aware methods and consistent benchmarks remain priorities for practical deployment [13][4].

## Background
One survey studies decoder-only models with 100M-5B parameters and evaluates both capability and device runtime costs. Its definition is narrower than rankings that include models under 100B parameters, so results must be compared within a stated size range [13][5]. Broader SLM surveys describe architecture, training, and compression choices [12].

## Compact Models and Compression
H2O-Danube3 illustrates compact model design for constrained deployment [11]. Structural pruning also appears in atomistic foundation models; this is related compression research rather than direct evidence of language-model inference gains [7]. Architecture and compression choices should be assessed against the language-model accuracy and runtime measurements described in SLM surveys [13][12].

## Collaborative and Adaptive Inference
SWARM-LLM routes work between local small models and cloud resources using uncertainty and safety signals. Compared with fully local execution, selective cloud access trades network and service costs for stronger answers on difficult queries [10].

## Training Efficiency and Subnetworks
RAPID targets efficient reinforcement learning for small models, while ProbeScale studies parameter-efficient subnetworks. They address training and model-selection costs alongside inference, so improvements in one stage should not be treated as equivalent gains in another [9][8].

## Benchmarks and Deployment Evaluation
The distil labs study compares 12 small models across 8 tasks and reports strong fine-tuned Qwen3 results. BenchLM provides another model ranking, but its under-100B category differs from the narrower SLM definition above [6][5][13]. The original research also lists MLCommons Inference and SLMbench, but reports failed retrieval; no benchmark result is attributed to those pages here [2][1].

## Trends and Open Problems
Fault-tolerant foundation models and faster diffusion sampling illustrate broader efficiency directions; neither alone establishes an SLM-specific improvement [4][3]. Open questions include comparable accuracy-latency measurements, combining compression methods, and evaluating local versus cloud-assisted execution under realistic deployment constraints [13][12][10].

## References
[1] SLMbench.ai. web. https://www.slmbench.ai (n.d.)
[2] MLCommons Inference v5.1. web. https://mlcommons.org/en/inference-v51 (n.d.)
[3] Hybrid-Basis Feature Forecasting for Diffusion Sampling Acceleration. arxiv. https://arxiv.org/abs/2610.05254 (2026-10-04)
[4] Fault-tolerant foundation models. arxiv. https://arxiv.org/abs/2610.10311 (2026-10-07)
[5] Small language models under 100B. web. https://benchlm.ai/best/small-language-models (2026-10-08)
[6] We Benchmarked 12 Small Language Models Across 8 Tasks to Find the Best Base Model for Fine-Tuning. web. https://www.distillabs.ai/blog/we-benchmarked-12-small-language-models-across-8-tasks-to-find-the-best-base-model-for-fine-tuning/ (2025-12-10)
[7] Compact SO(3) Equivariant Atomistic Foundation Models via Structural Pruning. arxiv. https://arxiv.org/abs/2605.08885 (2026-05-09)
[8] ProbeScale: Probing Analysis to Optimize Neural Scaling Laws for Efficient Small Language Model Inference. hf-search. https://huggingface.co/papers/2606.01806 (2026-06-01)
[9] RAPID: An Efficient Reinforcement Learning Algorithm for Small Language Models. hf-search. https://huggingface.co/papers/2510.03515 (2025-10-03)
[10] SWARM-LLM: Collaborative Inference for Edge-based Small Language Models. hf-search. https://huggingface.co/papers/2606.14711 (2026-04-22)
[11] H2O-Danube3 Technical Report. hf-search. https://huggingface.co/papers/2407.09276 (2024-07-12)
[12] A Survey on Small Language Models. web. https://aclanthology.org/anthology-files/pdf/ranlp/2025.ranlp-1.93.pdf (n.d.)
[13] Small Language Models: Survey, Measurements, and Insights. arxiv. https://arxiv.org/abs/2409.15790 (2025-02-26)
