# Survey on World Models

## TL;DR
- World models predict environmental dynamics to support planning, control, and interaction [11][10].
- Latent models prioritize compact dynamics; video simulators prioritize detailed predictions, with different trade-offs for planning [8][7][6].
- Recent work explores real-time control, physical interaction, and closed-loop task execution [9][5][3].
- Long-horizon consistency, causal reasoning, and transfer to real environments remain open problems [4][2].

## Background
World models represent how environments evolve so agents can anticipate outcomes and choose actions. Surveys connect modern neural world models with earlier ideas about internal simulation and distinguish prediction from broader world understanding [11][10].

## Latent Dynamics and Representations
PlaNet and Dreamer use compact latent dynamics for model-based reinforcement learning. Latent states reduce the cost of prediction, while video, 3D, and symbolic representations offer different balances of detail, interpretability, and planning utility [8][7][2].

## Neural Simulation and Physical Consistency
Transformer and diffusion approaches generate detailed future observations. Visual quality alone does not establish reliable simulation: physical consistency and stable long-term predictions remain central evaluation concerns [6]. DreamForge-World explores low-compute, real-time control, while InternW0 targets physical-world interaction [9][3].

## Planning and Closed-Loop Execution
SAGE investigates subgoal-conditioned action generation for latent planning. WorldGuide instead emphasizes goal-directed video modeling and feedback during procedural execution. Both connect predictive models with action, but at different levels of representation and control [1][5].

## Trends and Open Problems
Current surveys emphasize causal understanding, action conditioning, long-horizon reasoning, and sim-to-real transfer. Progress requires assessing whether predictions support useful decisions as well as visually plausible outcomes [10][4][2]. Integrating model families and interactive environments is a promising direction, but generalization across tasks remains unresolved [11][4].

## References
[1] SAGE: Subgoal-Conditioned Action Generation for Latent World Model Planning. hf-search. https://huggingface.co/papers/2607.17973 (2026-07-20)
[2] State of World Models 2026: Taxonomy, Benchmarks and Open Challenges. web. https://world-models.io/reports/state-of-world-models-2026/state-of-world-models-2026-v1.0.pdf (n.d.)
[3] InternW0: A Foundational Physical World Model for Efficient Real-World Interactions. hf-search. https://huggingface.co/papers/2609.27656 (2026-09-23)
[4] State of World Models 2026 | Landscape Report. web. https://world-models.io/reports/state-of-world-models-2026/ (n.d.)
[5] WorldGuide: Goal-Directed Video World Model for Procedural Task Execution. hf-daily. https://huggingface.co/papers/2610.12459 (2026-10-08)
[6] From Generation to Simulation: How Far Are World Models from Being True Simulators?. hf-search. https://huggingface.co/papers/2608.23070 (2026-08-24)
[7] World Models Survey | Comprehensive Overview. web. https://world-models.io/en/research/world-models-survey/ (n.d.)
[8] World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications. web. https://arxiv.org/abs/2606.00133 (2026-06-01)
[9] DreamForge-World 0.1 Preview: A Low-Compute Real-Time Controllable World Model. hf-search. https://huggingface.co/papers/2606.30292 (2026-06-29)
[10] Understanding World or Predicting Future? A Comprehensive Survey of World Models | ACM Computing Surveys. web. https://dl.acm.org/doi/10.1145/3746449 (2025-09-09)
[11] Agentic World Modeling: Foundations, Capabilities, Laws, and Beyond. web. https://arxiv.org/html/2604.22748v1 (2026-04-24)
