---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

**English** &nbsp;·&nbsp; [中文](/zh/)

Hi, I'm **Jun-Yu Pan**. I will begin an M.Eng. in Electronic Information at the [SJTU Paris Elite Institute of Technology](https://speit.sjtu.edu.cn/), [Shanghai Jiao Tong University](https://www.sjtu.edu.cn/), in September 2026, advised by [Prof. Wei-Long Zheng](https://weilongzheng.github.io/). I received my B.Eng. from the same institute in June 2026, with an Outstanding Bachelor's Thesis of Shanghai Jiao Tong University (Top 1%).

I am currently a Research Intern with the Brain Project (Star Project) in the Shanghai AI/ML Group at [Microsoft Research Asia (MSRA)](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/), advised by [Yansen Wang](https://www.microsoft.com/en-us/research/people/yansenwang/), and was recognized as a **Top 5% Intern**. My research focuses on **EEG foundation models**, **multimodal large language models (MLLMs)**, and their applications to neural understanding and affective computing.

News
======
- **2026.09** We developed MSDE for multi-scale future-state EEG pretraining and updated our studies on pretraining-data selection, multi-dataset fine-tuning, and generative visual grounding.
- **2026.09** We completed a study introducing strategy-open BCI and examining how users form and revise their own interaction strategies in a continuous EEG-based task.
- **2026.06** My bachelor's thesis was recognized as an Outstanding Bachelor's Thesis of Shanghai Jiao Tong University (Top 1%).
- **2026.05** Our work on Generative Visual Grounding for EEG understanding became available on [arXiv](https://arxiv.org/abs/2605.18172).
- **2026.05** We completed two studies on pretraining-data scaling and multi-dataset fine-tuning for EEG foundation models.
- **2026** We completed M4Lego, a multimodal pretraining framework for gameplay emotion recognition.
- **2025.04** I joined Microsoft Research Asia as a Research Intern.
- **2025** Our cross-scenario EEG emotion-recognition paper was published at ICASSP 2025.

Publications
======
1. **Jun-Yu Pan**, Ruicheng Yin, Yansen Wang, Bao-Liang Lu, Dongsheng Li, and Wei-Long Zheng. "From Static Descriptions to State Dynamics: Multi-Scale Pretraining for EEG Transfer." Under review, 2026.
2. Xin Xu<sup>&dagger;</sup>, <strong>Jun-Yu Pan</strong><sup>&dagger;</sup>, Ruicheng Yin, Zilong Wang, Dongqi Han, Dongsheng Li, Bao-Liang Lu, Wei-Long Zheng, and Yansen Wang. "Think It Your Way: Toward Strategy-Open Brain&ndash;Computer Interaction." Under review, 2026.
3. **Jun-Yu Pan**, Enze Zhang, Bao-Liang Lu, Wei-Long Zheng, Dongsheng Li, and Yansen Wang. ["Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs."](https://arxiv.org/abs/2605.18172) Available on *arXiv*.
4. **Jun-Yu Pan**, Ruicheng Yin, Bao-Liang Lu, Wei-Long Zheng, Dongsheng Li, and Yansen Wang. "Which Data, Not How Much: Architecture-Dependent Data Selection for EEG Foundation Models." Under review, 2026.
5. Ruicheng Yin, **Jun-Yu Pan**, Yansen Wang, Xiaoqing Zheng, and Dongsheng Li. "Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models." Under review, 2026.
6. <strong>Jun-Yu Pan</strong><sup>&dagger;</sup>, Jing-Yi Liu<sup>&dagger;</sup>, Bao-Liang Lu, and Wei-Long Zheng. "M4Lego: A Multi-Modal Pretraining Framework with Multi-Level Masking and Lego Blocks for Emotion Recognition During Gameplay." Under review, 2026.
7. **Jun-Yu Pan**, Hao-Long Yin, and Wei-Long Zheng. ["Double Domain Converter Transformer for Improving EEG-Based Emotion Recognition from Video to Game Scenarios."](https://ieeexplore.ieee.org/document/10889052) *ICASSP 2025*.

&dagger; Equal contribution.

[View all publications](/publications/)

Selected Research Projects
======
### Large-Scale Pretraining and Model Scaling for EEG Foundation Models
*Microsoft Research Asia · Brain Project (Star Project)*

- Investigated how increasing pretraining-data volume and model capacity affects transfer across EEG tasks, studying data and model scaling together.
- Independently handled the full workflow, from data curation and quality control to pretraining and downstream evaluation. Expanded the corpus to 515 sources and approximately 80,000 hours of windowed EEG; conducted experiments across the 25k, 49k, and 79k corpus series and Base-to-Giant models spanning 5.8M to 1.97B encoder parameters.
- In the complete 23-task comparison, 49k Large achieved 59.05% mean balanced accuracy with full fine-tuning and 54.09% with linear probing. It ranked first by average task rank in both settings among 12 evaluated local checkpoints, including reproduced LaBraM, CBraMod, and REVE baselines.

### From Static Descriptions to State Dynamics: Multi-Scale Pretraining for EEG Transfer
*Microsoft Research Asia · Brain Project (Star Project)*

- Studied how predicting future EEG states at different time scales can capture both transient events and sustained rhythms for transfer across tasks.
- Developed MSDE, which jointly predicts micro- and macro-scale future teacher states using a causal encoder and a shared, elapsed-time-conditioned transition operator.
- MSDE-Full and MSDE-10% achieved the two best average fine-tuning ranks across 20 OmniEEG-Bench tasks among eight evaluated models. MSDE-10% uses a 5.0M-parameter encoder pretrained on 2,115 hours of EEG; joint-scale supervision outperformed both single-scale variants on 18 of 20 tasks.

### Think It Your Way: Toward Strategy-Open Brain&ndash;Computer Interaction
*Microsoft Research Asia · Brain Project (Star Project)*

- Introduced strategy-open BCI, which specifies the task goal while allowing users to form and revise their own mental strategies rather than follow a prescribed interaction mapping.
- Conducted an offline study with 26 participants in a continuous three-lane parkour task using EEG and self-reports. Strategies were heterogeneous and revised mainly early; reported modalities partially matched physiological signatures, while movement direction and target lane remained decodable across visual themes.

### Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs
*Microsoft Research Asia · Brain Project (Star Project)*

- Studied how MLLMs can use their pretrained visual knowledge to improve EEG understanding and generation, including tasks without visual stimuli.
- Proposed GVG, using an EEG-to-image generator to create sample-specific proxy images, predict native visual tokens, and align EEG, images, and text.
- On six tasks, GVG-Janus improved mean balanced accuracy from 45.89% with text-only alignment to 53.46% with image-only alignment; trimodal alignment with full adaptation reached 60.05%. GVG-X-Omni approached NeuroLM-XL's average performance while tuning 170M parameters over a frozen 7B backbone.

### Which Data, Not How Much: Architecture-Dependent Data Selection for EEG Foundation Models
*Microsoft Research Asia · Brain Project (Star Project)*

- Studied interference among EEG pretraining datasets and how source composition, data volume, and model architecture affect downstream transfer.
- Audited 202 configurations across LaBraM, CBraMod, and BIOT, covering 16 candidate datasets and 13 downstream tasks; compared Progressive, Pairwise Dataset Valuation (PDV), Size, and Coverage rankings.
- Found 121 configurations that used fewer windows yet outperformed full-pool pretraining. The best subsets improved mean balanced accuracy by up to 5.58 percentage points; all 39 architecture-task combinations had a smaller, higher-scoring configuration.

### Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models
*Microsoft Research Asia · Brain Project (Star Project)*

- Studied interference during downstream multi-dataset fine-tuning and when auxiliary EEG datasets help or hurt a target task.
- Developed POSE, which uses MMD and Fréchet-distance levels and trends during target adaptation to select and weight auxiliary datasets, then schedules their participation through warm-up, joint training, and cool-down.
- Evaluated on 12 datasets. Mean balanced accuracy over 11 classification tasks increased from 54.5% to 56.0% on LaBraM and from 52.8% to 55.0% on CBraMod versus target-only fine-tuning, with gains on 10 and 9 of the 12 targets, respectively.

### Cross-Scenario and Multimodal Emotion Recognition
*BCMI, Shanghai Jiao Tong University*

- Proposed DDCT for EEG emotion recognition across video and gameplay scenarios; the work was published at ICASSP 2025.
- Developed M4Lego, a multimodal pretraining framework integrating EEG and eye movements for emotion recognition during gameplay.

Research Experience
======
- **Apr. 2025--Present:** Research Intern, Brain Project (Star Project), Shanghai AI/ML Group, [Microsoft Research Asia](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/); **Top 5% Intern**. Advisor: [Yansen Wang](https://www.microsoft.com/en-us/research/people/yansenwang/).
- **Jun. 2023--Jun. 2026:** Research Assistant, [BCMI](https://bcmi.sjtu.edu.cn/), Shanghai Jiao Tong University. Advisor: [Prof. Wei-Long Zheng](https://weilongzheng.github.io/).

[English CV (PDF)](/files/Jun-Yu_Pan_CV.pdf)
