# 2026-03-28 研究方向分析 (第10次迭代 - 下午)

> 日期: 2026-03-28 下午
> 分析者: Yunagi
> 主题: CT介入VLA技术路径深化 + ICRA 2026投稿窗口评估

---

## 摘要

基于上午论文分析（EchoVLA、π0、SG-VLA），本分析聚焦CT介入机器人VLA化的具体技术路径。同时评估ICRA 2026 VLA Workshop投稿机会，结合研究路线图的可执行性。

---

## 1. CT介入VLA技术路径: 从上午论文到具体架构

### 1.1 记忆增强系统 → 手术记忆模块

上午分析的EchoVLA为CT介入提供了直接的架构借鉴：

| EchoVLA组件 | CT介入映射 |
|------------|------------|
| Scene Memory | CT三维重建 + 术前规划图 |
| Episodic Memory | 手术步骤历史 + 风险事件 |
| 协同检索 | 术前/术中状态匹配 |

**手术记忆模块设计**:
```
┌────────────────────────────────────────────────────┐
│              手术记忆模块 (Surgical Memory)         │
├────────────────────────────────────────────────────┤
│  术前: CT分割 → 血管/神经标注 → 安全走廊规划       │
│    ↓                                               │
│  术中: 实时超声匹配 → 针尖追踪 → 偏差补偿           │
│    ↓                                               │
│  术后: 恢复轨迹 → 并发症记录 → 经验知识库           │
└────────────────────────────────────────────────────┘
```

### 1.2 空间锚定辅助任务 → 穿刺精度增强

SG-VLA的辅助任务训练范式可直接迁移：

| SG-VLA辅助任务 | CT介入对应任务 |
|---------------|----------------|
| 全局位置重建 | 患者体表坐标 → 体内靶点映射 |
| 关节配置重建 | 机械臂关节 → 针尖位姿 |
| 抓取affordance | 穿刺位点选择 + 进针角度 |
| 目标相对姿态 | 针尖 → 靶点相对姿态预测 |

**CT介入辅助任务设计**:
```python
# 辅助任务 1: 3D空间坐标回归
def aux_task_3d_localization(ct_slice, target_voxel):
    features = vla_encoder(ct_slice)
    pred_voxel = mlp_coord(features)  # 回归3D坐标
    
# 辅助任务 2: 穿刺角度回归  
def aux_task_needle_angle(ct_slice, insertion_point):
    features = vla_encoder(ct_slice)
    pred_angle = mlp_angle(features)  # 回归进针角度
    
# 辅助任务 3: 风险区域分割
def aux_task_risk_segmentation(ct_slice):
    features = vla_encoder(ct_slice)
    risk_mask = segmentation_head(features)  # 血管/神经分割
```

### 1.3 流匹配 → 高频穿刺控制

π0的流匹配架构适合CT介入的高频控制需求：
- 50Hz连续轨迹输出 → 实时针尖轨迹
- 流匹配收敛快 → 少样本微调
- 多平台泛化 → 不同穿刺机器人适配

---

## 2. ICRA 2026 VLA Workshop 评估

### 2.1 重要信息
- **截止日期**: 2026年4月15日
- **Workshop名称**: VLA for Real-World Robot Learning
- **数据平台**: 10,000+小时真实机器人数据
- **核心要求**: 真实机器人评估

### 2.2 投稿可行性分析

| 维度 | 当前状态 | 差距 | 优先级 |
|------|---------|------|--------|
| **核心算法** | Brain-Cerebellum 2.0 框架设计 | 需要具体实现 | 🔴 高 |
| **实验平台** | Isaac Lab 3.0 搭建中 | 需1-2周 | 🔴 高 |
| **数据集** | AMSim2Real 初步设计 | 需扩展 | 🟡 中 |
| **真实机器人** | LeRobot 初步探索 | 需对接CT机器人 | 🔴 高 |
| **论文撰写** | 未开始 | 需2-3周 | 🟡 中 |

### 2.3 备选方案: Abstract Submission
- Workshop接受Abstract-only投稿
- 可以先提交初步想法，获得反馈后再完善
- 建议: 3月底前提交Abstract，4月中完善Full Paper

---

## 3. 技术路线图更新 (W1-W12)

### 3.1 本周重点 (W1: 03/24-03/30)

| 任务 | 状态 | 负责人 | 备注 |
|------|------|--------|------|
| Isaac Lab 3.0 安装 | ⏳ 待开始 | Yunagi | GTC 2026新发布 |
| GSMem 复现 | ⏳ 待开始 | Yunagi | 3DGS空间记忆 |
| USCorUNet 下载 | ⏳ 待开始 | Yunagi | CBCT+超声融合 |
| FASTER 复现 | ⏳ 待开始 | Yunagi | 实时推理测试 |

### 3.2 两周目标 (W2: 03/31-04/06)

- [ ] Isaac Lab 3.0 + Newton 1.0 环境跑通
- [ ] GSMem 在AMSim2Real场景复现
- [ ] USCorUNet 超声-CBCT配准初步
- [ ] **ICRA 2026 Abstract 撰写**

### 3.3 一个月目标 (W3-W4: 04/07-04/20)

- [ ] CT-VLA 核心模块设计完成
- [ ] 辅助任务训练pipeline搭建
- [ ] ICRA 2026 Full Paper 提交
- [ ] LeRobot 真实机器人数据采集设计

---

## 4. 风险与挑战

### 4.1 技术风险

| 风险 | 概率 | 影响 | 缓解措施 |
|------|------|------|----------|
| CT数据获取困难 | 中 | 高 | 使用公开数据集(RIDER, LIDC) |
| 实时性不足 | 中 | 高 | 参考FASTER轻量化方案 |
| 安全验证复杂 | 高 | 高 | 分阶段验证(仿真→离体→临床) |

### 4.2 时间风险

- ICRA 2026截止前仅剩18天
- 需要快速产出初步结果
- 建议: Abstract优先，Full Paper迭代

---

## 5. 下一步行动

### 今日行动 (03/28)
- [ ] 安装 Isaac Lab 3.0 (预计1-2小时)
- [ ] 下载 GSMem 代码和模型
- [ ] 调研 CT 公开数据集 (RIDER, LIDC, NSCLC)

### 明日行动 (03/29)
- [ ] 搭建 Isaac Lab 3.0 + Newton 1.0 环境
- [ ] 跑通 GSMem Demo
- [ ] 开始 ICRA 2026 Abstract 撰写

### 本周行动 (03/24-03/30)
- [ ] 确认 CT 机器人硬件平台
- [ ] 设计 Brain-Cerebellum 2.0 架构
- [ ] 提交 ICRA 2026 Abstract

---

## 6. 结论

**核心结论**:
1. CT介入VLA技术路径清晰: 记忆模块 + 辅助任务 + 流匹配控制
2. ICRA 2026是重要时间节点，Abstract提交是务实选择
3. 本周重点是环境搭建和数据集调研

**夕凪機最強!!!** 🫧

---

## 参考资料

1. EchoVLA (arXiv:2511.18112) - 记忆增强VLA
2. π0 (arXiv:2410.24164) - 流匹配控制
3. SG-VLA (arXiv:2603.22760) - 空间锚定
4. Merlin (arXiv:2406.06512) - CT VLM基础模型
5. ICRA 2026 VLA Workshop - 截止4月15日
