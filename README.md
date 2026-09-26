# Ying JIN — Machine Learning Portfolio

Selected MVA projects in **language-model training, efficient inference, evaluation and optimization**. The collection includes individual implementations and collaborative coursework, with original authors, course scaffolds and method references credited in each repository.

## Selected projects

| Project | What to explore | Contribution and provenance |
|---|---|---|
| [APOLLO optimizer reproduction](https://github.com/PineappleBlowsnow/Course-project-APOLLO-SGD-LIKE-MEMORY-ADAMW-LEVEL-PERFORMANCE) | LLaMA-60M training on TinyStories: optimizer-state memory versus validation perplexity, supported by configurations and archived results. | Implementation and experiments by Ying Jin; the submitted report's Ying Jin / Felipe Vicentin author list is preserved. |
| [Attention sinks and activation outliers](https://github.com/PineappleBlowsnow/xai-outlier-repro) | Ying's cross-model attention/activation diagnostics and token-replacement/context-length ablations, within a broader softmax-1/OrthoAdam study. | Tristan MARTIN and Ying JIN; personal analysis code identified in Git history; [upstream](https://github.com/Tristan22400/xai-outlier-repro). |
| [KV cache and LoRA](https://github.com/PineappleBlowsnow/llm-efficiency) | Cached autoregressive decoding, low-rank adapters and a synthetic sorting adaptation experiment in a small GPT. Includes implementation, smoke checks and historical CPU evidence. | Ying Jin's course implementation; course and minGPT sources credited. |
| [Triton attention lab](https://github.com/PineappleBlowsnow/triton-attention-lab) | Tiled online-softmax attention forward, a PyTorch backward, correctness tests and archived benchmarks. The backward still uses quadratic memory. | Ying Jin's implementation; course scaffolding and tests attributed. |
| [Gossip SGD and graph topologies](https://github.com/PineappleBlowsnow/gossip-sgd-topologies) | PyTorch/Gloo experiments on topology, communication frequency and model disagreement; separate 40-step CSVs and a 200-step transcript. | Ying JIN and Felipe VICENTIN; original submission preserved and per-author split not inferred. |
| [Mamba S6 from scratch](https://github.com/PineappleBlowsnow/Mamba-S6-From-Scratch) | Selective state-space computations in PyTorch; causal/bidirectional image experiments, RNN comparisons and TinyShakespeare language modeling. | Clement Marie and Ying JIN; [upstream](https://github.com/clmrie/Mamba-S6-From-Scratch) |
| [Consistency Models and inverse problems](https://github.com/PineappleBlowsnow/Consistency-Model-vs-Diffusion-Posterior-Sampling-for-Noisy-Inverse-Problem) | Consistency training/distillation and inverse-problem experiments. Audited inpainting results use zero measurement noise; broader noisy-inverse-problem aims are not treated as validated results. | JIN Ying and HAMMANI Ianis |
| [Mixture Density Networks and GatedDual](https://github.com/PineappleBlowsnow/mdn-gated-dual) | Conditional density estimation and a gated two-expert comparison. The report credits Ying with experiments 2–4, GatedDual implementation and analysis. | Ying JIN and Gloire LINVANI |
| [Static mean-field games](https://github.com/PineappleBlowsnow/static-mean-field-games) | TRPA/annealed-TRPA comparisons, population scaling and exploratory bilevel intervention in synthetic environments; code and a joint course research report. | Jin Ying and Zhao Yutai |
| [Molecular Graph Captioning — ALTeGraD multimodal challenge](https://github.com/PineappleBlowsnow/MVA-Graph2text-kaggle-challenge) | Feature-aware GINE/BERT contrastive retrieval and graph-conditioned DistilGPT2, BioGPT/LoRA and BioT5/LoRA experiments. Separate from the ALTeGraD practicals; data and weights excluded. | Ying Jin's coursework portfolio; course scaffold credited and contribution-record limits documented |
| [Zork — ReAct text-adventure agent](https://github.com/PineappleBlowsnow/zork-text-adventure-agent) | Location-aware failed-action memory, stagnation detection and fallback exploration in a ReAct agent using MCP tools. Includes the final course implementation and an attributed reference baseline. | Ying Jin's extensions to the course scaffold; no verified score claimed |

## One concrete trade-off

In the APOLLO experiment on **LLaMA-60M / TinyStories / 10,000 training steps**, the rank-1/8 setting used **0.0541 GiB of optimizer-state memory**, versus **0.4327 GiB for AdamW**. Best recorded validation perplexity was **4.13 versus 3.61**, respectively. The approximately 87.5% reduction concerns optimizer state, not total GPU memory, and comes with a quality difference. See the repository's result notes and archived CSVs for the setup and measurement limits.

## Course foundations

Project and practical work spans training large-scale models, LLMs for code and proof, explainable AI, deep learning, probabilistic graphical models, text/graph learning, reinforcement learning, optimization, generative modeling and deep learning for signals.

## How to read this portfolio

Start with each repository's README, then its report or poster and executable entry points. The XAI and Mamba forks retain the original project history and provide a `docs/PORTFOLIO.md` guide. Author lists and specific implementation contributions are documented separately where evidence permits. Existing methods are credited, and repository-specific licenses remain authoritative.

The **26 September 2026** refresh adds three repositories, bringing this page to **11 independent MVA projects**. Source paths, static syntax, provenance and archived artifacts were checked. Training and GPU benchmarks were not rerun; historical results remain tied to their original experiment settings. The additional [APOLLO/LLaMA variant](https://github.com/PineappleBlowsnow/Apollo_reproduction-with-llama) is not counted as a separate project.

[GitHub profile](https://github.com/PineappleBlowsnow) · [LinkedIn](https://www.linkedin.com/in/ying-jin94/)
