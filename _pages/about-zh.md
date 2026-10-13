---
permalink: /zh/
title: ""
author_profile: true
---

[English](/) &nbsp;·&nbsp; **中文**

你好，我是**潘俊宇（Jun-Yu Pan）**。目前在 [Microsoft Research Asia (MSRA)](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/) Shanghai AI/ML Group 的 Brain Project（Star Project）担任 Research Intern，并获评 **Top 5% Intern**，导师为 [Yansen Wang](https://www.microsoft.com/en-us/research/people/yansenwang/)。我主要关注 **EEG Foundation Model**、**Multimodal Large Language Model (MLLM)** 以及 EEG Foundation Model 的应用。

我于 2026 年 6 月本科毕业于[上海交通大学巴黎卓越工程师学院](https://speit.sjtu.edu.cn/)，毕业论文获评上海交通大学优异学士学位论文（Top 1%）。2026 年 9 月起，我将在同一学院攻读电子信息硕士学位，师从[郑伟龙教授](https://weilongzheng.github.io/)，预计于 2029 年 3 月毕业。

最新动态
======
- **2026.09** 完成多尺度未来状态预训练方法 MSDE，并更新预训练数据选择、多数据集微调与生成式视觉对齐三项工作。
- **2026.09** 完成 strategy-open BCI 研究，考察用户在连续 EEG 交互任务中自主形成并调整交互策略的过程。
- **2026.06** 本科毕业论文获评上海交通大学优异学士学位论文（Top 1%）。
- **2026.05** Generative Visual Grounding EEG 理解工作上线 [arXiv](https://arxiv.org/abs/2605.18172)。
- **2026.05** 完成两项 EEG Foundation Model 研究，分别关注预训练数据选择与多数据集微调。
- **2026** 完成 M4Lego 初稿，研究游戏场景下的多模态情感识别。
- **2025.04** 加入 Microsoft Research Asia，担任 Research Intern。
- **2025** 跨场景 EEG 情感识别工作发表于 ICASSP 2025。

论文
======
1. **Jun-Yu Pan**, Ruicheng Yin, Yansen Wang, Bao-Liang Lu, Dongsheng Li, and Wei-Long Zheng. "From Static Descriptions to State Dynamics: Multi-Scale Pretraining for EEG Transfer." Under review, 2026.
2. Xin Xu<sup>&dagger;</sup>, <strong>Jun-Yu Pan</strong><sup>&dagger;</sup>, Ruicheng Yin, Zilong Wang, Dongqi Han, Dongsheng Li, Bao-Liang Lu, Wei-Long Zheng, and Yansen Wang. "Think It Your Way: Toward Strategy-Open Brain&ndash;Computer Interaction." Under review, 2026.
3. **Jun-Yu Pan**, Enze Zhang, Bao-Liang Lu, Wei-Long Zheng, Dongsheng Li, and Yansen Wang. ["Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs."](https://arxiv.org/abs/2605.18172) Available on *arXiv*.
4. **Jun-Yu Pan**, Ruicheng Yin, Bao-Liang Lu, Wei-Long Zheng, Dongsheng Li, and Yansen Wang. "Which Data, Not How Much: Architecture-Dependent Data Selection for EEG Foundation Models." Under review, 2026.
5. Ruicheng Yin, **Jun-Yu Pan**, Yansen Wang, Xiaoqing Zheng, and Dongsheng Li. "Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models." Under review, 2026.
6. <strong>Jun-Yu Pan</strong><sup>&dagger;</sup>, Jing-Yi Liu<sup>&dagger;</sup>, Bao-Liang Lu, and Wei-Long Zheng. "M4Lego: A Multi-Modal Pretraining Framework with Multi-Level Masking and Lego Blocks for Emotion Recognition During Gameplay." Under review, 2026.
7. **Jun-Yu Pan**, Hao-Long Yin, and Wei-Long Zheng. ["Double Domain Converter Transformer for Improving EEG-Based Emotion Recognition from Video to Game Scenarios."](https://ieeexplore.ieee.org/document/10889052) *ICASSP 2025*.

&dagger; 共同第一作者。

项目
======
### Large-Scale Pretraining and Model Scaling for EEG Foundation Models
*微软亚洲研究院 · Brain Project（Star Project）*

- 这项工作关注大规模 EEG 预训练：增加数据量和模型容量能带来怎样的跨任务迁移收益，以及如何有效扩展数据与模型。
- 我独立负责数据整理、质量控制、预训练和下游评测，将语料扩展至 515 个数据来源、约 8 万小时窗口化 EEG，开展 25k、49k、79k 三档语料实验，并构建从 Base 到 Giant、编码器参数量覆盖 5.8M 至 1.97B 的系列模型。
- 在 23 项下游任务评测中，所构建模型的整体性能在目前所有 EEG Foundation Models 中断档第一。

### From Static Descriptions to State Dynamics: Multi-Scale Pretraining for EEG Transfer
*微软亚洲研究院 · Brain Project（Star Project）*

- EEG 中既有短暂事件，也有持续节律。这项工作研究能否通过预测不同时间尺度的未来状态，让预训练模型学到更有利于迁移的动态特征。
- 我们提出 MSDE，用因果编码器表示已观测的 EEG，再通过一个以时间间隔为条件的共享转移算子，联合预测微观与宏观尺度的未来教师状态。
- 在 20 项 OmniEEG-Bench 任务上，MSDE-Full 与 MSDE-10% 在八个模型中取得前两位平均微调排名。MSDE-10% 的编码器仅有 5.0M 参数，使用 2,115 小时 EEG 预训练；联合尺度监督在 18 项任务上优于两种单尺度版本。

### Think It Your Way: Toward Strategy-Open Brain&ndash;Computer Interaction
*Microsoft Research Asia · Brain Project（Star Project）*

- 我们提出 strategy-open BCI：系统只规定任务目标，不预设 mental mapping，让用户自主形成并调整交互策略。
- 在 26 名受试者参与的连续三车道 parkour 任务中，我们联合分析 EEG、自报告与模态相关生理特征。结果显示，用户策略高度异质且调整主要发生在交互早期；主观报告与生理特征部分一致，同时 movement direction 和 target lane 在不同视觉主题下仍可解码。

### Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs
*微软亚洲研究院 · Brain Project（Star Project）*

- 这项工作研究如何利用 MLLM 已有的视觉知识提高 EEG 的理解与生成能力，包括没有视觉刺激的 EEG 任务。
- 我们提出 GVG，先由 EEG-to-image 生成器为每个样本生成代理图像，再预测模型原生的视觉 token，并进行 EEG、图像与文本的三模态对齐。
- 在六项任务上，GVG-Janus 的平均 balanced accuracy 从文本对齐的 45.89% 提升到图像对齐的 53.46%，三模态对齐结合全参数适配达到 60.05%。GVG-X-Omni 冻结 7B 主干、仅训练 170M 参数，平均表现接近 NeuroLM-XL。

### Which Data, Not How Much: Architecture-Dependent Data Selection for EEG Foundation Models
*微软亚洲研究院 · Brain Project（Star Project）*

- 预训练时加入更多 EEG 数据，并不总能带来更好的迁移效果。这项工作考察不同数据集之间的干扰，以及数据来源、规模和模型架构各自的影响。
- 我们在 LaBraM、CBraMod 和 BIOT 上评估了 202 组配置，覆盖 16 个候选数据集与 13 个下游任务，并比较 Progressive、Pairwise Dataset Valuation (PDV)、Size 和 Coverage 四种排序方法。
- 其中 121 组配置使用更少的训练窗口，却优于全量预训练；最佳子集的平均 balanced accuracy 最高提升 5.58 个百分点。全部 39 个模型—任务组合中，都能找到更小且表现更好的数据配置。

### Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models
*微软亚洲研究院 · Brain Project（Star Project）*

- 这项工作关注下游微调中的数据集干扰：哪些辅助数据能帮助目标任务，以及如何减少负迁移。
- 我们提出 POSE，根据目标适配期间 MMD 与 Fréchet 距离的水平和变化趋势选择、加权辅助数据，再通过 warm-up、joint-training 和 cool-down 控制辅助数据的参与。
- 在 12 个数据集上评估后，11 项分类任务的平均 balanced accuracy 从 54.5% 提升至 56.0%（LaBraM），从 52.8% 提升至 55.0%（CBraMod）；两个模型分别在 10 项和 9 项目标任务上优于仅用目标数据微调。

### 跨场景与多模态情感识别
*BCMI，上海交通大学*

- DDCT 关注从视频到游戏场景的 EEG 情感识别迁移，相关工作发表于 ICASSP 2025。
- M4Lego 则结合 EEG 与眼动信号，通过 multi-level masking 和 Lego-style block 建模游戏过程中的多模态情感。

科研经历
======
- **2025.04--至今：** Research Intern，[Microsoft Research Asia (MSRA)](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/) Shanghai AI/ML Group，Brain Project（Star Project）；**Top 5% Intern**。导师：[Yansen Wang](https://www.microsoft.com/en-us/research/people/yansenwang/)。
- **2023.06--2026.06：** Research Assistant，上海交通大学[仿脑计算与机器智能研究中心（BCMI）](https://bcmi.sjtu.edu.cn/)。导师：[郑伟龙教授](https://weilongzheng.github.io/)。

[English CV (PDF)](/files/Jun-Yu_Pan_CV.pdf)
