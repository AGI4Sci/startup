# AI4Sci 基础设施与自动化科研平台方案计划

**版本**：v0.1  
**定位**：AI4Sci 基础设施负责人视角  
**目标场景**：AI4AI 底座 + 蛋白质设计 + 器官芯片闭环  
**核心目标**：建设面向未来科学研究的基础设施，使科研过程能够被 AI 执行、记录、评价、训练和持续进化。

---

## 0. 一句话概括

我们要建设的不是一个科研聊天机器人，也不是单点蛋白质设计模型，而是一套 **Science Agent Evolution Infrastructure**：

> 用通用 Agent 作为执行入口，用科学资源图谱作为知识与工具底座，用 Scientific Memory 记录组织科研状态，用 Trajectory / Reward 形成训练数据，用 Agent Training 实现科研智能体持续进化，并通过蛋白质设计和器官芯片形成真实干湿闭环。

最终目标是成为科学研究的基础设施：

```text
科研任务
  ↓
Science Agent 执行
  ↓
科学资源 / 工具调用
  ↓
科研状态更新
  ↓
轨迹与奖励沉淀
  ↓
模型与 Agent 策略训练
  ↓
更强的自动化科研系统
```

---

## 1. 战略定位

### 1.1 我们不做什么

不应把项目定义成以下几类单点能力：

1. 不是普通科研 Copilot；
2. 不是简单文献 RAG；
3. 不是再造一个 Codex / Claude Code；
4. 不是只做蛋白质生成模型；
5. 不是只做器官芯片湿实验平台；
6. 不是只做 ELN / LIMS / 项目管理工具。

这些能力都重要，但都不是最终壁垒。

### 1.2 我们真正要做什么

我们要做的是：

> **科研智能体的进化基础设施。**

它的核心不是一次性回答问题，而是让科研组织持续积累：

- 科学资源；
- 项目状态；
- 决策历史；
- 失败经验；
- 专家判断；
- 实验反馈；
- Agent 轨迹；
- 训练数据；
- Reward / verifier；
- 可复用科研能力。

### 1.3 总体定位

```text
AI4AI 是发动机：
  负责让 Agent 能执行、记忆、评价、训练、进化。

AI4Sci 是任务场：
  蛋白质设计和器官芯片提供真实科学任务、实验反馈和物理世界 reward。

Science Agent OS 是产品形态：
  让科研组织可以用 AI 管理、执行和优化真实科研项目。
```

---

## 2. 总体架构

建议将整个体系分为七层。

```text
Science Agent Evolution Infrastructure

1. Execution Layer
   通用 Agent + 科研协作协议 + 人类介入机制

2. Scientific Resource Graph
   文献、数据库、工具、协议、实验、仪器、结构、序列等科学资源语义层

3. Scientific Memory
   项目状态、假设、证据、候选、实验、失败、决策的动态状态图

4. Trajectory Layer
   Agent 执行、人类纠偏、多专家争议、工具调用、实验反馈轨迹

5. Evaluation / Reward Layer
   程序 verifier、证据 verifier、专家 reviewer、实验 reward、成本约束

6. Agent Training Layer
   SFT、Preference Learning、Reward Model、Offline RL、Online RL、Agentic RL

7. Vertical Feedback Layer
   蛋白质设计 + 器官芯片作为第一批真实闭环场景
```

更简洁地说：

```text
资源底座 → 科研记忆 → 轨迹数据 → 科研裁判 → Agent 训练 → 自动化科研闭环
```

---

## 3. AI4AI 核心模块

## 3.1 Execution Layer：Agent OS 与人类协作协议

### 核心判断

底层 Agent OS 不应从零重做。Codex、Claude Code、OpenAI Agent、Gemini、LangGraph、AutoGen、MCP 等通用 Agent 能力会越来越强。

我们真正需要专门设计的是：

> **Human-AI Scientific Collaboration Protocol。**

也就是科研组织中，人类专家、Agent、工具、实验平台如何协作。

### 需要解决的问题

