---
permalink: /zh/
title: ""
author_profile: true
---

[English](/) &nbsp;·&nbsp; **中文**

你好，我是**潘俊宇（Jun-Yu Pan）**。我将于 2026 年 9 月在[上海交通大学巴黎卓越工程师学院](https://speit.sjtu.edu.cn/)攻读电子信息硕士学位，导师为[郑伟龙教授](https://weilongzheng.github.io/)，预计于 2029 年 3 月毕业。我于 2026 年 6 月本科毕业于同一学院，本科毕业论文获评上海交通大学优异学士学位论文（Top 1%）。

目前，我在 [Microsoft Research Asia (MSRA)](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/) Shanghai AI/ML Group 担任 Research Intern，导师为 [Yansen Wang](https://www.microsoft.com/en-us/research/people/yansenwang/)。我的研究方向包括 **EEG Foundation Model**、**Multimodal Large Language Model (MLLM)**，以及其在神经理解和情感计算中的应用。

最新动态
======
- **2026.06** 本科毕业论文获评上海交通大学优异学士学位论文（Top 1%）。
- **2026.05** Generative Visual Grounding EEG 理解工作已发布于 [arXiv](https://arxiv.org/abs/2605.18172)。
- **2026.05** 完成两项关于 EEG Foundation Model 预训练数据扩展与多数据集微调的研究。
- **2026** 完成面向游戏场景多模态情感识别的 M4Lego 预训练框架。
- **2025.04** 加入 Microsoft Research Asia，担任 Research Intern。
- **2025** 跨场景 EEG 情感识别工作发表于 ICASSP 2025。

论文
======
1. **Jun-Yu Pan**, Yansen Wang, Enze Zhang, Bao-Liang Lu, Wei-Long Zheng, and Dongsheng Li. ["Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs."](https://arxiv.org/abs/2605.18172) Available on *arXiv*.
2. **Jun-Yu Pan**, Ruicheng Yin, Yansen Wang, Bao-Liang Lu, Wei-Long Zheng, and Dongsheng Li. "Which Data, Not How Much: A Controlled Audit of Data Scaling in EEG Foundation Models." Manuscript, 2026.
3. Ruicheng Yin, **Jun-Yu Pan**, Yansen Wang, Xiaoqing Zheng, and Dongsheng Li. "Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models." Manuscript, 2026.
4. <strong>Jun-Yu Pan</strong><sup>&dagger;</sup>, Jing-Yi Liu<sup>&dagger;</sup>, Bao-Liang Lu, and Wei-Long Zheng. "M4Lego: A Multi-Modal Pretraining Framework with Multi-Level Masking and Lego Blocks for Emotion Recognition During Gameplay." Manuscript, 2026.
5. **Jun-Yu Pan**, Hao-Long Yin, and Wei-Long Zheng. ["Double Domain Converter Transformer for Improving EEG-Based Emotion Recognition from Video to Game Scenarios."](https://ieeexplore.ieee.org/document/10889052) *ICASSP 2025*.

&dagger; 共同一作。

项目
======
### 面向通用 EEG 理解的 Generative Visual Grounding
*Microsoft Research Asia*

- 提出 Generative Visual Grounding (GVG)，利用 EEG-to-image generator 生成与样本对应的 proxy image，并将 EEG 映射为离散 visual token，使 MLLM 能够复用预训练视觉先验。
- 构建 GVG-X-Omni 与 GVG-Janus，分别采用 Image-only 与 Image+Text alignment；GVG-X-Omni 在冻结 7B backbone、仅训练 170M 参数的情况下达到 1.7B 参数文本对齐 baseline 的性能，并通过三模态对齐进一步提升效果。

### EEG Foundation Model 的数据扩展与数据选择
*Microsoft Research Asia*

- 对 LaBraM、CBraMod 和 BIOT 开展 151 组受控预训练实验，覆盖 16 个公开数据集与 13 个下游任务。
- 提出基于 codebook coverage 的 H-ordering 与 Pairwise Dataset Valuation (PDV) 数据选择方法；经过筛选的数据子集相较全量预训练最高提升 5.53 个 balanced accuracy 百分点。

### Probe-Guided Multi-Dataset Fine-Tuning
*Microsoft Research Asia*

- 提出 POSE：在 target-adapted feature space 中，根据 MMD 与 Fréchet distance trajectory 选择并加权辅助 EEG 数据集。
- 结合 warm-up、joint-training 与 cool-down 训练流程，在 12 个数据集和两个 EEG Foundation Model 上完成评估，较 target-only fine-tuning 平均提升 3--4%，并缓解 negative transfer。

### 跨场景与多模态情感识别
*BCMI，上海交通大学*

- 提出 Double Domain Converter Transformer (DDCT)，用于视频与游戏场景之间的 EEG 跨场景情感识别，相关工作发表于 ICASSP 2025。
- 构建 M4Lego，通过 multi-level masking 与 Lego-style block 融合 EEG 和眼动信号，实现游戏过程中的多模态情感识别。

科研经历
======
- **2025.04--至今：** Research Intern，Shanghai AI/ML Group，[Microsoft Research Asia](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/)。导师：[Yansen Wang](https://www.microsoft.com/en-us/research/people/yansenwang/)。
- **2023.06--2026.06：** Research Assistant，上海交通大学[仿脑计算与机器智能研究中心（BCMI）](https://bcmi.sjtu.edu.cn/)。导师：[郑伟龙教授](https://weilongzheng.github.io/)。

[English CV (PDF)](/files/Jun-Yu_Pan_CV.pdf)
