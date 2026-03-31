# 研究笔记索引

> 最后更新: 2026-03-31

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
│   │   ├── 2026-03-25.md
│   │   ├── 2026-03-26.md
│   │   ├── 2026-03-27.md
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
    ├── 2026-03-19-research-directions-v2.md
    └── 2026-03-26-paper-analysis.md
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

### 2026-03-24 | 研究方向分析 (第9次迭代)
- 类型: 方向规划
- 内容: ICLR 2026全景分析(164篇VLA投稿)、ICRA 2026 VLA Workshop机会、CT介入升为最高优先级、医疗VLA领域空白发现

### 2026-03-25 | 论文深度分析 + GTC 2026
- 类型: 论文精读 + 产业动态
- 内容: GSMem(3DGS空间记忆)、Sim2Real生成式3D世界、Motion-MLLM自我运动感知、VITA零样本价值函数、Safe RL GP可证明安全、Complementary RL经验协同进化、NVIDIA GTC 2026重大发布(GROOT N2 World Action Model、Isaac Lab 3.0+Newton 1.0、Cosmos 3物理世界生成、IGX Thor医疗边缘计算)

### 2026-03-26 | 论文深度分析
- 类型: 论文精读
- 内容: TwinRL-VLA数字孪生协同RL、Simulation Distillation仿真蒸馏、Interactive World Simulator交互式世界模拟器、DAM-VLA动态动作专家、AR-VLA自回归动作专家；核心结论是 digital twin 正在成为探索引擎、world model 正在成为研究基础设施、VLA 控制正在走向模块化

### 2026-03-27 | 论文深度分析 (上午)
- 类型: 论文精读
- 内容: Merlin(首个CT领域VLM基础模型)、MS-HGNN(E(3)等变GNN+形态对称性)、Gaze-Regularized VLA(注视引导注意力)、VLA综述(80+模型系统梳理)；关键发现：CT影像领域正在复制VLA成功路径，Gaze-VLA为共享控制提供新思路

### 2026-03-27 | 研究方向分析 (第9次迭代 - 下午)
- 类型: 方向规划
- 内容: CT介入机器人完整技术栈整合(感知层→决策层→执行层→安全层)、Brain-Cerebellum 2.0架构增强、CT-VLA机会窗口识别、下午行动清单(Isaac Lab 3.0搭建、GSMem复现、USCorUNet下载)

### 2026-03-25 | 研究方向分析 (第10次迭代)
- 类型: 方向规划
- 内容: CT介入升为最高优先级，完整技术栈(感知→决策→执行→安全)，可执行路线图(W1-W12)

### 2026-03-26 | 论文深度分析
- 类型: 论文精读
- 内容: TwinRL-VLA数字孪生协同RL、Simulation Distillation仿真蒸馏、Interactive World Simulator交互式世界模拟器、DAM-VLA动态动作专家、AR-VLA自回归动作专家；核心结论是 digital twin 正在成为探索引擎、world model 正在成为研究基础设施、VLA 控制正在走向模块化

### 2026-03-28 | 论文深度分析
- 类型: 论文精读
- 内容: VLA综述(80+模型)、EchoVLA(记忆增强移动操纵)、π0(流匹配通用控制)、SG-VLA(空间锚定)；核心趋势：记忆系统崛起、空间理解深化、效率优化加速

### 2026-03-29 | 论文深度分析
- 类型: 论文精读
- 内容: DualCoT-VLA(双通道思维链并行推理)、VLA-IAP(交互对齐无训练Token剪枝1.25-1.54×加速)、Gaze-Regularized(注视引导注意力)、Causal World Model(因果世界模型)、Simulation Distillation(仿真蒸馏)；核心趋势：推理效率成为焦点、多模态思维链崛起、人类先验整合

### 2026-03-31 | 论文深度分析
- 类型: 论文精读
- 内容: 近期VLA/医疗/数字孪生相关论文的延续分析

### 2026-03-31 | 研究方向分析 (第12次迭代 - 下午)
- 类型: 方向规划
- 内容: 从论文跟踪收束到可投稿主线，提出“CT介入机器人中的可解释共享控制 + Digital Twin failure-mode数据闭环 + Brain-Cerebellum分层架构”的统一故事线；明确P0/P1/P2优先级与最小实验切口

### 2026-03-26 | 每日论文候选
- 类型: 候选检索
- 内容: TwinRL-VLA数字孪生协同RL、Simulation Distillation世界模型蒸馏、Interactive World Simulator交互式仿真器、PlayWorld自玩世界模型、DAM-VLA动态动作专家、AR-VLA自回归动作专家、LiteVLA-Edge边缘部署、Kinema4D四维世界建模