1. 哪些任务 Agent 可以自主执行？
2. 哪些任务必须人类审批？
3. 哪些节点需要 PI / 实验负责人 / 数据科学家 / 安全负责人介入？
4. 人类修改如何结构化成训练数据？
5. 多个专家意见冲突时如何处理？
6. Agent 出错后如何回溯和复盘？
7. 哪些操作需要安全、合规、预算 gate？

### 设计原则

```text
底层 Agent 可替换；
上层科学状态、资源、轨迹、reward 不可替换。
```

因此 Execution Layer 的核心资产不是 Agent 框架，而是：

- 科研任务状态机；
- 人类审批协议；
- 专家反馈结构化；
- 风险分级；
- 任务复盘；
- 决策理由记录。

---

## 3.2 Scientific Resource Graph：科学资源图谱

### 定义

Scientific Resource Graph 是一个逻辑上的科学资源语义层，不一定一开始就用图数据库物理存储。

它的目标是把科学资源从“资料库”变成“可被 Agent 决策和调用的资源地图”。

### 资源范围

第一阶段围绕蛋白质设计和器官芯片，重点包括：

- 文献；
- PubMed / bioRxiv / arXiv 等论文资源；
- UniProt、PDB、AlphaFold DB 等蛋白资源；
- target、gene、protein、domain、structure；
- disease、pathway、cell type；
- known ligand / antibody / binder；
- assay、protocol、readout；
- organ-chip model；
- experiment result；
- tool result；
- internal project artifacts。

### 不建议一开始做什么

不建议一开始做：

```text
全生命科学大图谱
纯 RDF triple store
纯 Neo4j
纯向量 RAG
```

更好的方式是：

```text
Postgres as source of truth
+ pgvector / full-text search
+ object storage
+ task-specific cards
+ optional graph projection
```

### 推荐物理架构

| 层 | 存储内容 | 建议实现 |
|---|---|---|
| Raw Object Layer | PDF、PDB、FASTA、图像、仪器原始文件 | S3 / MinIO / OSS |
| Metadata Layer | paper、target、protein、assay、dataset、protocol | Postgres |
| Relation / Evidence Layer | entity-edge、claim-evidence、provenance | Postgres，后续可同步图数据库 |
| Search Layer | 文本 chunk、摘要、embedding、BM25 | pgvector / OpenSearch / Elasticsearch |
| Analytics Layer | 大规模实验结果、omics、轨迹日志 | Parquet / DuckDB / ClickHouse / Iceberg |

### 核心不是 triple，而是 Claim-Evidence-Provenance

普通知识图谱可能存：

```text
Protein A interacts_with Protein B
```

科研资源图谱必须存：

```text
Claim:
  Protein A interacts with Protein B.

Evidence:
  哪篇论文？
  哪个数据库？
  哪个实验？
  哪个工具预测？
  支持还是反驳？
  证据强度多少？
  谁确认过？
  是否仍然有效？
```

也就是，每一条科学关系都要带证据、来源、上下文和可信度。

### 第一阶段产品形态：资源卡片

不要一开始追求宏大图谱，先做 5 类资源卡片：

1. **Target Card**
   - target 是什么；
   - 有哪些结构；
   - 疾病关联是什么；
   - 已有药物 / 抗体 / binder；
   - 可做 assay；
   - 风险是什么。

2. **Paper Card**
   - 文章解决什么问题；
   - 使用什么方法；
   - 产生什么数据；
   - 支持哪些 claim；
   - 是否有代码 / 数据可复现。

3. **Assay Card**
   - 测什么；
   - 输入输出是什么；
   - 阳性 / 阴性对照；
   - 成本、周期、历史成功率。

4. **Protocol Card**
   - 关键步骤；
   - 关键条件；
   - 失败原因；
   - 可自动化程度。

5. **Candidate Card**
   - 候选序列 / 结构；
   - 生成理由；
   - 计算分数；
   - 实验验证结果；
   - 下一轮修改建议。

---

## 3.3 Scientific Memory：科研状态图

