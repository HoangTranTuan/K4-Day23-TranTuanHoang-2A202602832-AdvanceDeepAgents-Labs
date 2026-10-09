# Survey on Reinforcement Learning for LLM Reasoning

## TL;DR
- RL for language models has expanded from preference alignment toward reasoning with verifiable rewards [17][16].
- Optimization methods address stability, sample reuse, and distributed training [6][14][5].
- Agreement-based rewards and staged curricula offer different ways to guide learning [15][13][4].
- Results span mathematics, tables, and finance, but gains depend on the task and training setting [12][11][10][1].

## Background
RL adjusts model behavior to improve expected rewards. Reasoning systems use correctness signals for tasks such as mathematics and coding, alongside earlier human-feedback approaches. Surveys connect this shift with broader methods for reasoning in foundation models [17][16].

## RL Optimization Methods
DISPO targets efficient, stable mathematical reasoning training; BAPO reuses off-policy data to improve sampling efficiency. Fed-GRPO studies reward-driven optimization in federated settings. These methods address different constraints and should be compared under matching training and evaluation conditions [6][14][5].

## Rewards and Curriculum Learning
Co-Reward uses contrastive agreement for self-supervised rewards, while staged learning and RuCL organize training by difficulty and rubric structure [15][13][4]. Inverse RL learns reasoning reward models from expert demonstrations; GRPODropout investigates rollout selection. Together, these directions link reward quality with exploration and training efficiency [9][3].

## Alternatives and Continual Learning
Functional repertoire evolution explores continual learning through reusable capabilities. It represents a complementary direction to parameter-update RL, rather than evidence that one method uniformly replaces the other [2][17].

## Results and Benchmarks
One-example RL investigates data-efficient mathematical reasoning, while Reasoning-Table and Fin-R1 specialize in table and financial tasks [12][11][10]. ProRL studies the effect of prolonged RL training, and demonstration-based reward learning offers another route to improving reasoning supervision [1][9]. These results cover different datasets and settings, limiting direct comparisons [12][11][10][1].

## Trends and Open Problems
Surveys emphasize reward robustness, efficient optimization, and the relationship between language models and broader RL systems [8][7]. Remaining challenges include generalizing rewards across domains, maintaining exploration, and comparing methods with consistent baselines and computational budgets [17][8][3].

## References
[1] ProRL: Prolonged Reinforcement Learning Expands Reasoning Boundaries in Large Language Models. hf-search. https://huggingface.co/papers/2505.24864 (2025-05-30)
[2] From a Prompt to Repertoires: Evolving Functional REpertoires Enable LLM Continual Learning. arxiv. https://arxiv.org/abs/2610.11373 (2026-10-08)
[3] GRPODropout: Less is More for Online Reinforcement Learning Rollouts. arxiv. https://arxiv.org/abs/2610.11854 (2026-10-08)
[4] RuCL: Stratified Rubric-Based Curriculum Learning for Multimodal Large Language Model Reasoning. hf-search. https://huggingface.co/papers/2602.21628 (2026-02-25)
[5] Fed-GRPO: Reward-Signal-Driven Federated Group Relative Policy Optimization. arxiv. https://arxiv.org/abs/2610.11502 (2026-10-08)
[6] DISPO: Enhancing Training Efficiency and Stability in Reinforcement Learning for Large Language Model Mathematical Reasoning. hf-search. https://huggingface.co/papers/2602.00983 (2026-02-01)
[7] LLM-Enhanced Reinforcement Learning: A Survey. web. https://arxiv.org/pdf/2404.00282 (n.d.)
[8] Reinforcement Learning Enhanced LLMs: A Survey. web. https://arxiv.org/html/2412.10400v1 (2024-12-05)
[9] Learning Reasoning Reward Models from Expert Demonstration via Inverse Reinforcement Learning. hf-search. https://huggingface.co/papers/2510.01857 (2025-10-02)
[10] Fin-R1: A Large Language Model for Financial Reasoning through Reinforcement Learning. hf-search. https://huggingface.co/papers/2503.16252 (2025-03-20)
[11] Reasoning-Table: Exploring Reinforcement Learning for Table Reasoning. hf-search. https://huggingface.co/papers/2506.01710 (2025-06-02)
[12] Reinforcement Learning for Reasoning in Large Language Models with One Training Example. hf-search. https://huggingface.co/papers/2504.20571 (2025-04-29)
[13] How Difficulty-Aware Staged Reinforcement Learning Enhances LLMs' Reasoning Capabilities: A Preliminary Experimental Study. hf-search. https://huggingface.co/papers/2504.00829 (2025-04-01)
[14] Buffer Matters: Unleashing the Power of Off-Policy Reinforcement Learning in Large Language Model Reasoning. hf-search. https://huggingface.co/papers/2602.20722 (2026-03-16)
[15] Co-Reward: Self-supervised Reinforcement Learning for Large Language Model Reasoning via Contrastive Agreement. hf-search. https://huggingface.co/papers/2508.00410 (2025-08-01)
[16] A Survey of Reasoning with Foundation Models: Concepts, Methodologies, and Outlook. web. https://dl.acm.org/doi/10.1145/3729218 (2025-06-12)
[17] A Survey of Reinforcement Learning for Large Reasoning Models. arxiv. https://arxiv.org/abs/2509.08827 (n.d.)
