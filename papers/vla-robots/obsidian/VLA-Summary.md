---
title: VLA 论文关系图谱
tags: [summary, VLA, robot-learning]
---

# VLA 论文关系图谱

## 论文列表

| 论文 | 年份 | 核心方向 | 分析类型 |
|------|------|----------|----------|
| [[RT-2]] | 2023 | VLA 开创性工作 | 大致 |
| [[OpenVLA]] | 2024 | 开源 VLA + 微调 | 大致 |
| [[Fine-tuning VLA]] | 2025 | VLA 微调优化 | 大致 |
| [[π0]] | 2024 | Flow Matching VLA | 大致 |
| [[π0.5]] | 2025 | VLA 开放世界泛化 | **精细** |
| [[MoLe-VLA]] | 2025 | 高效动态VLA | **精细** |
| [[Embodied-Robot-Manipulation]] | 2025 | 基础模型综述 | **精细** |
| [[DexVLA]] | 2025 | 灵巧手+共享控制 | 大致 |

## 发展脉络

```
RT-2 (2023) → OpenVLA (2024) → π0 (2024) → π0.5 (2025)
                        ↘︎
                    MoLe-VLA (2025) - 高效变体
```

## 核心关系

### RT-2 → OpenVLA
- OpenVLA 是 RT-2 的开源复现
- 同样基于视觉语言模型
- 改进了训练数据和模型架构

### OpenVLA → Fine-tuning VLA
- 同一作者团队
- Fine-tuning 深入研究如何高效微调 OpenVLA
- 平衡速度与成功率

## 研究方向归类

### 基础模型
- RT-2: 证明 VLA 可行
- OpenVLA: 开源基础设施

### 训练/微调
- Fine-tuning VLA: 如何高效微调

### 你的研究关联
- [[DexVLA]] - 灵巧手 + 共享控制
- 可结合数字孪生做 Sim2Real

## 待补充
- π0 相关论文
- 其他 VLA 最新工作