### 定义

Scientific Memory 不是聊天记忆，而是：

> **科研项目的动态状态图 + 不可变事件账本 + 可检索视图。**

它要回答的不是“我们聊过什么”，而是：

```text
我们现在相信什么？
为什么相信？
哪些假设还活着？
哪些结论被推翻？
哪些候选已经失败？
失败原因是什么？
下一步为什么这么做？
```

### 推荐架构

```text
Event Log：记录所有状态变化
        ↓
State Reducer：把事件转成当前状态
        ↓
Scientific State Graph：当前项目状态图
        ↓
Retrieval Views：给 Agent / 人类使用
```

### 核心状态节点

第一阶段建议包含：

```text
Project
Hypothesis
Claim
Candidate
Experiment
Result
Decision
Failure
Protocol
Dataset
Artifact
Human / Agent
```

其中最关键的是：

1. Hypothesis；
2. Claim；
3. Candidate；
4. Experiment / Result；
5. Decision；
6. Failure。

### 状态边

建议定义有语义的边，而不是简单 related_to：

```text
Hypothesis --supported_by--> Evidence
Hypothesis --refuted_by--> Result
Decision --based_on--> Claim
Decision --chooses--> Candidate
Experiment --tests--> Hypothesis
Experiment --uses--> Protocol
Experiment --produces--> Result
Result --updates--> Claim
Failure --caused_by--> Protocol / Candidate / Assay
Candidate --derived_from--> PreviousCandidate
Claim --supersedes--> OldClaim
Human / Agent --approved--> Decision
```

每条边需要记录：

```text
created_at
created_by
source_event_id
confidence
status
valid_from
valid_to
```

### 关键产品形态：State Packet

每次 Agent 工作前，不应该喂聊天历史，而应该喂结构化状态包。

例如 Protein Design State Packet：

```text
Target:
  IL-6R

Active hypothesis:
  blocking domain X may reduce inflammatory signaling

Known evidence:
  paper A, assay B, structure C

Rejected approaches:
  peptide scaffold family Y failed due to aggregation

Current candidates:
  P7, P9, P11

Open risks:
  off-target binding to homolog Z

Next decision:
  whether to send P9/P11 to expression
```

### Scientific Memory 的壁垒

它的核心壁垒是：

> **状态压缩。**

也就是把海量聊天、文献、代码、实验、会议纪要、失败记录，压缩成可信、可追溯、可更新的科研状态。

---

## 3.4 Trajectory Layer：科研轨迹数据

### 定义

Trajectory Data 不是普通日志，而是：

> **可训练的科研决策样本。**

每条关键轨迹都要回答：

```text
在什么状态下？
看到了什么信息？
有哪些可选动作？
选择了什么动作？
为什么选择？
结果如何？
reward 是什么？
下次应该如何改？
```

### 轨迹数据的五层视图

```text
Raw Event Log
  ↓
Episode View
  ↓
Transition View
  ↓
Preference View
  ↓
Training Sample View
```

### A. Raw Event Log

记录：

- Agent message；
- tool call；
- tool output；
- human comment；
- file change；
- experiment status；
- instrument result；
- review decision。

用途：审计、回放、追溯。

### B. Episode View

一个 episode 对应一次完整科研任务。

例如：

```text
给定 target，设计 20 个 binder 候选并推荐 top 5 进入实验。
```

### C. Transition View

这是最重要的 RL-ready 格式：

```text
s_t, a_t, o_t, r_t, s_{t+1}, done, metadata
```

其中 action 不建议用 token，而应使用科研宏动作：

```text
search_literature
retrieve_structure
generate_candidates
run_structure_prediction
rank_candidates
request_experiment
revise_hypothesis
reject_candidate
escalate_to_human
stop_direction
```

### D. Preference View

用于记录专家选择、候选排序、方案比较。

例如：

```text
实验设计 B > 实验设计 A，
因为 B 包含阳性对照，且能区分机制 A 和 B。
```

### E. Training Sample View

一条 episode 最终应编译成多种训练样本：

