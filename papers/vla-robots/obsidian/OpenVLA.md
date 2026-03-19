---
title: OpenVLA
authors: Moo Jin Kim, Karl Pertsch, Siddharth Karamcheti, et al.
year: 2024
arXiv: 2406.09246
tags: [VLA, robot-learning, open-source]
---

# OpenVLA: An Open-Source Vision-Language-Action Model

## 核心贡献
- 7B 参数开源 VLA 模型
- 基于 Llama 2 + DINOv2 + SigLIP 视觉编码器
- 训练数据：97 万真实机器人演示
- 首次开源 VLA + 完整微调框架

## 关键结果
- 在 29 个任务上比 RT-2-X (55B) 高 16.5% 成功率
- 参数少 7 倍
- 微调效果优于 Diffusion Policy 20.4%
- 支持 LoRA 微调和量化

## 局限性
- 泛化能力仍有限
- 需要大量微调数据
- 推理速度有待优化

## 相关论文
- [[RT-2]] - 早期 VLA 工作
- [[Fine-tuning VLA]] - 本文的微调研究

## 可创新方向
- 轻量化微调
- 零样本泛化
- 结合数字孪生
