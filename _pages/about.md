---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

Hi, I'm **Jun-Yu Pan**. I will begin an M.Eng. in Electronic Information at the [SJTU Paris Elite Institute of Technology](https://speit.sjtu.edu.cn/), [Shanghai Jiao Tong University](https://www.sjtu.edu.cn/), in September 2026, advised by [Prof. Wei-Long Zheng](https://weilongzheng.github.io/). I received my B.Eng. from the same institute in June 2026, with an Outstanding Bachelor's Thesis (Top 1%).

I am currently a Research Intern at [Microsoft Research Asia (MSRA)](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/), advised by [Yansen Wang](https://www.microsoft.com/en-us/research/people/yansenwang/). My research focuses on **EEG foundation models**, **multimodal large language models (MLLMs)**, and their applications to neural understanding and affective computing.

News
======
- **2026.06** My bachelor's thesis was recognized as an Outstanding Bachelor's Thesis (Top 1%) by the SJTU Paris Elite Institute of Technology.
- **2026.05** Our work on Generative Visual Grounding for EEG understanding became available on [arXiv](https://arxiv.org/abs/2605.18172).
- **2026.05** We completed two studies on pretraining-data scaling and multi-dataset fine-tuning for EEG foundation models.
- **2026** We completed M4Lego, a multimodal pretraining framework for gameplay emotion recognition.
- **2025.04** I joined Microsoft Research Asia as a Research Intern.
- **2025** Our cross-scenario EEG emotion-recognition paper was published at ICASSP 2025.

Publications
======
1. **Jun-Yu Pan**, Yansen Wang, Enze Zhang, Bao-Liang Lu, Wei-Long Zheng, and Dongsheng Li. ["Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs."](https://arxiv.org/abs/2605.18172) Available on *arXiv*.
2. **Jun-Yu Pan**, Ruicheng Yin, Yansen Wang, Bao-Liang Lu, Wei-Long Zheng, and Dongsheng Li. "Which Data, Not How Much: A Controlled Audit of Data Scaling in EEG Foundation Models." Manuscript, 2026.
3. Ruicheng Yin, **Jun-Yu Pan**, Yansen Wang, Xiaoqing Zheng, and Dongsheng Li. "Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models." Manuscript, 2026.
4. <strong>Jun-Yu Pan</strong><sup>&dagger;</sup>, Jing-Yi Liu<sup>&dagger;</sup>, Bao-Liang Lu, and Wei-Long Zheng. "M4Lego: A Multi-Modal Pretraining Framework with Multi-Level Masking and Lego Blocks for Emotion Recognition During Gameplay." Manuscript, 2026.
5. **Jun-Yu Pan**, Hao-Long Yin, and Wei-Long Zheng. ["Double Domain Converter Transformer for Improving EEG-Based Emotion Recognition from Video to Game Scenarios."](https://ieeexplore.ieee.org/document/10889052) *ICASSP 2025*.

&dagger; Equal contribution.

[View all publications](/publications/)

Selected Research Projects
======
### Generative Visual Grounding for Universal EEG Understanding
*Microsoft Research Asia*

- Proposed Generative Visual Grounding (GVG), which uses an EEG-to-image generator to create instance-specific proxy images and maps EEG into discrete visual tokens for MLLMs.
- Built GVG-X-Omni and GVG-Janus with image-only and Image+Text alignment. GVG-X-Omni matched a 1.7B-parameter text-aligned baseline while tuning 170M parameters on a frozen 7B backbone.

### Data Scaling and Curation for EEG Foundation Models
*Microsoft Research Asia*

- Audited 151 pretraining configurations across LaBraM, CBraMod, and BIOT, covering 16 public datasets and 13 downstream tasks.
- Developed codebook-coverage H-ordering and Pairwise Dataset Valuation (PDV); informed subsets outperformed full-pool pretraining by up to 5.53 percentage points in balanced accuracy.

### Probe-Guided Multi-Dataset Fine-Tuning
*Microsoft Research Asia*

- Developed POSE, a target-conditioned framework that selects and weights auxiliary EEG datasets using distributional-distance trajectories in a target-adapted feature space.
- Evaluated POSE on 12 datasets and two EEG foundation models, improving average target-only fine-tuning by 3--4% while mitigating negative transfer.

### Cross-Scenario and Multimodal Emotion Recognition
*BCMI, Shanghai Jiao Tong University*

- Proposed DDCT for EEG emotion recognition across video and gameplay scenarios; the work was published at ICASSP 2025.
- Developed M4Lego, a multimodal pretraining framework integrating EEG and eye movements for emotion recognition during gameplay.

Research Experience
======
- **Apr. 2025--Present:** Research Intern, [Microsoft Research Asia](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/). Advisor: [Yansen Wang](https://www.microsoft.com/en-us/research/people/yansenwang/).
- **Jun. 2023--Jun. 2026:** Research Assistant, [BCMI](https://bcmi.sjtu.edu.cn/), Shanghai Jiao Tong University. Advisor: [Prof. Wei-Long Zheng](https://weilongzheng.github.io/).

[Download my CV](/files/Jun-Yu_Pan_CV.pdf)