| 数据类型 | 用途 |
|---|---|
| SFT sample | 学习好轨迹、好工具调用、好报告 |
| Preference pair | 学习专家偏好、候选排序、方案选择 |
| Reward model sample | 学习估计 scientific value |
| Transition sample | 做 offline RL / actor-critic |
| Critique sample | 训练 reviewer / failure diagnosis |
| Recovery sample | 训练错误恢复和回溯 |

### 最关键原则

不要让 Agent 留下聊天记录，而要让它留下：

> **可训练的科研决策样本。**

---

## 3.5 Evaluation / Reward Layer：科研裁判系统

### 定义

科研 reward 不是一个 LLM judge，而应是多层级 scientific verifier system。

它的核心问题是：

```text
这个 Agent 的行动是否产生了可复现、可验证、对科学目标有增益的结果？
```

### Reward Vector

不要只存一个分数，要存 reward vector：

```text
Reward Vector =
  任务完成度
  结果正确性
  证据充分性
  新颖性
  可实验性
  实验结果
  成本
  时间
  可复现性
  安全 / 合规
  信息增益
```

训练时可以派生 scalar reward，但底层必须保留分项。

### 多层裁判

| 层级 | 裁判类型 | 例子 |
|---|---|---|
| L1 | 格式与任务完成 verifier | 是否输出指定文件、候选、报告 |
| L2 | 确定性 correctness verifier | 代码是否跑通、结构是否合法、指标是否达标 |
| L3 | 科学证据 verifier | claim 是否被文献 / 数据 / 工具结果支持 |
| L4 | 专家 rubric judge | 科学合理性、新颖性、可实验性 |
| L5 | 真实实验 reward | 表达、结合、功能、毒性、器官芯片表型 |

### Reward 哲学

科研 reward 不应只奖励成功，还要奖励 information gain。

```text
失败但能减少不确定性 = 有价值
失败且不可解释、不可复用 = 低价值
```

因此应奖励：

- 主动查 baseline；
- 发现关键负结果；
- 识别实验不可行性；
- 发现文献冲突；
- 及时停止低价值方向；
- 记录失败原因；
- 生成可复现实验配置。

惩罚：

- 编造引用；
- 跳过 baseline；
- 只优化单一 proxy score；
- 忽略实验约束；
- 不记录失败；
- 过度消耗预算；
- 给出不可证伪假设。

---

## 3.6 Agent Training Layer：智能体训练与优化

### 训练目标

不是一开始训练生命科学大模型，而是先训练科学决策策略。

优先训练：

- tool selection；
- retrieval strategy；
- target analysis；
- experiment planning；
- candidate ranking；
- failure recovery；
- reviewer judgment；
- project planning。

### 训练路线

#### 阶段 1：SFT on good trajectories

学习专家和高质量 Agent 的好轨迹：

- 如何拆任务；
- 如何查资源；
- 如何调用工具；
- 如何生成候选；
- 如何写实验计划；
- 如何总结证据。

#### 阶段 2：Preference Learning

用专家选择、候选排序、方案比较训练偏好模型。

例如：

```text
好实验设计 > 缺少对照的实验设计
成功候选 > 失败候选
正确失败诊断 > 空泛失败解释
```

#### 阶段 3：Reward Model / Verifier Model

训练模型预测：

- 设计是否值得实验；
- claim 是否被证据支持；
- assay 是否能验证假设；
- 候选是否高风险；
- failure diagnosis 是否可信。

#### 阶段 4：Offline RL

用历史 transition 数据优化：

- 工具选择；
- 检索策略；
- 候选筛选；
- 实验优先级；
- 失败恢复。

#### 阶段 5：Online RL / Active Learning Loop

在受控场景中，让 Agent 提出候选、选择实验、拿到结果、继续迭代。

---

## 4. AI4Sci 垂直闭环场景

## 4.1 蛋白质设计闭环

### 定位

蛋白质设计不是单独做一个生成模型，而是作为：

> **reward-guided protein design agent + wet validation loop。**

