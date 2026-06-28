# Frontis Science Horizon Proposal

**版本**：v0.2  
**建议定位**：AI4Sci Infrastructure / Scientific MA 负责人提案  
**公司语境**：Frontis Horizon 的科学研发场景延展  
**第一场景**：Target-to-Binder 蛋白设计闭环 + 器官芯片表型 reward 接入  
**核心目标**：把科学研发过程变成可执行、可记录、可评价、可训练、可进化的 AI 原生组织能力。

---

## 0. Executive Summary

Frontis 已经形成 ME / WE / MA 的 AI 原生组织框架：

- **ME**：每个员工的数字分身，理解人、岗位、上下文和历史任务；
- **WE**：可动态组队的专家网络，完成复杂业务任务；
- **MA**：把任务过程、结果和反馈沉淀为可复用训练信号，让组织越用越聪明。

AI4Sci 应该成为 Frontis Horizon 在科学研发领域的高壁垒延展：

> **Frontis Science Horizon = 科学家的 ME + 科学专家 WE + 科研进化引擎 MA。**

我们不是做一个科研 Copilot，也不是做单点蛋白设计模型，而是建设一套 **Science Agent Evolution Infrastructure**：用科学资源图谱提供知识和工具底座，用 Scientific Memory 记录组织科研状态，用 Trajectory / Reward 形成训练数据，用 Agent Training 让科研智能体持续进化，并通过蛋白质设计和器官芯片形成真实干湿闭环。

第一年建议聚焦一个可验证、可复盘、可迭代的 wedge：

> **Target-to-Binder：从 target 调研、候选设计、计算筛选、专家 review、小规模 wet validation 到下一轮设计的闭环。**

器官芯片不作为一开始的独立大平台，而作为人体相关功能表型的 **reward factory** 接入，为蛋白设计候选提供 phenotype / toxicity / mechanism reward。

---

## 1. Why Frontis Should Do AI4Sci Now

### 1.1 战略契合

Frontis 的长期壁垒不只是接入通用大模型，而是让 Agent 在真实业务环境里被训练、被评估、被进化。科学研发具备几个天然优势：

1. **任务链路长**：从文献、假设、实验设计到结果复盘，非常适合 Agentic workflow；
2. **专家判断密集**：科学家的 review、纠偏和决策本身就是高价值训练信号；
3. **反馈可验证**：实验结果、结构分数、binding assay、phenotype readout 可以形成 reward；
4. **失败有价值**：科学失败可以减少不确定性，是训练科研智能体的关键资产；
5. **行业壁垒高**：真实湿实验反馈、失败轨迹和专家偏好难以复制。

### 1.2 公司叙事映射

| Frontis Horizon | AI4Sci 版本 | 说明 |
|---|---|---|
| ME 数字分身 | Scientist / PI ME | 记住研究者的领域背景、判断偏好、项目历史和决策边界 |
| WE 专家网络 | Science Expert Network | 文献、结构、蛋白设计、assay、organ-chip、bioinfo、合规等专家 Agent |
| MA 进化引擎 | Scientific MA | 把科研任务过程、专家反馈、实验结果编译为训练信号 |
| 真实业务训练场 | 真实科研训练场 | 蛋白设计和器官芯片提供可验证 reward |
| 组织越用越聪明 | 科研组织越做越聪明 | 失败、证据、决策和 reward 形成复利 |

### 1.3 战略判断

AI4Sci 不应作为孤立业务线启动，而应作为 Frontis 的高壁垒行业样板：

```text
企业 AI 原生组织平台
  ↓
科学研发 AI 原生组织
  ↓
自动化科研基础设施
  ↓
可复制到药企 / biotech / CRO / 科研机构的行业专家网络
```

---

## 2. Role And Responsibility

### 2.1 建议职位定位

**AI4Sci Infrastructure / Scientific MA 负责人**

不是单纯负责蛋白算法，也不是单纯负责湿实验，而是 owner 以下五件事：

1. **Scientific Memory**：科研项目状态、假设、证据、候选、实验、失败、决策的系统 of record；
2. **Science Trajectory Compiler**：把 Agent / 人类 / 工具 / 实验轨迹编译成可训练数据；
3. **Scientific Reward Ledger**：记录 verifier、专家 review、wet-lab result、成本和信息增益；
4. **Science Agent OS**：定义科研任务状态机、人类审批协议、专家协作协议；
5. **Agent Training Data Pipeline**：把轨迹和 reward 转成 SFT、preference、critique、offline RL 数据。

