---
permalink: /zh/
title: ""
author_profile: true
---

[English](/) &nbsp;·&nbsp; **中文**

你好，我是**潘俊宇（Jun-Yu Pan）**。目前在 [Microsoft Research Asia (MSRA)](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/) Shanghai AI/ML Group 担任 Research Intern，导师为 [Yansen Wang](https://www.microsoft.com/en-us/research/people/yansenwang/)。我主要关注 **EEG Foundation Model**、**Multimodal Large Language Model (MLLM)** 以及 EEG Foundation Model 的应用。

我于 2026 年 6 月本科毕业于[上海交通大学巴黎卓越工程师学院](https://speit.sjtu.edu.cn/)，毕业论文获评上海交通大学优异学士学位论文（Top 1%）。2026 年 9 月起，我将在同一学院攻读电子信息硕士学位，师从[郑伟龙教授](https://weilongzheng.github.io/)，预计于 2029 年 3 月毕业。

最新动态
======
- **2026.06** 本科毕业论文获评上海交通大学优异学士学位论文（Top 1%）。
- **2026.05** Generative Visual Grounding EEG 理解工作上线 [arXiv](https://arxiv.org/abs/2605.18172)。
- **2026.05** 完成两项 EEG Foundation Model 研究，分别关注预训练数据选择与多数据集微调。
- **2026** 完成 M4Lego 初稿，研究游戏场景下的多模态情感识别。
- **2025.04** 加入 Microsoft Research Asia，担任 Research Intern。
- **2025** 跨场景 EEG 情感识别工作发表于 ICASSP 2025。

论文
======
1. **Jun-Yu Pan**, Yansen Wang, Enze Zhang, Bao-Liang Lu, Wei-Long Zheng, and Dongsheng Li. ["Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs."](https://arxiv.org/abs/2605.18172) Available on *arXiv*.
2. **Jun-Yu Pan**, Ruicheng Yin, Yansen Wang, Bao-Liang Lu, Wei-Long Zheng, and Dongsheng Li. "Which Data, Not How Much: A Controlled Audit of Data Scaling in EEG Foundation Models." Under review, 2026.
3. Ruicheng Yin, **Jun-Yu Pan**, Yansen Wang, Xiaoqing Zheng, and Dongsheng Li. "Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models." Under review, 2026.
4. <strong>Jun-Yu Pan</strong><sup>&dagger;</sup>, Jing-Yi Liu<sup>&dagger;</sup>, Bao-Liang Lu, and Wei-Long Zheng. "M4Lego: A Multi-Modal Pretraining Framework with Multi-Level Masking and Lego Blocks for Emotion Recognition During Gameplay." Under review, 2026.
5. **Jun-Yu Pan**, Hao-Long Yin, and Wei-Long Zheng. ["Double Domain Converter Transformer for Improving EEG-Based Emotion Recognition from Video to Game Scenarios."](https://ieeexplore.ieee.org/document/10889052) *ICASSP 2025*.

&dagger; 共同第一作者。

项目
======
### 面向通用 EEG 理解的 Generative Visual Grounding
*Microsoft Research Asia*

- 为了让 MLLM 更好地利用 EEG，我们提出 Generative Visual Grounding (GVG)：先由 EEG-to-image generator 生成对应的 proxy image，再把 EEG 映射为离散 visual token，从而复用模型已有的视觉先验。
- 基于这一思路，我们实现了 GVG-X-Omni 和 GVG-Janus。GVG-X-Omni 冻结 7B backbone、仅训练 170M 参数，即达到 1.7B 参数 text-aligned baseline 的表现；Image+Text alignment 还能进一步提升效果。

### EEG Foundation Model 的数据扩展与数据选择
*Microsoft Research Asia*

- 我们在 LaBraM、CBraMod 和 BIOT 上完成了 151 组受控预训练实验，覆盖 16 个公开数据集和 13 个下游任务，用统一设置比较数据来源与数据规模的影响。
- 在这些实验的基础上，我们提出基于 codebook coverage 的 H-ordering 与 Pairwise Dataset Valuation (PDV)。筛选后的数据子集相比全量预训练最高提升 5.53 个 balanced accuracy 百分点。

### Probe-Guided Multi-Dataset Fine-Tuning
*Microsoft Research Asia*

- 为了减少多数据集微调中的 negative transfer，我们设计了 POSE：在 target-adapted feature space 中，依据 MMD 与 Fréchet distance trajectory 选择并加权辅助 EEG 数据集。
- POSE 采用 warm-up、joint-training 和 cool-down 三阶段训练流程。在 12 个数据集和两个 EEG Foundation Model 上，它相比 target-only fine-tuning 平均提升 3--4%。

### 跨场景与多模态情感识别
*BCMI，上海交通大学*

- DDCT 关注从视频到游戏场景的 EEG 情感识别迁移，相关工作发表于 ICASSP 2025。
- M4Lego 则结合 EEG 与眼动信号，通过 multi-level masking 和 Lego-style block 建模游戏过程中的多模态情感。

科研经历
======
- **2025.04--至今：** Research Intern，[Microsoft Research Asia (MSRA)](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/) Shanghai AI/ML Group。导师：[Yansen Wang](https://www.microsoft.com/en-us/research/people/yansenwang/)。
- **2023.06--2026.06：** Research Assistant，上海交通大学[仿脑计算与机器智能研究中心（BCMI）](https://bcmi.sjtu.edu.cn/)。导师：[郑伟龙教授](https://weilongzheng.github.io/)。

[English CV (PDF)](/files/Jun-Yu_Pan_CV.pdf)