### 起步任务建议

优先选择：

```text
Target-specific binder / peptide / mini-protein design
```

不要一开始做过大的“通用蛋白设计”。

### 闭环流程

```text
Target selection
  ↓
Target Card 生成
  ↓
机制与结构证据分析
  ↓
候选生成
  ↓
结构预测 / developability / specificity 过滤
  ↓
候选排序
  ↓
小规模表达 / binding / function assay
  ↓
实验结果写入 Memory / Reward
  ↓
下一轮设计
```

### 蛋白设计 reward

计算侧：

- 结构合理性；
- interface confidence；
- developability；
- specificity；
- novelty；
- diversity。

实验侧：

- 表达成功；
- 纯化质量；
- binding KD / EC50；
- specificity；
- functional assay；
- toxicity / safety。

### 关键壁垒

1. 候选设计轨迹；
2. 失败候选与失败原因；
3. 实验结果与计算分数之间的映射；
4. 专家筛选偏好；
5. reward-guided search policy。

---

## 4.2 器官芯片闭环

### 定位

器官芯片不应只被视为湿实验平台，而应定义为：

> **人体相关功能表型 reward factory。**

它为 Agent 提供：

- function reward；
- toxicity reward；
- phenotype reward；
- mechanism reward；
- failure reward。

### 起步方向建议

建议优先从一个系统切入：

1. 肝脏芯片：ADMET、毒性、代谢，商业路径清晰；
2. 肿瘤免疫芯片：功能价值高，但复杂度较高；
3. 血管 / 炎症芯片：适合屏障、炎症、免疫迁移 readout。

### 器官芯片 reward

以炎症 / 免疫相关场景为例：

- 细胞活性；
- 炎症因子；
- 成像表型；
- barrier / TEER-like readout；
- time-series phenotype；
- toxicity；
- batch quality；
- readout sensitivity。

### 关键壁垒

1. organ-chip protocol 数据；
2. 细胞状态和 batch metadata；
3. perturbation-to-phenotype 数据；
4. 失败实验原因；
5. 与蛋白设计候选的功能反馈闭环。

---

## 5. 数据资产闭环

整个系统最重要的资产闭环如下：

```text
Scientific Resource Graph
  提供外部世界知识和工具地图

Scientific Memory
  记录内部项目状态和组织认知

Trajectory Data
  记录 Agent 和人类如何行动、决策、纠错

Reward Ledger
  记录 verifier、专家、实验反馈和成本

Agent Training
  把轨迹和 reward 转成模型能力
```

### 核心数据资产

| 资产 | 价值 |
|---|---|
| Resource Graph | 科学资源和工具可调用化 |
| Scientific Memory | 越用越聪明的组织科研账本 |
| Decision Trajectory | 训练科研 planning / reasoning / decision policy |
| Correction Trajectory | 训练错误诊断、专家纠偏、失败恢复 |
| Failure Memory | 防止重复失败，形成长期经验资产 |
| Reward Ledger | 定义科学价值，连接实验和模型训练 |
| Wet-lab Feedback | 真实世界 reward，最难复制 |

---

## 6. 最小可行产品 MVP

第一阶段不要做大而全系统。建议 MVP 聚焦三个产品能力。

### MVP 1：Target-to-Binder Research Agent

输入：一个 target。  
输出：Target Card + 设计可行性报告 + top design strategy。  
裁判：文献真实性、结构信息完整性、assay 可行性、专家 review。

### MVP 2：Protein Candidate Design & Review Loop

输入：target structure + design constraints。  
输出：top-k 候选 + 结构预测 + ranking + wet-lab plan。  
裁判：结构 / developability verifier + 专家 reviewer + 小规模实验结果。

### MVP 3：Organ-chip Experiment Planner

输入：候选蛋白 / perturbation + 假设。  
输出：cell type、chip model、readout、control、dose、time point、统计方案。  
裁判：实验负责人 review + 实验执行结果 + 表型 reward。

---

## 7. 关键系统组件