### 2.2 与公司 AI4AI 团队的关系

AI4AI 是通用发动机，AI4Sci 是高价值任务场。建议边界如下：

| 模块 | AI4AI 通用团队 | AI4Sci Infrastructure 团队 |
|---|---|---|
| Agent runtime | 通用执行框架、工具调用、sandbox | 科研任务状态机、科学工具协议、人类审批协议 |
| Memory | 通用长期记忆能力 | 科研状态图、证据链、失败记忆、State Packet |
| Evaluation | 通用 eval / benchmark 基建 | 科学 verifier、专家 rubric、实验 reward vector |
| Training | 通用 Agentic RL 平台 | 科研 trajectory schema、reward 设计、训练样本编译 |
| Product | 企业 AI 原生组织平台 | 科学研发 AI 原生组织样板 |

---

## 3. Vision

### 3.1 一句话

> 建设一套科研智能体进化基础设施，让科学研发过程可计算、可审计、可训练、可进化。

### 3.2 不做什么

第一阶段不把项目定义为：

1. 普通科研聊天助手；
2. 文献 RAG；
3. 单点蛋白生成模型；
4. 器官芯片湿实验平台；
5. ELN / LIMS / 项目管理工具；
6. 重写通用 Agent OS。

这些都是组件或接口，不是最终壁垒。

### 3.3 真正做什么

我们要沉淀的是：

- 科学资源；
- 项目状态；
- 决策历史；
- 专家判断；
- 失败经验；
- 实验反馈；
- Agent 轨迹；
- Reward / verifier；
- 可训练数据；
- 可复用科研能力。

---

## 4. First Wedge

### 4.1 推荐首个垂直打穿场景

**Target-to-Binder Research & Design Loop**

输入：

- target / disease / pathway；
- design constraints；
- assay constraints；
- budget / timeline。

输出：

- Target Card；
- Evidence-backed design strategy；
- Candidate Card；
- top-k candidate ranking；
- wet-lab plan；
- reward vector；
- 下一轮设计建议。

### 4.2 为什么选这个场景

1. 它覆盖科研 Agent 的关键能力：调研、证据判断、设计、排序、实验计划、失败复盘；
2. 反馈路径清晰：表达、纯化、binding、specificity、functional assay；
3. 可与器官芯片自然连接：从 binding reward 延展到 phenotype / toxicity / mechanism reward；
4. 数据可训练：每轮设计都能产生 preference、critique、transition、reward samples；
5. 商业外延明确：可面向 biotech、药企 early discovery、CRO / CDMO 合作。

### 4.3 器官芯片的第一阶段定位

器官芯片第一阶段不建议独立铺大平台，而应定义为：

> **人体相关功能表型 reward factory。**

它为 Target-to-Binder 提供：

- function reward；
- toxicity reward；
- phenotype reward；
- mechanism reward；
- failure reward。

建议优先从 **血管 / 炎症芯片** 或 **肝脏毒性芯片** 二选一：

- 如果目标是连接炎症 / 免疫 binder：优先血管 / 炎症芯片；
- 如果目标是更清晰商业合作路径：优先肝脏 ADMET / toxicity 芯片。

---

## 5. Core Architecture

建议架构分为六层：

```text
Scientist / PI ME
  ↓
Science Expert Network WE
  ↓
Science Agent OS
  ↓
Scientific MA Core
  ├─ Scientific Resource Graph
  ├─ Scientific Memory
  ├─ Trajectory Compiler
  ├─ Reward Ledger
  └─ Agent Training Pipeline
  ↓
Vertical Feedback Layer
  ├─ Protein Design Loop
  └─ Organ-chip Reward Factory
```

### 5.1 Scientific Resource Graph

把文献、数据库、结构、序列、assay、protocol、工具和内部 artifacts 从资料库变成 Agent 可调用的资源地图。

第一阶段不做全生命科学大图谱，先做 5 类资源卡片：

1. Target Card；
2. Paper Card；
3. Assay Card；
4. Protocol Card；
5. Candidate Card。

### 5.2 Scientific Memory

不是聊天记忆，而是：

