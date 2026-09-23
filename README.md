# Ying JIN — Machine Learning Portfolio

Selected MVA projects in **model training, evaluation and optimization**, with a focus on language models and research engineering. These repositories contain collaborative coursework and research implementations; each project preserves its authors and original method references.

## Selected projects

| Project | What to explore | Collaboration |
|---|---|---|
| [APOLLO optimizer reproduction](https://github.com/PineappleBlowsnow/Course-project-APOLLO-SGD-LIKE-MEMORY-ADAMW-LEVEL-PERFORMANCE) | Small language-model training, optimizer diagnostics and the memory–quality trade-off against AdamW; source, configurations and a joint report. | Ying Jin and Felipe Vicentin |
| [Attention sinks and activation outliers](https://github.com/PineappleBlowsnow/xai-outlier-repro) | Evaluation of softmax-1 attention and OrthoAdam in small GPT-2-style models; attention/activation analyses, perplexity and post-training quantization. | Tristan MARTIN and Ying JIN; [upstream](https://github.com/Tristan22400/xai-outlier-repro) |
| [Mamba S6 from scratch](https://github.com/PineappleBlowsnow/Mamba-S6-From-Scratch) | Selective state-space computations in PyTorch; causal/bidirectional image experiments, RNN comparisons and TinyShakespeare language modeling. | Clement Marie and Ying JIN; [upstream](https://github.com/clmrie/Mamba-S6-From-Scratch) |
| [Consistency Models and noisy inverse problems](https://github.com/PineappleBlowsnow/Consistency-Model-vs-Diffusion-Posterior-Sampling-for-Noisy-Inverse-Problem) | A study of consistency models, diffusion methods and noisy inverse problems, with the course report and experimental code. | JIN Ying and HAMMANI Ianis |
| [Mixture Density Networks and GatedDual](https://github.com/PineappleBlowsnow/mdn-gated-dual) | Conditional density estimation and a gated two-expert comparison. The report credits Ying with experiments 2–4, GatedDual implementation and analysis. | Ying JIN and Gloire LINVANI |
| [Static mean-field games](https://github.com/PineappleBlowsnow/static-mean-field-games) | TRPA/annealed-TRPA comparisons, population scaling and exploratory bilevel intervention in synthetic environments; code and a joint course research report. | Jin Ying and Zhao Yutai |
| [Molecular Graph Captioning — ALTeGraD multimodal challenge](https://github.com/PineappleBlowsnow/MVA-Graph2text-kaggle-challenge) | Feature-aware GINE/BERT contrastive retrieval and graph-conditioned DistilGPT2, BioGPT/LoRA and BioT5/LoRA experiments. Separate from the ALTeGraD practicals; data and weights excluded. | Ying Jin's coursework portfolio; course scaffold credited and contribution-record limits documented |

## One concrete trade-off

In the joint APOLLO experiment on **LLaMA-60M / TinyStories / 10,000 training steps**, the rank-1/8 setting used **0.0541 GB of optimizer-state memory**, versus **0.4327 GB for AdamW**. Evaluation perplexity was **4.13 versus 3.61**, respectively. The 87.5% reduction concerns optimizer state, not total GPU memory, and comes with a quality difference. See the repository report for the setup and other variants.

## Course foundations

Project and practical work spans training large-scale models, LLMs for code and proof, explainable AI, deep learning, probabilistic graphical models, text/graph learning, reinforcement learning, optimization, generative modeling and deep learning for signals.

## How to read this portfolio

Start with each repository's README, then its report or poster and executable entry points. The XAI and Mamba forks retain the original project history and provide a `docs/PORTFOLIO.md` guide. A coauthored result is not presented as a solo contribution. Existing methods are credited, and repository-specific licenses remain authoritative.

The September 2026 documentation refresh checked source paths and static Python syntax. It did not rerun model training or establish new benchmark results; historical results remain tied to the experiments described in the individual reports.

[GitHub profile](https://github.com/PineappleBlowsnow) · [LinkedIn](https://www.linkedin.com/in/ying-jin94/)