建议第一年重点建设以下 6 个系统组件。

### 7.1 Science Workspace

科研项目统一入口：

- 项目状态；
- 假设；
- 候选；
- 实验；
- 失败；
- 决策；
- Agent 任务；
- 人类审批。

### 7.2 Scientific Resource Registry

统一管理：

- 文献；
- 数据库；
- protein / target / disease / pathway；
- assay / protocol；
- tools；
- internal artifacts。

### 7.3 Scientific Memory Engine

负责：

- Event Log；
- State Graph；
- Node versioning；
- Decision / Failure / Hypothesis cards；
- Agent-facing State Packet。

### 7.4 Science Trajectory Compiler

负责把原始日志编译成：

- Episode dataset；
- Transition dataset；
- Preference dataset；
- Reward dataset；
- SFT dataset；
- Failure dataset。

### 7.5 Scientific Reward Ledger

负责记录：

- verifier result；
- expert review；
- wet-lab result；
- cost；
- information gain；
- final reward vector；
- trainability score。

### 7.6 Agent Training Pipeline

负责：

- SFT；
- preference learning；
- reward model；
- offline RL；
- online RL；
- evaluation；
- model versioning。

---

## 8. 团队组织建议

第一阶段建议 18–25 人，不宜过度膨胀。

### 8.1 AI4AI / Agentic Infrastructure 组：6–8 人

| 角色 | 人数 | 重点 |
|---|---:|---|
| Agent 系统负责人 | 1 | 多 Agent、工具调用、状态管理 |
| Agentic RL 负责人 | 1–2 | trajectory、reward、offline / online RL |
| Infra / MLOps 工程师 | 2 | sandbox、服务、数据管线、模型服务 |
| Eval / Benchmark 工程师 | 1–2 | verifier、benchmark、leaderboard |
| 科研 workflow PM | 1 | 科研流程抽象、任务设计 |

### 8.2 Scientific Data / Resource 组：3–4 人

| 角色 | 人数 | 重点 |
|---|---:|---|
| 科学知识工程师 | 1–2 | entity、claim、evidence、provenance |
| 数据工程师 | 1–2 | 文献、数据库、实验数据、索引 |
| 生物信息工程师 | 1 | 蛋白 / 多组学 / 数据库理解 |

### 8.3 蛋白质设计组：4–6 人

| 角色 | 人数 | 重点 |
|---|---:|---|
| 蛋白设计科学家 | 1–2 | binder、peptide、mini-protein |
| 结构生物 / 计算生物专家 | 1 | 结构预测、筛选、设计工具 |
| ML 研究员 | 1–2 | 生成、搜索、ranking、reward-guided design |
| 实验接口科学家 | 1 | 表达、纯化、binding assay 对接 |

### 8.4 器官芯片 / 湿实验闭环组：4–6 人

| 角色 | 人数 | 重点 |
|---|---:|---|
| Organ-chip 负责人 | 1 | 芯片模型、readout、protocol |
| 细胞生物专家 | 1–2 | cell type、organoid、疾病模型 |
| 自动化实验工程师 | 1 | 液体处理、成像、LIMS / ELN |
| 图像 / 多模态分析工程师 | 1–2 | 表型分析、time-series、omics |

### 8.5 BD / 合规 / 项目运营：2–3 人

| 角色 | 人数 | 重点 |
|---|---:|---|
| Pharma / Biotech BD | 1 | 外部合作项目 |
| IP / 合规 / 数据治理 | 1 | 数据权属、伦理、合规 |
| 项目运营 | 1 | 资源、周期、交付管理 |

---

## 9. 路线图

## 0–3 个月：建立最小闭环

目标：跑通一个可审计的 AI-assisted 科研任务闭环。

交付：

1. Science Workspace v0；
2. Target Card / Paper Card / Assay Card v0；
3. Scientific Memory 最小 schema；
4. Agent 任务状态机；
5. Trajectory logging；
6. 专家 review 表；
7. 一个 target-to-binder 可行性分析 demo。

关键结果：

