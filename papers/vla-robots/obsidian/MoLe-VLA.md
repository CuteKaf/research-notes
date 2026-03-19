---
title: MoLe-VLA
authors: Rongyu Zhang, Menghang Dong, Yuan Zhang, et al.
year: 2025
arXiv: 2503.20384
tags: [VLA, efficient, layer-skipping, Mixture-of-Experts]
---

# MoLe-VLA: Dynamic Layer-skipping Vision Language Action Model

## 0. 摘要翻译
多模态大语言模型(MLLMs)在理解复杂语言和视觉数据方面表现出色，使通用机器人系统能够解释指令并执行具身任务。然而，它们的实际部署受到大量计算和存储需求的阻碍。本文提出MoLe-VLA，通过动态层激活实现高效的机器人操作。

## 1. 方法动机
a) 驱动力：降低VLA的计算成本，实现实际部署
b) 现有痛点：
   - MLLM计算和存储需求大
   - 现有稀疏化方法忽视关键的后层语义信息
c) 研究假设：借鉴神经科学的浅脑假说和专家混合模型，每层作为专家动态激活

## 2. 方法设计 ⭐
a) Pipeline:
   1. 将LLM每层视为专家
   2. Spatial-Temporal Aware Router (STAR) 动态选择激活的层
   3. Cognition Self-Knowledge Distillation (CogKD) 补偿丢失的认知能力
   4. 输出动作序列

b) 关键模块：
   - STAR Router：基于机器人当前状态选择性激活层，模拟大脑不同信号通路
   - CogKD框架：利用认知特征增强任务理解和动作生成

## 3. 方法对比
| 方法 | 优点 | 缺点 |
|------|------|------|
| 传统VLA | 精度高 | 计算大 |
| Early Exit | 省计算 | 忽视后层语义 |
| **MoLe-VLA** | **精度+省计算** | **需训练Router** |

## 4. 实验表现
- RLBench模拟环境 + 真实机器人
- **8% 成功率提升**
- **计算成本降低 5.6倍**
- 10个任务平均成功率高

## 5. 学习与应用
- 可迁移：需要异构任务数据
- 对你的价值：高效VLA适合边缘部署

## 6. 总结
- 一句话：动态层跳过实现VLA效率与性能兼得
- 速记：每层专家→动态选择→认知蒸馏→省计算5.6倍

## 局限性与创新点
- 局限：Router训练复杂度
- 你的创新机会：结合你的数字孪生场景做轻量化部署