---

## 研究方向摘要

### 核心方向（优先级更新）
1. **CT介入机器人 + VLA** ⭐⭐⭐⭐⭐ - 首个医疗场景VLA应用，ICLR 2026无竞品
2. **可解释VLA决策框架** ⭐⭐⭐⭐⭐ - Failure Mode诊断 + 安全约束
3. **数字孪生 + VLA** ⭐⭐⭐⭐ - 虚实融合训练框架
4. **Brain-Cerebellum架构** ⭐⭐⭐⭐ - StructVLA + FASTER实现

### 技术栈
- 模型: OpenVLA / π0 (OpenPI) / **GR00T N1.7** / **GR00T N2 (待发)**
- 数据: LeRobot / AMSim2Real / VLA-IT (650K) / **Cosmos 3合成数据** / **生成式3D世界**
- 平台: Isaac Sim / **Isaac Lab 3.0** / **Newton 1.0** / 真机LeRobot
- 空间表示: **GSMem (3DGS空间记忆)**
- 传感融合: **Motion-MLLM (IMU+视觉)**
- 新增: USCorUNet (CBCT+超声融合) / FASTER (实时推理) / **VITA (零样本价值函数)** / **Safe RL GP (可证明安全)** / **IGX Thor (边缘计算)**

---

## 待办事项

### 🔴 最高优先级 (本周)
- [ ] **安装Isaac Lab 3.0 + Newton 1.0** (GTC 2026新发布，仿真基础设施升级)
- [ ] **复现GSMem** (3DGS空间记忆对数字孪生+CT介入有直接价值) - 项目: vulab-ai.github.io/GSMem/
- [ ] **下载USCorUNet代码并复现CBCT+超声融合** (CT介入核心) - 代码: github.com/anonymous-codebase/us-cbct-demo
- [ ] **复现FASTER延迟测试** (实时性核心突破) - 项目: innovator-zero.github.io/FASTER
- [ ] **跟踪GR00T N2发布** (World Action Model架构值得关注)

### 🔴 高优先级
- [ ] **精读StructVLA两阶段训练** (Brain-Cerebellum架构实现)
- [ ] **精读VLANeXt 12条设计准则**
- [ ] **复现Feature Control实验（OpenVLA特征可观测性）**
- [ ] **评估ICRA 2026 VLA Workshop参与可行性** (截止: 4月15日)

### 🟡 中优先级
- [ ] 复现OpenVLA在DROID上的基线性能
- [ ] 用LeRobot跑100/200/500条数据消融
- [ ] 整理AMSim2Real数据收集清单
- [ ] 阅读π0.5多源数据协同细节
- [ ] 设计Failure Mode诊断方案
- [ ] 设计Critic架构（三系统框架）
- [ ] 评估RLT穿刺精度任务可行性
- [ ] 下载VLA-IT数据集 (650K)
- [ ] 精读DT→WM综述五大组件
- [ ] 设计AMSim2Real世界模型架构

### 研究方向更新 (2026-03-25 下午)
- **GSMem**: 3DGS作为持久空间记忆，后验可重观察性突破，对CT介入场景重建有直接价值
- **生成式3D世界**: 场景多样性 > 样本数量，Sim2Real成功率从9.7%→79.8%，完美匹配AMSim2Real
- **Motion-MLLM**: IMU作为新模态，低成本实现3D场景理解，与GSMem形成互补
- **VITA**: VLM零样本价值函数，Brain层任务进度监控，test-time adaptation动态适应
- **Safe RL GP**: 可证明安全边界，CT介入安全约束核心技术
- **Complementary RL**: 经验提取器+策略执行器协同进化，解决静态经验存储问题
- **GTC 2026**: NVIDIA全面押注Physical AI，从数据问题转向计算问题，GR00T N2 World Action Model架构值得关注
- **IGX Thor**: 医疗机器人边缘计算平台成熟，J&J和Medtronic已采用，CT介入硬件平台标准
- **Cosmos 3**: 物理世界生成模型，解决机器人数据稀缺问题，与生成式3D世界方法高度互补
- **战略转变**: 从"跟随热点"转向"填补空白"，医疗VLA领域完全空白
- **CT介入机器人**: 最高优先级，完整技术栈(感知→决策→执行→安全)，可执行路线图(W1-W12)
- **ICRA 2026**: VLA Workshop提供真实机器人评估平台，10,000+小时数据
- **ICLR 2026**: 164篇VLA投稿增长18倍，LIBERO已饱和(>95%)，离散扩散VLAs竞争激烈

---

*由 OpenClaw 自动维护*