```text
Agent 能围绕一个 target 完成调研、证据整理、设计建议、专家 review，并把过程写入 Memory / Trajectory。
```

---

## 3–6 个月：形成蛋白设计小闭环

目标：打通设计—计算筛选—实验建议—小规模实验反馈。

交付：

1. Protein Candidate Card；
2. 候选设计与 ranking pipeline；
3. structure / developability verifier；
4. 小规模表达 / binding 实验接入；
5. Reward Ledger v0；
6. Science Trajectory Compiler v0；
7. 第一批 SFT / preference 数据导出。

关键结果：

```text
完成至少一个 target 的 top-k candidate design，并拿到初步实验反馈。
```

---

## 6–12 个月：形成干湿反馈飞轮

目标：将实验结果稳定反哺 Memory、Reward 和 Agent Training。

交付：

1. Evidence Graph v1；
2. Failure Memory v1；
3. Decision-Outcome linkage；
4. Agent-facing State Packet；
5. Offline RL / preference learning prototype；
6. Organ-chip Experiment Planner v0；
7. 一个 organ-chip phenotype reward demo。

关键结果：

```text
系统不只是执行任务，而能从失败和实验反馈中更新下一轮设计策略。
```

---

## 12–18 个月：平台化与外部合作

目标：形成可复用的 Science Agent OS + 两个垂直场景闭环。

交付：

1. Science Agent OS v1；
2. Resource Graph v1；
3. Scientific Memory v1；
4. Trajectory / Reward Dataset v1；
5. Agent Training Pipeline v1；
6. Protein Design Closed-loop v1；
7. Organ-chip Reward Factory v1；
8. 1–2 个外部合作项目。

关键结果：

```text
证明该系统能在真实科研任务中提升候选发现效率、降低重复失败、缩短迭代周期。
```

---

## 10. 关键指标

### 平台指标

| 维度 | 指标 |
|---|---|
| 任务执行 | Agent 完成任务比例、人工介入次数 |
| 复现性 | 可 rerun 的代码 / 实验 / 工具调用比例 |
| 记忆质量 | 状态包准确率、过期结论识别率 |
| 轨迹质量 | 可训练 trajectory 数量、decision coverage |
| Reward 质量 | verifier 覆盖率、专家一致性、实验反馈率 |
| 训练效果 | 训练后任务成功率、候选排序提升 |

### 科学指标

| 维度 | 指标 |
|---|---|
| 蛋白设计 | top-k 实验成功率、表达成功率、binding 成功率 |
| 器官芯片 | 表型 readout 稳定性、机制区分能力、毒性识别率 |
| 科研效率 | 从 target 到实验候选的周期、单位预算有效候选数 |
| 失败复用 | 重复失败率下降、failure rule 复用次数 |
| 信息增益 | 每轮实验减少的不确定性、决策改变次数 |

### 北极星指标

建议定义为：

> **单位实验预算下产生有效科学结论 / 有效候选的效率提升。**

---

## 11. 护城河设计

### 第一层：资源护城河

- 高质量文献索引；
- 生物数据库镜像；
- protein / target / assay / protocol 结构化资源；
- 实验数据；
- 内部失败样本；
- 专家审查记录。

### 第二层：状态护城河

- 项目状态；
- 假设树；
- 证据链；
- 决策历史；
- 失败路径；
- 专家偏好。

### 第三层：轨迹护城河

- Agent 执行轨迹；
- 人类纠偏轨迹；
- 多专家争议轨迹；
- 实验反馈轨迹；
- 失败恢复轨迹。

### 第四层：Reward 护城河

- 程序 verifier；
- 证据 verifier；
- 专家 rubric；
- wet-lab assay；
- organ-chip phenotype；
- 成本 / 周期 / 成功率；
- 科学价值评价。

最难复制的是：

> **真实科研失败轨迹 + 专家纠偏 + 实验反馈 + organ-chip phenotype reward。**

---

## 12. 主要风险与规避

### 风险 1：做成普通科研 Copilot

