---
layout: archive
title: "个人简历"
permalink: /zh/cv/
author_profile: true
---

[English](/cv/) &nbsp;·&nbsp; **中文**

[中文简历（PDF）](/files/Jun-Yu_Pan_CV_ZH.pdf) &nbsp;·&nbsp; [English CV (PDF)](/files/Jun-Yu_Pan_CV.pdf)

教育背景
======
- **上海交通大学**，上海<br>
  电子信息硕士，上海交通大学巴黎卓越工程师学院<br>
  2026 年 9 月--2029 年 3 月（预计）<br>
  导师：郑伟龙副教授<br>
  研究方向：EEG Foundation Model、Multimodal Large Language Model (MLLM) 及 EEG Foundation Model 应用

- **上海交通大学**，上海<br>
  工学学士，上海交通大学巴黎卓越工程师学院<br>
  2022 年 9 月--2026 年 6 月<br>
  学积分：87.12/100 | GPA：3.66/4.3 | 排名：7/19<br>
  荣誉：上海交通大学优异学士学位论文（Top 1%）；三等奖学金（Top 15%）；学业进步奖学金

科研经历
======
- **微软亚洲研究院（MSRA）**，Research Intern<br>
  Shanghai AI/ML Group | Brain Project（Star Project）| 2025 年 4 月--至今<br>
  Top 5% Intern | 导师：王延森高级研究员<br>
  研究 data-centric EEG Foundation Model 与 EEG-MLLM alignment，涵盖预训练数据选择、多数据集微调和 Generative Visual Grounding。

- **上海交通大学仿脑计算与机器智能研究中心（BCMI）**，Research Assistant<br>
  2023 年 6 月--2026 年 6 月 | 导师：郑伟龙副教授<br>
  研究基于 EEG 的情感计算，包括跨场景、对比学习和多模态情感识别。

项目
======
*微软亚洲研究院 | Brain Project（Star Project）*

- **Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs**
  - 研究如何利用 MLLM 提升 EEG 的理解与生成能力。
  - 提出 Generative Visual Grounding (GVG)，利用 EEG-to-image generator 生成样本级 proxy image，并将 EEG 映射为离散 visual token，使 MLLM 能够复用预训练视觉先验。
  - 构建 GVG-X-Omni 与 GVG-Janus；前者在冻结 7B backbone、仅训练 170M 参数时达到 1.7B 参数文本对齐 baseline 的性能，Image+Text alignment 进一步提升效果。

- **Which Data, Not How Much: A Controlled Audit of Data Scaling in EEG Foundation Models**
  - 研究基础脑电大模型预训练过程中的数据集干扰问题。
  - 在 LaBraM、CBraMod 和 BIOT 上开展 151 组受控预训练实验，覆盖 16 个公开数据集与 13 个下游任务，并提出 H-ordering 与 Pairwise Dataset Valuation (PDV)。
  - 所选数据子集相较全量预训练最高提升 5.53 个 balanced accuracy 百分点，表明预训练效果取决于数据集兼容性而非单纯的数据规模。

- **Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models**
  - 研究基础脑电大模型下游微调过程中的数据集干扰问题。
  - 提出 POSE，在 target-adapted feature space 中依据 MMD 与 Fréchet distance trajectory 选择并加权辅助数据集，并采用 warm-up、joint-training 与 cool-down 训练流程。
  - 在 12 个数据集和两个 EEG Foundation Model 上较 target-only fine-tuning 平均提升 3--4%，并有效缓解 negative transfer。

*BCMI，上海交通大学*

- **Double Domain Converter Transformer for Improving EEG-Based Emotion Recognition from Video to Game Scenarios**
  - 研究视频与游戏场景间 EEG 分布差异造成的跨场景情感识别性能下降问题。
  - 提出 Double Domain Converter Transformer (DDCT)，通过 adversarial learning 将双 domain converter 与 Transformer 结合，保留情感信息并缩小场景分布差异。
  - 在视频--游戏混合场景和视频到游戏跨场景任务上分别达到 84.95% 与 74.76% 的准确率，相关论文发表于 ICASSP 2025。

- **M4Lego: A Multi-Modal Pretraining Framework with Multi-Level Masking and Lego Blocks for Emotion Recognition During Gameplay**
  - 研究如何融合 EEG 与眼动信号，提升自然交互式游戏场景中的多模态情感识别能力。
  - 构建 M4Lego，结合 multi-level masking、asymmetric conditional positional encoding 与 Lego-style modular fusion，学习模态内和跨模态表征。
  - 在三项游戏情感识别任务的 balanced accuracy、F1 score 与 accuracy 上整体优于九个强基线，主要提升超过 3 个百分点，最高超过 9 个百分点。

论文
======
1. **Jun-Yu Pan**, Yansen Wang, Enze Zhang, Bao-Liang Lu, Wei-Long Zheng, and Dongsheng Li. ["Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs."](https://arxiv.org/abs/2605.18172) *International Conference on Learning Representations (ICLR)*, under review.
2. **Jun-Yu Pan**, Ruicheng Yin, Yansen Wang, Bao-Liang Lu, Wei-Long Zheng, and Dongsheng Li. "Which Data, Not How Much: A Controlled Audit of Data Scaling in EEG Foundation Models." *Advances in Neural Information Processing Systems (NeurIPS 2026)*, under review.
3. Ruicheng Yin, **Jun-Yu Pan**, Yansen Wang, Xiaoqing Zheng, and Dongsheng Li. "Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models." *Advances in Neural Information Processing Systems (NeurIPS 2026)*, under review.
4. <strong>Jun-Yu Pan</strong><sup>&dagger;</sup>, Jing-Yi Liu<sup>&dagger;</sup>, Bao-Liang Lu, and Wei-Long Zheng. "M4Lego: A Multi-Modal Pretraining Framework with Multi-Level Masking and Lego Blocks for Emotion Recognition During Gameplay." *IEEE Transactions on Affective Computing*, under review.
5. **Jun-Yu Pan**, Hao-Long Yin, and Wei-Long Zheng. ["Double Domain Converter Transformer for Improving EEG-Based Emotion Recognition from Video to Game Scenarios."](https://ieeexplore.ieee.org/document/10889052) *ICASSP 2025*.

&dagger; 共同一作。

技术能力
======
- **编程语言：** Python、C
- **机器学习框架：** PyTorch
- **语言：** 中文、英语、法语
