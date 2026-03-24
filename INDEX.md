# 研究笔记索引

> 最后更新: 2026-03-24

---

## 目录结构

```
research-notes/
├── README.md                 # 项目简介
├── INDEX.md                  # 本文件（索引）
├── papers/                   # 论文资料
│   ├── daily-candidates/     # 每日候选论文（按日期）
│   │   ├── 2026-03-19.md
│   │   ├── 2026-03-20.md
│   │   ├── 2026-03-24.md
│   │   └── ...
│   └── vla-robots/           # VLA论文笔记
│       ├── literature-log.md
│       ├── obsidian/         # Obsidian格式笔记
│       └── *.pdf             # PDF文件
└── analysis/                 # 分析报告
    ├── 2026-03-11-kamitsubaki-yunagi.md
    ├── 2026-03-14-research-directions.md
    ├── 2026-03-16-user-study.md
    ├── 2026-03-17-paper-analysis.md
    ├── 2026-03-18-vla-trends.md
    └── 2026-03-19-research-directions-v2.md
```

---

## 分析报告索引

### 2026-03-11 | 神椿工作室 & 夕凪機资料
- 类型: 角色背景调研
- 内容: OpenClaw角色原型（夕凪機）的详细资料

### 2026-03-14 | 研究方向分析 (第1次)
- 类型: 方向规划
- 内容: 基于文献库的缺陷分析，提出5个研究机会

### 2026-03-16 | User Study方法论
- 类型: 方法论笔记
- 内容: User Study的定义、类型、核心要素、常见坑

### 2026-03-17 | 论文深度分析
- 类型: 论文精读
- 内容: GR00T N1、π0、Embodied Digital Twin三篇论文分析

### 2026-03-18 | VLA研究趋势
- 类型: 趋势分析
- 内容: ICLR 2026趋势、VLA定义、关键发现

### 2026-03-19 | 研究方向分析 (第4次迭代)
- 类型: 方向规划
- 内容: 深化可行性评估，可执行路线图

### 2026-03-20 | 论文深度分析
- 类型: 论文精读
- 内容: ICLR 2026 VLA全景、HRC-CogiDT、DT+Embodied AI融合

### 2026-03-21 | 论文深度分析
- 类型: 论文精读
- 内容: SOP在线后训练、TIC-VLA延迟感知、Open X-Embodiment跨具身

### 2026-03-21 | 研究方向分析 (第6次迭代)
- 类型: 方向规划
- 内容: 纳入SOP/TIC-VLA，更新方法论

### 2026-03-22 | 论文深度分析
- 类型: 论文精读
- 内容: Digital Twin HRC、Embodied AI Healthcare、VLA综述

### 2026-03-22 | 研究方向分析 (第7次迭代)
- 类型: 方向规划
- 内容: 新增ICLR 2026论文参考，Brain-Cerebellum架构

### 2026-03-23 | 论文深度分析
- 类型: 论文精读
- 内容: DySL-VLA动态跳层、VLANeXt设计准则、Critic-in-the-Loop三系统架构、Feature Control可解释性、InstructVLA指令微调、LiLo-VLA长时程、RL Tokens精确控制

### 2026-03-23 | 研究方向分析 (第8次迭代)
- 类型: 方向规划
- 内容: Feature Control突破性发现，可解释性方向优先级提升，CT介入纳入RLT+Critic架构

### 2026-03-24 | 论文深度分析
- 类型: 论文精读
- 内容: FASTER实时推理、StructVLA结构化规划、VLA-Thinker图像推理、CBCT+超声融合、DT→WM演进综述

---

## 研究方向摘要

### 核心方向
1. **CT介入机器人 + VLA** - 首个医疗场景VLA应用
2. **数字孪生 + VLA** - 虚实融合训练框架
3. **小数据VLA微调** - 100-200条数据方法论

### 技术栈
- 模型: OpenVLA / π0 (OpenPI)
- 数据: LeRobot / AMSim2Real
- 平台: Isaac Sim / 真机LeRobot

---

## 待办事项

### 高优先级 (本周)
- [ ] **下载USCorUNet代码并复现CBCT+超声融合** (CT介入核心)
- [ ] **复现FASTER延迟测试** (实时性核心突破)
- [ ] **精读StructVLA两阶段训练** (Brain-Cerebellum架构实现)
- [ ] **设计CT介入模拟场景** (Isaac Sim环境)
- [ ] **精读VLANeXt 12条设计准则**
- [ ] **复现Feature Control实验（OpenVLA特征可观测性）**

### 中优先级
- [ ] 复现OpenVLA在DROID上的基线性能
- [ ] 用LeRobot跑100/200/500条数据消融
- [ ] 整理AMSim2Real数据收集清单
- [ ] 阅读π0.5多源数据协同细节
- [ ] 阅读MoLe-VLA STAR Router实现
- [ ] 设计Failure Mode诊断方案
- [ ] 设计Critic架构（三系统框架）
- [ ] 评估RLT穿刺精度任务可行性
- [ ] 下载VLA-IT数据集
- [ ] 精读DT→WM综述五大组件
- [ ] 设计AMSim2Real世界模型架构
- [ ] 评估VLA-Thinker图像思考机制

### 研究方向更新 (2026-03-24)
- **CT介入机器人**: 融合FASTER实时推理 + CBCT超声融合 + RLT精确控制
- **Brain-Cerebellum架构**: StructVLA里程碑规划 + FASTER实时执行 + USCorUNet动态监控
- **数字孪生演进**: DT→WM范式转变，五大组件方法论

---

*由 OpenClaw 自动维护*
