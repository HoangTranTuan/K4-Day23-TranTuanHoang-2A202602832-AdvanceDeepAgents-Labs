# Survey on Video and Multimodal Generation

## TL;DR
- Video generation increasingly combines diffusion, transformer, and latent compression components [21][20][18].
- Multimodal systems coordinate text, images, audio, and video through unified models or modular pipelines [22][17][16][15].
- Evaluation covers visual quality, motion, text alignment, and safety [14][13][10].
- Long sequences, physical coherence, data efficiency, and human-aligned assessment remain difficult [11][9][3][1].

## Background
Video generation must maintain coherence across frames, while multimodal generation must align different forms of information. Surveys trace progress from GANs and VAEs toward diffusion and foundation models, covering both generative mechanisms and text-to-media applications [22][21][20][8][7].

## Video Generation Approaches
GANs favor sharp output but can be unstable; VAEs offer compact representations but may lose detail. Diffusion and transformer-based approaches improve modeling capacity with higher computational costs [21][20][19]. LTX-Video, CV-VAE, and VACE illustrate work on latent generation, compatible video representations, and integrated creation or editing [18][5][6].

## Multimodal Generation Approaches
Unified serving runtimes and modular skill systems address different parts of multimodal execution [17][16]. Native audio-visual dialogue and interactive speech synthesis extend generation beyond silent video, while physical-world modeling investigates cross-modal semantics [15][4][3]. Broader surveys place these approaches within modality fusion and text-to-media generation [22][12][8].

## Results and Evaluation
EvalCrafter assesses visual quality, motion, content fidelity, and text alignment using 17 objective metrics and human judgments [14][2]. VBench++ broadens video evaluation, while T2VSafetyBench examines safety under malicious and jailbreak prompts [10][13]. Quality and safety therefore require complementary evaluations rather than a single performance score [14][13][10].

## Trends and Open Problems
Long-video generation increases demands on planning, memory, and temporal consistency [11]. MUG-V 10B investigates efficient training pipelines, while multimodal interface research emphasizes adaptation and coherent interaction across platforms [9][1]. Open problems include scalable training, sustained physical consistency, and evaluation that reflects human expectations across modalities [12][11][3][1].

## References
[1] Generative AI in Multimodal User Interfaces: Trends, Challenges, and Cross-Platform Adaptability. arxiv. https://arxiv.org/abs/2411.10234 (2024-11-15)
[2] EvalCrafter: Benchmarking and Evaluating Large Video Generation Models. hf-search. https://huggingface.co/papers/2310.11440 (2023-10-17)
[3] OmniFysics-Nano-V2 Technical Report: Understanding the Physical World Across Modalities. arxiv. https://arxiv.org/abs/2609.25738 (2026-09-22)
[4] Interactive TTS: Dynamic Speaking Style Adaptation for Expressive Speech Synthesis. arxiv. https://arxiv.org/abs/2609.25707 (2026-09-22)
[5] CV-VAE: A Compatible Video VAE for Latent Generative Video Models. hf-search. https://huggingface.co/papers/2405.20279 (2024-05-30)
[6] VACE: All-in-One Video Creation and Editing. hf-search. https://huggingface.co/papers/2503.07598 (2025-03-10)
[7] Text-to-video generators: a comprehensive survey. web. https://link.springer.com/article/10.1186/s40537-025-01314-3 (2025-11-14)
[8] Next-Gen AIGC: a review of multimodal foundation models for text-to-media innovations. web. https://link.springer.com/article/10.1007/s11704-025-51171-9 (2026-02-20)
[9] MUG-V 10B: High-efficiency Training Pipeline for Large Video Generation Models. hf-search. https://huggingface.co/papers/2510.17519 (2025-10-20)
[10] VBench++: Comprehensive and Versatile Benchmark Suite for Video Generative Models. hf-search. https://huggingface.co/papers/2411.13503 (2024-11-20)
[11] Video Is Worth a Thousand Images: Exploring the Latest Trends in Long Video Generation. arxiv. https://arxiv.org/abs/2412.18688 (2024-12-24)
[12] A Survey of Generative Categories and Techniques in Multimodal Generative Models. arxiv. https://arxiv.org/abs/2506.10016 (2025-05-29)
[13] T2VSafetyBench: Evaluating the safety of text-to-video generative models. web. http://dl.acm.org/doi/10.5555/3737916.3739955 (2024-12-10)
[14] EvalCrafter: Benchmarking and Evaluating Large Video Generation Models. web. https://openaccess.thecvf.com/content/CVPR2024/papers/Liu_EvalCrafter_Benchmarking_and_Evaluating_Large_Video_Generation_Models_CVPR_2024_paper.pdf (2024)
[15] OmniVChat: Synthesizing, Benchmarking, and Training for Native Audio-Visual Dialogue. arxiv. https://arxiv.org/abs/2609.21465 (2026-09-18)
[16] Omni-IO Skills: Harnessing Your Agent Omni-Native. arxiv. https://arxiv.org/abs/2609.31847 (2026-09-25)
[17] vLLM-Omni Technical Report: A Unified Serving Runtime for Omni-Modality Generation. arxiv. https://arxiv.org/abs/2610.09307 (2026-10-07)
[18] LTX-Video: Realtime Video Latent Diffusion. hf-search. https://huggingface.co/papers/2501.00103 (2024-12-30)
[19] Bridging Text and Video Generation: A Survey. arxiv. https://arxiv.org/abs/2510.04999 (2025-10-06)
[20] A Survey on Video Diffusion Models. hf-search. https://huggingface.co/papers/2310.10647 (2023-10-16)
[21] Image Generation Models: A Technical History. arxiv. https://arxiv.org/abs/2603.07455 (2026-03-08)
[22] Generative AI for multimodal content: a survey with empirical and experimental evaluations. web. https://link.springer.com/article/10.1007/s10462-026-11525-6 (2026-03-19)
