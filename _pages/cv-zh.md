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
  研究 EEG 基础模型与 EEG-MLLM 对齐，涵盖大规模预训练、模型扩展、多尺度预测学习、数据选择、多数据集微调和生成式视觉对齐。完成四篇 ICLR 2027 投稿（其中三篇为第一作者）及一篇共同一作 CHI 2027 投稿。

- **上海交通大学仿脑计算与机器智能研究中心（BCMI）**，Research Assistant<br>
  2023 年 6 月--2026 年 6 月 | 导师：郑伟龙副教授<br>
  研究基于 EEG 的情感计算，包括跨场景、对比学习和多模态情感识别。

项目
======
*微软亚洲研究院 | Brain Project（Star Project）*

- **Large-Scale Pretraining and Model Scaling for EEG Foundation Models**
  - 研究大规模 EEG 预训练中数据量与模型容量对跨任务迁移性能的影响，探索数据与模型的有效扩展方式。
  - 独立负责数据整理、质量控制、预训练与评测全流程，将语料扩展至 515 个来源、约 8 万小时窗口化 EEG，构建编码器参数量覆盖 5.8M 至 1.97B 的系列模型。
  - 在 23 项任务上，49k Large 的全参数微调与线性探测平均 balanced accuracy 分别为 59.05% 和 54.09%，两种设置下的平均任务排名均为 12 个本地参评 checkpoint 中的第 1。

- **From Static Descriptions to State Dynamics: Multi-Scale Pretraining for EEG Transfer**
  - 研究如何通过预测不同时间尺度的未来状态，学习 EEG 瞬态事件与持续节律的动态变化，提升跨任务迁移能力。
  - 提出 MSDE，以因果编码器和时间间隔条件化的共享转移算子，从同一 EEG 状态联合预测微观与宏观尺度的未来教师状态。
  - MSDE-Full 与 MSDE-10% 在 20 项 OmniEEG-Bench 任务中取得八个模型中的前两位平均排名；后者仅用 5.0M 参数编码器和 2,115 小时 EEG 预训练。

- **Think It Your Way: Toward Strategy-Open Brain&ndash;Computer Interaction**
  - 研究当用户不受预设 mental mapping 限制、自主形成交互策略时，EEG 是否仍能支持对任务目标的稳定解码。
  - 对 26 名受试者开展连续三车道 parkour 任务的离线研究，联合分析 EEG、自报告与模态相关生理特征，并跨视觉主题解码 movement direction 和 target lane。
  - 发现用户策略高度异质且调整集中在交互早期；主观报告与生理特征部分一致，同时两类任务表征在不同策略下仍可解码。

- **Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs**
  - 研究如何利用 MLLM 提升 EEG 的理解与生成能力。
  - 提出 GVG，利用 EEG-to-image 生成器构建样本级代理图像，通过原生视觉 token 预测及 EEG—图像—文本三模态对齐复用 MLLM 的视觉先验。
  - GVG-Janus 在六项任务上的平均 balanced accuracy 从文本对齐的 45.89% 提升至图像对齐的 53.46%；三模态对齐结合全参数适配达到 60.05%。

- **Which Data, Not How Much: Architecture-Dependent Data Selection for EEG Foundation Models**
  - 研究基础脑电大模型预训练中的数据集干扰，以及数据来源组合、规模和模型架构对迁移性能的影响。
  - 在 LaBraM、CBraMod 和 BIOT 上评估 202 组配置，覆盖 16 个候选数据集与 13 个下游任务，比较 Progressive、PDV、Size 和 Coverage 四种数据排序方法。
  - 121 组配置以更少训练窗口优于全量预训练，最佳子集平均 balanced accuracy 最高提升 5.58 个百分点；数据来源的效用随模型架构而变化。

- **Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models**
  - 研究基础脑电大模型下游微调过程中的数据集干扰问题。
  - 提出 POSE，依据目标适配期间 MMD 与 Fréchet 距离的水平和变化趋势选择、加权辅助数据集，再分阶段引入与减少辅助训练。
  - 在 12 个数据集上评估，11 项分类任务的平均 balanced accuracy 较仅用目标数据微调提升 1.5（LaBraM）和 2.2（CBraMod）个百分点。

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
1. **Jun-Yu Pan**, Ruicheng Yin, Yansen Wang, Bao-Liang Lu, Dongsheng Li, and Wei-Long Zheng. "From Static Descriptions to State Dynamics: Multi-Scale Pretraining for EEG Transfer." *International Conference on Learning Representations (ICLR 2027)*, under review.
2. Xin Xu<sup>&dagger;</sup>, <strong>Jun-Yu Pan</strong><sup>&dagger;</sup>, Ruicheng Yin, Zilong Wang, Dongqi Han, Dongsheng Li, Bao-Liang Lu, Wei-Long Zheng, and Yansen Wang. "Think It Your Way: Toward Strategy-Open Brain&ndash;Computer Interaction." *ACM CHI Conference on Human Factors in Computing Systems (CHI 2027)*, under review.
3. **Jun-Yu Pan**, Enze Zhang, Bao-Liang Lu, Wei-Long Zheng, Dongsheng Li, and Yansen Wang. ["Visualizing the Invisible: Generative Visual Grounding Empowers Universal EEG Understanding in MLLMs."](https://arxiv.org/abs/2605.18172) *International Conference on Learning Representations (ICLR 2027)*, under review.
4. **Jun-Yu Pan**, Ruicheng Yin, Bao-Liang Lu, Wei-Long Zheng, Dongsheng Li, and Yansen Wang. "Which Data, Not How Much: Architecture-Dependent Data Selection for EEG Foundation Models." *International Conference on Learning Representations (ICLR 2027)*, under review.
5. Ruicheng Yin, **Jun-Yu Pan**, Yansen Wang, Xiaoqing Zheng, and Dongsheng Li. "Discern, Then Combine: Probe-Guided Multi-Dataset Fine-Tuning for EEG Foundation Models." *International Conference on Learning Representations (ICLR 2027)*, under review.
6. <strong>Jun-Yu Pan</strong><sup>&dagger;</sup>, Jing-Yi Liu<sup>&dagger;</sup>, Bao-Liang Lu, and Wei-Long Zheng. "M4Lego: A Multi-Modal Pretraining Framework with Multi-Level Masking and Lego Blocks for Emotion Recognition During Gameplay." *IEEE Transactions on Affective Computing*, under review.
7. **Jun-Yu Pan**, Hao-Long Yin, and Wei-Long Zheng. ["Double Domain Converter Transformer for Improving EEG-Based Emotion Recognition from Video to Game Scenarios."](https://ieeexplore.ieee.org/document/10889052) *ICASSP 2025*.

&dagger; 共同一作。

技术能力
======
- **编程语言：** Python、C
- **机器学习框架：** PyTorch
- **语言：** 中文、英语、法语
