# 研究笔记索引

> 最后更新: 2026-03-21

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

- [ ] 复现OpenVLA在DROID上的基线性能
- [ ] 用LeRobot跑100/200/500条数据消融
- [ ] 整理AMSim2Real数据收集清单
- [ ] 阅读π0.5多源数据协同细节
- [ ] 阅读MoLe-VLA STAR Router实现

---

*由 OpenClaw 自动维护*
