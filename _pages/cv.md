---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

**English** &nbsp;·&nbsp; [中文](/zh/cv/)

[English CV (PDF)](/files/Jun-Yu_Pan_CV.pdf) &nbsp;·&nbsp; [中文简历（PDF）](/files/Jun-Yu_Pan_CV_ZH.pdf)

Education
======
- **Shanghai Jiao Tong University**, Shanghai, China<br>
  M.Eng. in Electronic Information, SJTU Paris Elite Institute of Technology<br>
  September 2026 -- March 2029 (Expected)<br>
  Advisor: Prof. Wei-Long Zheng<br>
  Research interests: EEG foundation models, multimodal large language models, and applications of EEG foundation models

- **Shanghai Jiao Tong University**, Shanghai, China<br>
  Bachelor of Engineering, SJTU Paris Elite Institute of Technology<br>
  September 2022 -- June 2026<br>
  Weighted Average: 87.12/100 | GPA: 3.66/4.3 | Rank: 7/19<br>
  Honors: Outstanding Bachelor's Thesis of Shanghai Jiao Tong University (Top 1%); Third-Class Scholarship (Top 15%); Academic Progress Scholarship

Research Experience
======
- **Microsoft Research Asia (MSRA)**, Research Intern<br>
  Shanghai AI/ML Group | Brain Project (Star Project) | April 2025 -- Present<br>
  Top 5% Intern | Advisor: Yansen Wang<br>
  Research on EEG foundation models and EEG-MLLM alignment, spanning large-scale pretraining, model scaling, predictive learning, data selection, multi-dataset fine-tuning, and visual grounding. Completed four ICLR 2027 submissions (three as first author) and one co-first-author CHI 2027 submission.

- **BCMI, Shanghai Jiao Tong University**, Research Assistant<br>
  June 2023 -- June 2026 | Advisor: Prof. Wei-Long Zheng<br>
  Research on EEG-based affective computing, including cross-scenario, contrastive, and multimodal emotion recognition.

Selected Research Projects
======
*Microsoft Research Asia | Brain Project (Star Project)*

- **Large-Scale Pretraining and Model Scaling for EEG Foundation Models:** Independently handled data curation, quality control, pretraining, and evaluation to study data and model scaling. Expanded the corpus to 515 sources and approximately 80,000 hours of windowed EEG, with model variants spanning 5.8M to 1.97B encoder parameters. Across 23 downstream tasks, the developed models currently rank first by a substantial margin among all EEG foundation models.
- **From Static Descriptions to State Dynamics: Multi-Scale Pretraining for EEG Transfer:** Developed MSDE to jointly predict micro- and macro-scale future teacher states. MSDE-Full and MSDE-10% achieved the two best average fine-tuning ranks across 20 OmniEEG-Bench tasks among eight models; MSDE-10% uses a 5.0M-parameter encoder pretrained on 2,115 hours of EEG.
- **Think It Your Way: Toward Strategy-Open Brain&ndash;Computer Interaction:** Introduced strategy-open BCI in an offline study of 26 participants; combined EEG, self-reports, physiological-signature analysis, and cross-theme decoding of movement direction and target lane.
- **Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs:** Used EEG-to-image proxy generation and visual-token prediction to align EEG with MLLMs. GVG-Janus improved mean balanced accuracy across six tasks from 45.89% (text-only) to 53.46% (image-only); trimodal alignment with full adaptation reached 60.05%.
- **Which Data, Not How Much: Architecture-Dependent Data Selection for EEG Foundation Models:** Audited 202 configurations across three architectures, 16 candidate datasets, and 13 downstream tasks. Compared Progressive, PDV, Size, and Coverage rankings; 121 configurations beat full-pool pretraining with fewer windows, with best-subset gains up to 5.58 mean balanced-accuracy points.
- **Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models:** Developed POSE to select and weight auxiliary data from MMD and Fréchet-distance levels and trends, then schedule their participation. Across 12 datasets, mean balanced accuracy over 11 classification tasks improved by 1.5 points on LaBraM and 2.2 points on CBraMod over target-only fine-tuning.

*BCMI, Shanghai Jiao Tong University*

- **Cross-Scenario and Multimodal Emotion Recognition:** Developed DDCT and M4Lego for cross-scenario and multimodal gameplay emotion recognition.

Publications
======
1. **Jun-Yu Pan**, Ruicheng Yin, Yansen Wang, Bao-Liang Lu, Dongsheng Li, and Wei-Long Zheng. "From Static Descriptions to State Dynamics: Multi-Scale Pretraining for EEG Transfer." *International Conference on Learning Representations (ICLR 2027)*, under review.
2. Xin Xu<sup>&dagger;</sup>, <strong>Jun-Yu Pan</strong><sup>&dagger;</sup>, Ruicheng Yin, Zilong Wang, Dongqi Han, Dongsheng Li, Bao-Liang Lu, Wei-Long Zheng, and Yansen Wang. "Think It Your Way: Toward Strategy-Open Brain&ndash;Computer Interaction." *ACM CHI Conference on Human Factors in Computing Systems (CHI 2027)*, under review.
3. **Jun-Yu Pan**, Enze Zhang, Bao-Liang Lu, Wei-Long Zheng, Dongsheng Li, and Yansen Wang. ["Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs."](https://arxiv.org/abs/2605.18172) *International Conference on Learning Representations (ICLR 2027)*, under review.
4. **Jun-Yu Pan**, Ruicheng Yin, Bao-Liang Lu, Wei-Long Zheng, Dongsheng Li, and Yansen Wang. "Which Data, Not How Much: Architecture-Dependent Data Selection for EEG Foundation Models." *International Conference on Learning Representations (ICLR 2027)*, under review.
5. Ruicheng Yin, **Jun-Yu Pan**, Yansen Wang, Xiaoqing Zheng, and Dongsheng Li. "Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models." *International Conference on Learning Representations (ICLR 2027)*, under review.
6. <strong>Jun-Yu Pan</strong><sup>&dagger;</sup>, Jing-Yi Liu<sup>&dagger;</sup>, Bao-Liang Lu, and Wei-Long Zheng. "M4Lego: A Multi-Modal Pretraining Framework with Multi-Level Masking and Lego Blocks for Emotion Recognition During Gameplay." *IEEE Transactions on Affective Computing*, under review.
7. **Jun-Yu Pan**, Hao-Long Yin, and Wei-Long Zheng. ["Double Domain Converter Transformer for Improving EEG-Based Emotion Recognition from Video to Game Scenarios."](https://ieeexplore.ieee.org/document/10889052) *ICASSP 2025*.

&dagger; Equal contribution.

Technical Skills
======
- **Programming:** Python, C
- **Frameworks:** PyTorch
- **Languages:** Mandarin, English, French