规避：坚持做 Memory、Trajectory、Reward、Training，不只做聊天和文献总结。

### 风险 2：只做 RAG，不做资源图谱

规避：从 entity、claim、evidence、provenance、task card 入手。

### 风险 3：没有真实 wet reward

规避：蛋白设计和器官芯片必须作为 feedback layer，而不是展示 demo。

### 风险 4：轨迹数据不可训练

规避：建设 Science Trajectory Compiler，从一开始按 state-action-observation-reward 记录。

### 风险 5：Reward hacking

规避：visible verifier + hidden verifier + expert audit + wet-lab validation。

### 风险 6：团队过度偏算法

规避：必须配置科研 workflow PM、实验接口科学家、数据工程和 wet-lab 负责人。

### 风险 7：做得太大，第一年没有闭环

规避：第一年只聚焦 target-to-binder + 一个 organ-chip reward 场景。

---

## 13. 当下最需要决策的问题

### 战略层

1. 第一年优先打穿哪个蛋白设计任务？
   - binder；
   - peptide；
   - enzyme；
   - antibody-like molecule。

2. 器官芯片第一优先系统是什么？
   - 肝脏；
   - 肿瘤免疫；
   - 血管 / 炎症。

3. 是先服务内部科研，还是一开始就设计外部合作产品？

### 产品层

4. Science Workspace 是内部系统，还是未来商业化产品？
5. Scientific Memory 是否作为所有项目的强制系统 of record？
6. 人类审批节点如何设计，哪些任务必须审批？

### 数据层

7. 文献和公共数据库资源是否需要自建镜像？
8. 实验数据、失败样本、专家 review 的数据权属如何定义？
9. Trajectory 数据是否默认可用于模型训练？

### 组织层

10. 第一阶段团队规模是 10 人、20 人还是 30 人？
11. 湿实验是自建、合作还是外包？
12. 是否需要早期绑定高校 / 药企 / CRO / 器官芯片公司合作？

---

## 14. 建议的内部表述

可以对管理层这样讲：

> 我们不是做一个单点 AI4Sci 应用，而是建设一套科研智能体进化基础设施。通用 Agent 负责执行，科学资源图谱提供知识和工具，Scientific Memory 记录项目状态，Trajectory / Reward 将科研过程变成训练数据，Agent Training 让系统持续变强。蛋白质设计和器官芯片是第一批真实闭环场景，用于产生高价值实验反馈和物理世界 reward。长期看，这套系统会沉淀为自动化科研的基础设施。

可以对技术团队这样讲：

> 我们的核心系统是 Resource Graph、Scientific Memory、Science Trajectory Compiler、Scientific Reward Ledger 和 Agent Training Pipeline。不要把重点放在重写 Agent OS，而要把科研资源、状态、决策、失败、实验反馈结构化，并编译成可训练数据。

可以对科学家这样讲：

> 这个系统不是替代科学家，而是把科研项目中的假设、证据、候选、实验、失败、决策持续记录下来，让 Agent 帮助调研、设计、复盘和提出下一步建议。科学家负责关键判断，系统负责让判断可追溯、可复用、可训练。

---

## 15. 最终总结

本方案的核心不是“AI 帮科学家写报告”，而是：

> **让科研过程本身变成可计算、可审计、可训练、可进化的系统。**

最终形成五个核心资产：

1. **Scientific Resource Graph**：科学资源和工具地图；
2. **Scientific Memory**：组织科研状态账本；
3. **Trajectory Data**：Agent 和人类科研决策轨迹；
4. **Reward Ledger**：科学价值和实验反馈裁判系统；
5. **Agent Training Pipeline**：让系统持续进化的训练引擎。

蛋白质设计和器官芯片不是孤立业务，而是这套基础设施的第一批高价值训练场和验证场。

长期愿景：

```text
从 AI-assisted science
到 AI-executed science
再到 AI-evolving science infrastructure
```

也就是：

> **从辅助科研，到自动化科研，再到能够自我进化的科学研究基础设施。**