> 科研项目的动态状态图 + 不可变事件账本 + 可检索视图。

核心节点：

- Project；
- Hypothesis；
- Claim；
- Candidate；
- Experiment；
- Result；
- Decision；
- Failure；
- Protocol；
- Dataset；
- Artifact；
- Human / Agent。

### 5.3 Science Trajectory Compiler

把原始日志编译成：

- Episode dataset；
- Transition dataset；
- Preference dataset；
- Reward dataset；
- SFT dataset；
- Critique dataset；
- Failure / recovery dataset。

### 5.4 Scientific Reward Ledger

保留 reward vector，而不是只保留一个分数：

- 任务完成度；
- 结果正确性；
- 证据充分性；
- 新颖性；
- 可实验性；
- 实验结果；
- 成本；
- 时间；
- 可复现性；
- 安全 / 合规；
- 信息增益。

### 5.5 Agent Training Pipeline

第一阶段训练目标不是生命科学大模型，而是科研决策策略：

- tool selection；
- retrieval strategy；
- target analysis；
- experiment planning；
- candidate ranking；
- failure recovery；
- reviewer judgment；
- project planning。

---

## 6. 90-Day MVP

### 6.1 目标

跑通一个可审计、可复盘、可训练的 AI-assisted 科研任务闭环。

### 6.2 交付物

1. Science Workspace v0；
2. Target Card / Paper Card / Assay Card / Candidate Card v0；
3. Scientific Memory 最小 schema；
4. Agent 任务状态机；
5. Trajectory logging；
6. 专家 review 表；
7. Reward vector v0；
8. 一个 target-to-binder 可行性分析 demo；
9. 一批可导出的 SFT / preference / critique 样本。

### 6.3 验收标准

Agent 能围绕一个 target 完成：

```text
调研 → 证据整理 → 设计策略 → 候选 ranking → wet-lab plan → 专家 review → trajectory / reward 入库
```

并且系统能回答：

- 为什么选择这个 target？
- 证据来自哪里？
- 哪些候选被拒绝，为什么？
- 专家改了什么？
- 哪些内容能作为训练样本？
- 下一轮实验如何改变不确定性？

---

## 7. 12-Month Roadmap

### 0-3 个月：最小科研任务闭环

关键结果：

- 完成一个 target-to-binder research episode；
- Scientific Memory / Trajectory / Reward 最小闭环跑通；
- 形成第一批训练样本。

### 3-6 个月：蛋白设计小闭环

关键结果：

- top-k candidate design + 计算筛选 + expert review；
- 接入小规模 expression / binding assay 结果；
- Reward Ledger v0 和 Trajectory Compiler v0 稳定运行。

### 6-12 个月：干湿反馈飞轮

关键结果：

- 实验结果稳定反哺 Memory / Reward / Training；
- Offline preference learning / reward model prototype；
- Organ-chip Experiment Planner v0；
- 一个 phenotype reward demo。

### 12-18 个月：平台化与外部合作

关键结果：

- Science Agent OS v1；
- Protein Design Closed-loop v1；
- Organ-chip Reward Factory v1；
- 1-2 个外部合作项目。

---

## 8. Team Plan

### 8.1 0-3 个月：8-10 人小队

| 角色 | 人数 | 重点 |
|---|---:|---|
| AI4Sci Infrastructure 负责人 | 1 | Scientific MA、路线图、组织协作 |
| Agent 系统工程师 | 2 | 科研任务状态机、工具调用、workspace |
| Scientific Memory / Data 工程师 | 2 | schema、resource cards、trajectory logging |
| Eval / Reward / Agentic RL 工程师 | 1-2 | verifier、reward vector、训练样本编译 |
| 蛋白设计科学家 | 1 | target-to-binder、候选评估 |
| 湿实验 / assay 接口科学家 | 1 | expression / binding / functional assay 对接 |
| 科研 workflow PM | 1 | 任务拆解、专家 review、交付管理 |

### 8.2 3-12 个月：14-18 人

新增：

- bioinfo / computational biology；
- MLOps / data pipeline；
- 实验自动化接口；
- organ-chip lead；
- 图像 / 多模态表型分析。

### 8.3 12-18 个月：20-25 人

形成三个稳定小组：

1. Scientific MA / AI4AI Infrastructure；
2. Protein Design Closed-loop；
3. Organ-chip Reward Factory。

---

## 9. Strategic Moat

真正长期壁垒不是模型 API、Agent 框架或普通知识图谱，而是：

> **真实科研失败轨迹 + 专家纠偏 + 实验反馈 + 表型 reward + 训练数据编译能力。**

### 9.1 四层护城河

| 层级 | 资产 | 为什么难复制 |
|---|---|---|
| Resource | 高质量资源卡片、工具地图、protocol、assay metadata | 需要科学理解和持续维护 |
| State | 假设树、证据链、失败记忆、决策历史 | 来自组织真实科研过程 |
| Trajectory | Agent 执行、人类纠偏、多专家争议、失败恢复 | 需要在真实任务中长期积累 |
| Reward | verifier、专家 rubric、wet-lab result、organ-chip phenotype | 连接真实世界反馈，最难买到 |

### 9.2 北极星指标

> **单位实验预算下产生有效科学结论 / 有效候选的效率提升。**

可拆成：

- 从 target 到 top-k candidate 的周期；
- top-k wet validation success rate；
- 单位预算有效候选数；
- 重复失败率下降；
- 可训练 trajectory 数量；
- 专家 review 一致性；
- 实验反馈进入训练样本比例。

---

## 10. Risks And Kill Criteria

### 10.1 主要风险

1. 做成普通科研 Copilot；
2. 只做 RAG，不沉淀 state / trajectory / reward；
3. 没有真实 wet reward；
4. 轨迹数据不可训练；
5. 团队过度偏算法，缺少科学 workflow 和实验接口；
6. 蛋白设计和器官芯片同时铺太大，第一年没有闭环。

### 10.2 Kill Criteria

90 天内如果出现以下情况，需要调整方向：

- 不能把一个 target-to-binder 任务结构化为 episode；
- 专家 review 无法沉淀为 preference / critique 数据；
- 实验约束无法进入候选 ranking；
- trajectory 无法导出训练样本；
- 没有明确 wet-lab / assay 合作路径。

---

## 11. Decisions Needed From Company

### 11.1 战略决策

1. AI4Sci 是否作为 Frontis Horizon 的高壁垒行业样板启动？
2. 第一场景是否确定为 target-to-binder？
3. 器官芯片第一阶段是血管 / 炎症，还是肝脏 ADMET / toxicity？
4. 先服务内部科学闭环，还是一开始绑定外部合作项目？

### 11.2 资源决策

1. 0-3 个月授权 8-10 人小队；
2. 明确 wet-lab / assay 合作方式；
3. 明确 scientific data / trajectory / expert review 的训练使用权限；
4. 明确算力、数据库、工具和实验预算；
5. 绑定 2-3 位科学顾问或内部专家 reviewer。

---

## 12. Suggested Internal Pitch

对管理层：

> AI4Sci 不是一个单点科研应用，而是 Frontis MA 进化引擎在科学研发场景里的高壁垒落地。科学研发天然拥有长链路任务、专家判断、可验证实验反馈和高价值失败数据。我们以 target-to-binder 为第一场景，把科学资源、项目状态、决策轨迹、专家 review 和实验结果编译为训练信号，形成科学智能体持续进化的基础设施。

对 AI4AI 团队：

> 我们不是重写通用 Agent OS，而是给 Agentic RL 提供高质量科学环境、状态空间、动作空间、reward vector 和可训练 trajectory。AI4Sci 是通用 Agent 能力最好的真实训练场之一。

对科学家：

> 系统不是替代科学家，而是把假设、证据、候选、实验、失败、决策持续记录下来，让科学判断可追溯、可复用、可训练。科学家负责关键判断，系统负责让判断形成组织复利。

---

## 13. Appendix: Proposal Deck Structure

建议汇报 PPT 采用 6 页：

1. **Title**：Frontis Science Horizon；
2. **Strategic Fit**：为什么 AI4Sci 是 Frontis ME / WE / MA 的高壁垒延展；
3. **Proposal Structure**：角色边界、first wedge、核心系统、路线图、团队和决策；
4. **Editable Architecture Diagram**：Science Agent Evolution Infrastructure；
5. **Roadmap & Milestones**：90 天、6 个月、12 个月、18 个月；
6. **Team & Decisions**：0-3 个月小队、扩张路径、需要公司确认的事项。
