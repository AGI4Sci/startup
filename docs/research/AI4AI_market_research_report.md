# AI4AI 公司与机构系统调研报告

**日期**：2026-06-29
**口径**：公开资料调研，覆盖全球与中国代表性公司、科研机构、开源社区和标准/安全组织。  
**定义**：本报告中的 AI4AI 指“用 AI 或高度自动化系统来提升 AI 研发、训练、推理、部署、评测、安全、数据生产和科研发现”的技术、产品与机构生态。

---

## 1. Executive Summary

AI4AI 正从“辅助工具”变成 AI 产业的核心生产资料。它不只是 AI 编程助手，也不只是 MLOps，而是覆盖 AI 生产全链路的基础设施：算力、数据、模型训练、推理优化、Agent 开发、评测、可观测、安全对齐、自动化科研和开源生态。

截至 2026 年，商业化最成熟的方向主要有四类：

1. **算力与推理云**：NVIDIA、CoreWeave、Lambda、Cerebras、Groq、Together AI、Fireworks、Baseten 等正在把 GPU/ASIC、调度、模型服务和开发平台打包为“AI 工厂”。
2. **AI 编程与软件工程 Agent**：GitHub Copilot、OpenAI Codex、Claude Code、Cursor、Devin、Replit、Lovable、Vercel v0 等正在从代码补全走向异步软件工程代理。
3. **LLMOps、评测与可观测性**：LangSmith、Arize/Phoenix、Braintrust、Langfuse、Galileo、W&B/Weave、Datadog 等解决 Agent 上线后的质量、成本、回归和 trace 问题。
4. **数据、RLHF 与合成数据**：Scale AI、Snorkel、Labelbox、Mercor、Databricks、Hugging Face、NVIDIA Cosmos、Gretel、Mostly AI 等围绕高质量训练数据、专家反馈、合成数据和数据治理构建壁垒。

科研机构和安全评测机构的战略重要性快速上升。Google DeepMind 的 AlphaEvolve、Sakana AI 的 AI Scientist、FutureHouse、Microsoft Discovery、上海 AI Lab Intern-Discovery 等代表“AI 做科研”的早期路线；METR、NIST CAISI、UK AI Security Institute、MLCommons AILuminate、EU AI Office 等代表“AI 能否安全地改进 AI”的外部度量与治理路线。

2026 年 Q1 以来，“AI 自我迭代/递归自改进”成为 AI4AI 里最强的新增融资与叙事热点。Recursive Superintelligence、Ineffable Intelligence、Ricursive Intelligence、Mirendil、Deeptune、AfterQuery、General Intuition、AMI Labs 等海外创业公司，分别押注自动化 AI 研究、经验驱动强化学习、训练环境、AI 芯片闭环和世界模型；中国则更集中在具身智能、世界模型、物理 AI 数据与 Agentic OS，例如自变量机器人、星海图、极佳视界、千寻智能、光轮智能、Flowith、MemoraX AI 和中数睿智。

中国市场呈现“大厂云平台 + 国产算力 + 企业私有化 AI 开发工具 + 中文评测/开源生态”的结构。代表力量包括华为昇腾/华为云、阿里云 PAI/百炼/通义灵码、百度智能云千帆/Comate、火山引擎方舟/Trae、腾讯云 TI-ONE/CodeBuddy、上海 AI Lab/OpenCompass、智源/FlagEval、ModelScope、Dify、DeepSeek、CodeGeeX、海天瑞声、数据堂、光轮智能和第四范式。

---

## 2. AI4AI 的产业链框架

| 层级 | 核心问题 | 海外代表 | 中国代表 |
|---|---|---|---|
| 算力与 AI 云 | 训练、推理、GPU 调度、AI 工厂 | NVIDIA、AMD、Google TPU、AWS Trainium、CoreWeave、Lambda、Crusoe、Cerebras、Groq、Together AI、Fireworks、Baseten | 华为昇腾/华为云、阿里云 PAI、百度百舸/昆仑芯、腾讯云 HCC/TI-ONE、火山方舟、商汤 SenseCore、寒武纪、壁仞、摩尔线程、沐曦、燧原 |
| 训练/推理优化 | 降低训练和推理成本，提高吞吐 | TensorRT-LLM、Triton、vLLM、SGLang、Ray/Anyscale、Modular、Databricks/Mosaic | PAI-Blade/TorchAcc、MindSpore/CANN、飞桨、国产推理框架生态 |
| AI 编程与软件工程 Agent | 代码生成、重构、测试、PR、异步开发 | GitHub Copilot、OpenAI Codex、Claude Code、Cursor、Devin/Cognition、Replit、Lovable、Vercel v0、Bolt、Augment、Sourcegraph/Amp、Tabnine、Poolside | 通义灵码/Qoder、百度 Comate、Trae、MarsCode、华为 CodeArts、腾讯 CodeBuddy、CodeGeeX、DeepSeek Coder |
| Agent 框架与应用开发 | 多 Agent 编排、RAG、工具调用、工作流 | LangChain/LangGraph/LangSmith、LlamaIndex、CrewAI、Microsoft Agent Framework、OpenAI Agents SDK、Google ADK、AWS Bedrock AgentCore | Dify、ModelScope AgentScope、MetaGPT、百度千帆、阿里百炼、火山方舟、腾讯元器 |
| LLMOps/评测/可观测性 | Trace、eval、prompt 回归、成本、质量门禁 | Arize/Phoenix、Braintrust、Langfuse、Galileo、W&B/Weave、Datadog、Comet/Opik、Promptfoo、Ragas、DeepEval | OpenCompass、FlagEval、SuperCLUE、信通院可信 AI 评测体系 |
| 数据/RLHF/合成数据 | 高质量数据、专家反馈、仿真数据、数据治理 | Scale AI、Snorkel、Labelbox/Alignerr、Mercor、Surge AI、Appen、TELUS、Databricks、Snowflake、Hugging Face、Gretel、Mostly AI、Tonic、NVIDIA Cosmos、Parallel Domain | 海天瑞声、数据堂、Testin 云测、龙猫数据、整数智能、Data-Juicer、光轮智能、51Sim、卓印智能 |
| 自我迭代与 Agentic RL | 自动化 AI 研究、可交互环境、可验证奖励、长程 rollout、递归改进 | Recursive Superintelligence、Ineffable Intelligence、Ricursive Intelligence、Mirendil、Deeptune、AfterQuery、Prime Intellect、General Intuition、AMI Labs | Flowith、MemoraX AI、光轮智能、极佳视界、星海图、自变量机器人、千寻智能、中数睿智 |
| AutoML/NAS | 自动建模、调参、架构搜索、模型压缩 | Google Vertex AutoML/NAS、AWS SageMaker Autopilot、Azure AutoML/NNI、DataRobot、H2O.ai、Dataiku | 第四范式、华为 ModelArts、阿里云 PAI、百度 EasyDL/飞桨、腾讯 TI-ONE |
| 科研/开源/安全机构 | AI 研究自动化、标准、风险评测 | Google DeepMind、OpenAI、Anthropic、Meta FAIR、Microsoft Research、Ai2、Stanford CRFM/HAI、Berkeley BAIR、Hugging Face、PyTorch Foundation、EleutherAI、LMArena、METR、NIST CAISI、UK AISI、MLCommons、EU AI Office | 上海 AI Lab、北京智源 BAAI、OpenMMLab、InternLM、OpenCompass、ModelScope、鹏城实验室、之江实验室、北大科学智能学院、中国信通院 |

---

## 3. 全球代表公司与机构

### 3.1 算力、AI 云与推理平台

| 公司/机构 | 核心产品/技术 | AI4AI 价值 | 近期进展/备注 |
|---|---|---|---|
| NVIDIA | Blackwell/Rubin GPU、CUDA、TensorRT-LLM、Triton、NVLink、DGX Cloud、Run:ai | 训练、推理、调度、网络、软件栈全覆盖，是 AI 工厂的事实底座 | 收购 Run:ai 强化 GPU 调度；TensorRT-LLM 持续服务 LLM 推理优化 |
| AMD | Instinct MI300/MI350/MI400、ROCm | NVIDIA 替代路线，降低算力供应和成本风险 | 通过 ROCm 强化开源生态和大模型支持 |
| Google Cloud | TPU、AI Hypercomputer、Vertex AI | 自研加速器与云平台深度绑定 | Ironwood TPU 面向推理时代 |
| AWS | Trainium、Inferentia、Neuron、SageMaker、Bedrock | 低成本训练/推理芯片与模型平台 | Anthropic 等大客户推动 Trainium 生态 |
| Microsoft Azure | Azure AI、Maia 100、Azure OpenAI、Copilot 基础设施 | 服务大规模模型训练、推理和企业 AI 应用 | 与 OpenAI/GitHub/Copilot 形成应用牵引 |
| CoreWeave | GPU 云、Kubernetes 集群、托管训练/推理 | Neocloud 代表，面向 AI 原生工作负载优化 | 2025 年完成对 Weights & Biases 的收购，补齐开发平台 |
| Lambda | GPU 云、Superintelligence Cloud、GPU 服务器 | 为 AI 团队提供低门槛算力 | 2025 年获超 15 亿美元融资用于扩展 AI 云 |
| Crusoe | 能源优先 AI 数据中心、Crusoe Cloud | 绑定能源与数据中心，降低 AI factory 成本 | 大规模融资扩张 AI 基础设施 |
| Cerebras | Wafer-Scale Engine、CS 系统、推理云 | 大芯片路线减少多卡通信瓶颈 | 面向训练和低延迟推理 |
| Groq | LPU、GroqCloud | 低延迟高吞吐推理 | 主打推理时代 tokens/sec |
| Together AI | 开放模型训练/推理 API、AI Acceleration Cloud | 降低开放模型部署和微调成本 | 2025 年获 3.05 亿美元融资 |
| Fireworks AI | 高性能开放模型 API 和推理平台 | 支持开放模型生产化、定制化和高吞吐推理 | 2025 年融资后估值约 40 亿美元 |
| Baseten | 模型推理部署平台、跨云 GPU 调度 | 服务企业私有模型上线 | 2026 年继续融资扩张推理平台 |
| Runpod | On-demand GPU、serverless GPU | 开发者和小团队低门槛算力 | 面向开发者生态增长 |
| Modular | MAX、Mojo | 跨 CPU/GPU/ASIC 的统一 AI 计算层 | 试图降低 CUDA 锁定 |

### 3.2 AI 编程与软件工程 Agent

| 公司/机构 | 核心产品 | AI4AI 价值 | 近期进展/备注 |
|---|---|---|---|
| Microsoft / GitHub | GitHub Copilot、Agent Mode、Copilot coding agent、Agent HQ | 从补全到异步开发、代码评审和多 Agent 编排入口 | GitHub Copilot 已成为 AI 编程主流入口 |
| OpenAI | Codex Web/CLI/App/IDE、Codex SDK、Agents SDK、Evals | 自动编码、PR、测试、长任务代理与评测闭环 | Codex 成为 OpenAI 面向软件工程的核心产品线 |
| Anthropic | Claude Code、Model Context Protocol | 终端原生编码代理和工具/数据连接标准 | Claude Code 与 MCP 强化开发者生态 |
| Anysphere / Cursor | Cursor AI IDE、Agent、Composer、Background Agent | AI 原生 IDE 标杆，强调 repo 级上下文与多步修改 | 2025 年 Series D 融资 23 亿美元，投后 293 亿美元 |
| Cognition | Devin、Devin Desktop | 任务级软件工程代理 | 收购 Windsurf，强化 AI 编程入口 |
| Windsurf / Codeium | Agentic IDE、AI 编程插件 | 插件式和 IDE 式 AI 编程 | 并入 Cognition/Devin 生态 |
| Replit | Replit Agent、Agent 4 | 浏览器端从自然语言到应用、部署和协作 | 面向非专业开发者和全栈原型 |
| Lovable | Prompt-to-app / vibe coding | 非专业开发者快速生成应用 | 资本关注度高 |
| Vercel | v0.app | 生成 Web 应用、组件和前端代码 | 与 Vercel 部署生态天然结合 |
| StackBlitz / Bolt | bolt.new、WebContainers | 浏览器内全栈 AI Web 开发 | 开发者体验强 |
| AWS | Amazon Q Developer、Kiro | 编码、迁移、spec-driven development | 与 AWS 云开发流程整合 |
| Google | Gemini Code Assist、Jules | 编码代理、代码理解、异步任务 | 与 Google Cloud、Gemini 生态结合 |
| Augment Code | 企业级代码助手 | 大型代码库上下文理解 | 面向企业私有代码库 |
| Sourcegraph / Amp | Cody、Amp、Code Search | 大代码库检索、理解与代码代理 | Sourcegraph 与 Amp 分拆后分别聚焦 |
| Tabnine | 企业私有化 AI coding platform | 安全合规、本地/隔离部署 | 企业市场定位清晰 |
| Poolside AI | 软件工程基础模型 | 面向企业、政府和防务的软件自动化 | 2024 年获得大额融资 |

### 3.3 Agent 框架、LLMOps 与评测可观测性

| 公司/项目 | 核心产品/技术 | AI4AI 价值 |
|---|---|---|
| LangChain | LangChain、LangGraph、LangSmith | Agent 编排、状态图、调试、评测和生产观测 |
| LlamaIndex | 数据/RAG/知识 Agent 框架、LlamaCloud、LlamaParse | 帮助 Agent 接入企业知识和非结构化数据 |
| CrewAI | 多 Agent 编排框架与企业平台 | 角色、任务、工具协作 |
| Microsoft Agent Framework | AutoGen 与 Semantic Kernel 的统一方向 | 企业级多 Agent SDK 和运行时 |
| OpenAI Agents SDK | Agent 构建、工具调用、handoff、trace | OpenAI 原生 Agent 开发底座 |
| Google ADK | Agent Development Kit | 面向 Gemini/Google Cloud 的 Agent 开发 |
| AWS Bedrock AgentCore | Agent 运行时、身份、记忆、评测 | 云原生 Agent 部署与治理 |
| Arize / Phoenix | AI/LLM/Agent observability、eval、OpenTelemetry/OpenInference | 生产 Agent trace、评测和质量分析 |
| Braintrust | AI eval、数据集、实验、回归测试、生产反馈 | 把 AI 产品质量门禁工程化 |
| Langfuse | 开源 LLM engineering platform | trace、prompt、eval、成本监控和自托管 |
| Galileo | AI observability、evaluation、guardrails | 生产 Agent 可靠性 |
| Weights & Biases / Weave | 实验追踪、GenAI trace/eval | 从传统 MLOps 扩展到 GenAI 生命周期 |
| Datadog | LLM Observability | APM 与 LLM trace/cost/eval 结合 |
| Comet / Opik | 开源 LLM eval/observability | prompt 版本、实验与评测管理 |
| Promptfoo | Prompt 回归测试、CI 集成 | 轻量级评测工具 |
| Ragas | RAG 评测 | RAG pipeline 的质量评估 |
| DeepEval | LLM-as-judge、CI 评测 | 开源评测与测试框架 |

### 3.4 数据、RLHF 与合成数据

| 公司/机构 | 核心产品/技术 | AI4AI 价值 |
|---|---|---|
| Scale AI | Data Engine、Data Foundry、RLHF、评测数据 | 人类专家 + 数据工具链，为前沿模型生产训练/对齐/评测数据 |
| Snorkel AI | Snorkel Flow、程序化标注、弱监督 | 用规则、模型和人审组合降低高质量标签成本 |
| Labelbox / Alignerr | AI data factory、RL data engine、专家网络 | 偏好数据、评测、专家标注与 RL 数据生产 |
| Mercor | 专家人才网络 | 为 AI 实验室提供代码、医学、法律等高难专家数据 |
| Surge AI | 专家和众包混合数据 | 面向大模型训练和评测 |
| Appen / TELUS / Sama / iMerit | 传统标注和专家数据服务 | 从 CV/NLP 标注转向 GenAI、RLHF 和评测 |
| Databricks | Lakehouse、Unity Catalog、Mosaic AI、MLflow、Lilac | 把企业数据变成可治理、可训练、可评测的 AI 资产 |
| Snowflake | AI Data Cloud、Cortex AI、数据治理 | 在安全边界内调用企业结构化/非结构化数据 |
| Hugging Face | Hub、Datasets、Evaluate、Spaces、AutoTrain | 全球模型和数据分发、复现、评测底座 |
| NVIDIA | Cosmos、Omniverse Replicator、Isaac Sim、NeMo synthetic data | 为机器人、自动驾驶、LLM 生成可控合成数据 |
| Gretel | 隐私保护合成数据 | 企业结构化数据合成 |
| Mostly AI | 合成数据平台 | 隐私合规场景下的数据生成 |
| Tonic.ai | 测试数据和合成数据 | 软件测试、数据安全和 AI 训练 |
| Parallel Domain | 自动驾驶/机器人仿真数据 | 长尾场景、传感器组合和视觉数据生成 |
| Synthesis AI | 计算机视觉合成数据 | 视觉模型训练数据生成 |

### 3.5 AutoML、NAS 与自动化模型工程

| 公司/平台 | 核心产品/技术 | AI4AI 价值 |
|---|---|---|
| Google Cloud / Google Research | Vertex AI AutoML、Neural Architecture Search | 自动搜索模型结构、超参、精度/延迟/内存权衡 |
| AWS | SageMaker Autopilot | 自动建模、特征处理和模型选择 |
| Microsoft | Azure AutoML、NNI | 自动特征工程、超参优化、NAS、模型压缩 |
| DataRobot | 企业 AutoML、MLOps、治理 | 从 AutoML 扩展到 AI 平台 |
| H2O.ai | Driverless AI | 自动特征工程、建模和调参 |
| Dataiku | 企业 AI/ML 平台 | 面向业务用户和数据科学团队的自动化建模 |

### 3.6 科研、开源、安全与标准机构

| 机构 | 方向 | AI4AI 价值 |
|---|---|---|
| Google DeepMind / Google Research | 基础模型、AI for Science、算法发现、AlphaEvolve | 直接用 AI 优化算法、芯片、数据中心和训练流程 |
| OpenAI | 推理模型、Codex、Evals、Preparedness Framework、Model Spec | 自动编码、评测、安全和模型行为规范 |
| Anthropic | Claude、Claude Code、MCP、Responsible Scaling Policy | 编码代理、工具协议和安全扩展框架 |
| Meta AI / FAIR | Llama、开放模型、多模态和训练基础设施 | 开放权重生态降低研发门槛 |
| Microsoft Research / AI for Science | Microsoft Discovery、MatterGen、Aurora | 多智能体 R&D、材料生成和科学基础模型 |
| Allen Institute for AI | OLMo、开放数据和训练透明化 | 为学界复现和研究训练机制提供样本 |
| Stanford HAI / CRFM | AI Index、HELM、Foundation Model Transparency Index | 中立测量、透明度和政策研究 |
| Berkeley BAIR、MIT CSAIL、Mila、Vector、ELLIS | 基础研究、RL、机器人、多模态 | 人才与前沿研究源头 |
| Hugging Face | Hub、Transformers、Datasets、Spaces | 全球开源模型与数据基础设施 |
| PyTorch Foundation / Linux Foundation | PyTorch、Ray、开放 AI compute stack | 训练和分布式计算事实标准 |
| EleutherAI / LAION / LMArena | 开放数据、LM Evaluation Harness、Chatbot Arena | 开放评测和社区基准 |
| METR | 长任务、自主能力、AI R&D 加速评测 | 衡量模型能否完成越来越长的真实任务 |
| NIST CAISI | 美国 AI 测量科学、风险管理和安全评测 | 外部 TEVV 框架和标准 |
| UK AI Security Institute | 前沿模型安全评测、红队、能力趋势监测 | 公共安全评测机构代表 |
| MLCommons / AILuminate | AI 安全和风险基准 | 行业中立安全 benchmark |
| EU AI Office | AI Act、GPAI Code、透明度和系统性风险 | 监管和合规标准制定 |
| FutureHouse | AI Scientist、科研 Agent | 文献检索、综述、实验规划、数据分析 |
| Sakana AI | The AI Scientist | 自动提出假设、写代码、跑实验、写论文 |

### 3.7 AI 自我迭代、Agentic RL 与自动化 AI 研究

2026 年 Q1 以来，海外市场出现一批明确把“AI 改进 AI”“从经验中学习”“自动化 AI 研究”作为核心叙事的创业公司。它们与传统 AI infra、AI coding、LLMOps 的区别在于：不只提供工具，而是试图构建可持续产生训练信号的闭环系统，包括代码环境、芯片设计、游戏/物理世界、实验室、专家工作流和自动化评测。

| 公司/机构 | 2026 年 Q1 以来融资与估值 | 核心路线 | AI4AI 价值与判断 |
|---|---|---|---|
| Recursive Superintelligence | 2026 年 5 月宣布 A 轮 6.5 亿美元，估值约 46.5 亿美元；此前 FT/Sifted 口径为至少 5 亿美元 | Recursive self-improvement、automated AI research、self-improving coding agents、open-ended algorithms | 最贴近“递归自改进”的公司之一，直接把 AI 自动研究和 AI 科学家作为目标；融资额口径需跟踪公司正式披露 |
| Ineffable Intelligence | 2026 年 4 月种子轮 11 亿美元，估值约 51 亿美元；Sequoia、Lightspeed 等参与 | David Silver 路线，强化学习 superlearner，从环境经验而非人类数据中学习 | 2026 年 RL 回潮的标志性事件；强调 no pre-training / no imitation 的经验优先路线 |
| Ricursive Intelligence | 2026 年 1 月 A 轮 3 亿美元，投后估值 40 亿美元；Lightspeed 领投，DST、NVentures、Felicis、Sequoia 等参与 | AI-driven semiconductor design、model-hardware co-evolution | 用 AI 设计更优 AI 芯片，再用芯片反过来加速 AI，属于“硬件-模型”递归闭环 |
| Mirendil | 2026 年 6 月种子轮 2 亿美元，估值约 10 亿美元；a16z、Kleiner Perkins 领投，NVIDIA 等参与 | Self-accelerating AI R&D、frontier AI research automation | 前 Anthropic/Google 研究员团队，目标是让科学家训练自己的 AI 研究助手，是 AI lab 自动化的纯正玩家 |
| Deeptune | 2026 年 3 月 A 轮 4300 万美元；a16z 领投 | Agent training gyms、computer-use/code environments、agentic RL | 把“训练环境”产品化，为前沿模型团队提供可交互任务和可验证反馈 |
| AfterQuery | 2026 年 4 月 A 轮 3000 万美元，估值约 3 亿美元；Altos 领投 | Expert data、RL environments、agent evals、computer-use workflows | 从专家数据延展到 RL 环境与 Agent 评测，属于前沿实验室的数据和 reward infrastructure |
| General Intuition | 2026 年 6 月 A 轮 3.2 亿美元，估值约 23 亿美元；Khosla Ventures 领投 | Game data、world models、spatial-temporal reasoning、agents learn to act | 从游戏和虚拟环境中学习可迁移的行动模型，连接数字世界 Agent 与物理世界 Agent |
| AMI Labs / Advanced Machine Intelligence | 2026 年 3 月种子轮 10.3 亿美元，估值约 35 亿美元；投资方完整名单仍需跟踪 | Yann LeCun 路线，world models、现实表征学习、非纯 LLM 路线 | 与 Ineffable 同样反对“只靠语言数据”，但更偏世界模型和现实理解 |
| Prime Intellect | 2026 年 2 月发布 Lab、Environments Hub、Hosted Training 和 Hosted Evaluations；未披露同期新融资 | Open RL environments、self-improving agents、distributed training | 更偏平台层，把环境、rollout、训练和评测基础设施开放给开发者和企业 |
| Periodic Labs | 2026 年 5 月媒体称正在洽谈 5 亿美元新融资，估值 70-75 亿美元；新轮未确认 | AI scientist、autonomous labs、materials discovery、nature as RL environment | 把真实物理实验室作为 reward environment，是 AI4Sci 与 AI 自我迭代的交汇方向 |
| Core Automation | 2026 年 5 月媒体称已融资 1 亿美元，并寻求 3-5 亿美元甚至更高融资；信息未充分确认 | Continual learning、automated AI lab、new learning algorithms | 观察项，代表前 OpenAI 人才向“持续学习/自动化实验室”外溢 |

上述公司可以分成四类：一是 Recursive Superintelligence、Mirendil 代表的“AI 自动化 AI 研究”；二是 Ineffable、Prime Intellect、Deeptune、AfterQuery 代表的“环境 + 奖励 + rollout”；三是 Ricursive 代表的“AI 设计 AI 硬件”；四是 AMI Labs、General Intuition、Periodic Labs 代表的“世界模型/物理实验环境”。它们共同指向同一个判断：下一轮 AI4AI 的瓶颈不只是模型规模，而是能否形成可验证、可扩展、可复用的经验闭环。

---

## 4. 中国代表公司与机构

### 4.1 大厂云与平台

| 公司/机构 | 核心产品/技术 | AI4AI 价值 |
|---|---|---|
| 阿里云 | PAI、PAI-灵骏、百炼、通义灵码、ModelScope、AgentScope | 覆盖训练、推理、模型服务、Agent 构建、AI 编程和开源社区 |
| 百度智能云 | 千帆、百舸、文心快码 Comate、昆仑芯 | 模型开发、部署、调优、AI 编程和自研芯片闭环 |
| 华为云 / 昇腾 | Ascend、CANN、MindSpore、ModelArts、CodeArts | 国产算力、云平台、MLOps 和研发 Agent |
| 火山引擎 | 火山方舟、豆包、Trae、MarsCode | 模型服务、Agent 部署、AI IDE 和编程助手 |
| 腾讯云 | TI-ONE、HCC、混元、CodeBuddy、元器 | 训练/推理平台、AI 编程和 Agent 应用构建 |
| 商汤 | SenseCore AI 大装置 | 大规模算力调度、模型训练和生成式 AI 平台 |

### 4.2 国产 AI 芯片与基础设施

| 公司 | 核心产品/技术 | AI4AI 价值 |
|---|---|---|
| 华为昇腾 | Ascend 910B/910C、Atlas、CANN | 国产训练/推理主平台 |
| 寒武纪 | MLU 系列 | 云端 AI 训练和推理加速 |
| 壁仞科技 | GPGPU、BIRENSUPA | 训练、推理和边缘 AI |
| 摩尔线程 | MUSA、全功能 GPU | AI 计算、图形和科学计算 |
| 沐曦集成 | MetaX GPU | 国产 AI 训练/推理方案 |
| 燧原科技 | GCU/云燧 | AI 训练和推理芯片 |
| 天数智芯 | 通用 GPU | 训练/推理组合方案 |
| 百度昆仑芯 | 昆仑芯 P800 等 | 与百度智能云/文心模型深度耦合 |

### 4.3 AI 编程、Agent 与开源框架

| 公司/项目 | 核心产品/技术 | AI4AI 价值 |
|---|---|---|
| 通义灵码 | AI 编码助手、企业版 | 代码生成、问答、单测、研发流程辅助 |
| 百度 Comate | 文心快码 | 代码生成、注释、单测、企业私有化 |
| Trae / MarsCode | AI IDE 和编程助手 | 面向国内开发者的 AI coding 入口 |
| 华为 CodeArts | 代码智能体、研发流程 Agent | 企业 DevOps + AI |
| 腾讯 CodeBuddy | AI 编程助手 | 代码理解、生成和企业接入 |
| CodeGeeX | 代码生成/翻译/补全 | 清华/智谱系国产代码模型与工具 |
| DeepSeek Coder | 开源/开放代码模型 | 降低国产 AI 编程成本 |
| Dify | 开源 Agentic workflow/RAG 平台 | 中国团队、全球开源生态，适合企业 Agent 构建 |
| MetaGPT | 多 Agent 软件公司框架 | 模拟产品、架构、工程角色协作 |
| ModelScope AgentScope | 多 Agent 开发框架 | 与魔搭模型社区结合 |

### 4.4 评测、数据与 AI4Sci

| 公司/机构 | 核心产品/技术 | AI4AI 价值 |
|---|---|---|
| 上海 AI Lab | OpenCompass、OpenMMLab、InternLM、Intern-Discovery | 中国 AI4AI 公共研发底座，覆盖模型、评测、AI4Sci |
| 北京智源 BAAI | FlagOpen、FlagEval、BGE、FlagOS | 开源模型、数据、算法、评测和系统软件 |
| 中国信通院 CAICT | 可信 AI、方升大模型基准、数据集质量评估 | 国内模型评测、合规和产业落地标准 |
| SuperCLUE | 中文大模型评测 | 中文场景能力、Agent 和工具调用评估 |
| 海天瑞声 | 语音/CV/NLP/多模态数据、标注、清洗 | 大模型训练和评测数据供应 |
| 数据堂 | 版权数据集、多模态数据 | 大模型数据资产 |
| Testin 云测 | AI 数据与测试服务 | 数据标注、模型测试和质量保障 |
| 龙猫数据 | 数据采集标注 | 大模型数据服务 |
| 整数智能 | 数据工程平台、ACE Service | 自动化标注和数据工程 |
| Data-Juicer | 数据清洗、合成、分析、标注 | 预训练/微调数据工程模块化 |
| 光轮智能 | 自动驾驶/具身智能仿真合成数据 | 物理 AI、机器人和自动驾驶数据闭环 |
| 51Sim | 自动驾驶仿真、合成数据 | 长尾场景和仿真评测 |
| 卓印智能 JoinAI | Simulaix/Terra | 端到端生成训练数据 |
| 第四范式 | Sage HyperCycle、先知 AI 平台 | 企业 AutoML 和行业模型开发 |
| 深势科技 DP Technology | 科学大模型、药物/材料研发工具 | AI for Science 工具链，可反哺科研 Agent |
| 北京科学智能研究院 | AI for Science、物理建模、数值算法、HPC | 中国科学智能基础设施 |

### 4.5 AI 自我进化、具身世界模型与 Agentic OS

国内 2026 年 Q1 以来的“AI 自我迭代”融资热度，更多体现为具身智能、世界模型、物理 AI 数据闭环和企业 Agentic OS。与海外 Recursive / Ineffable 这类纯 AI 研究自动化公司相比，国内公司更强调真实场景数据、机器人本体、仿真合成数据、评测和部署反馈。

| 公司/团队 | 2026 年 Q1 以来融资进展 | 核心路线 | AI4AI 价值与判断 |
|---|---|---|---|
| 自变量机器人 X Square | 2026 年 1 月 A++ 轮 10 亿元；2026 年 4 月媒体称 B 轮近 20 亿元，需以公司确认为准 | 通用具身智能大模型、VLA、世界模型、真实场景数据闭环 | WALL-A 将 VLA 与世界模型融合，强调感知、预测、推理和动作统一；代表国内具身基础模型大额融资 |
| 星海图 Galaxea AI | 2026 年 2 月 B 轮 10 亿元；2026 年 4 月 B+ 轮 20 亿元 | 真实数据路线、VLA、世界模型、机器人生产力场景 | 从开发者市场转向生产场景，订单和场景数据反哺模型迭代 |
| 极佳视界 | 2026 年 Q1 至 Q2 连续完成大额融资；公开报道包括 Pre-B 约 10 亿元、B1 约 15 亿元、6 月 B2 轮 10 亿元 | 世界模型驱动物理 AGI、GigaWorld/GigaBrain、强化学习自我进化 | 明确提出“世界模型 + 强化学习”的自我进化路线，是国内与 Ineffable/AMI 相邻的物理 AI 代表 |
| 千寻智能 Spirit AI | 2026 年 2 月连续融资近 20 亿元；2026 年 6 月 A+ 轮 15 亿元，三个月累计接近 50 亿元 | Physical AI、VLA、数据金字塔、低成本采集 | 把大规模真实场景数据和学习算法作为核心资产，押注机器人模型的规模化迭代 |
| 智平方 AI² Robotics | 2026 年 2 月 B 轮系列融资超 10 亿元 | GOVLA 具身大模型、模型-硬件-场景飞轮 | 强调真实场景和产业客户反馈，让模型能力随部署扩大持续更新 |
| 灵心巧手 Linker Hand | 2026 年 2 月 B 轮近 15 亿元；4 月 B+ 轮未披露金额，市场有估值传闻 | 灵巧手、技能库、真机强化学习、Linker Agents | 为具身 Agent 提供末端执行、技能数据和真机 RL 基础设施 |
| 光轮智能 Lightwheel | 2026 年 6 月官方披露新一轮融资；金额未披露，媒体称 A++/A+++ 合计约 10 亿元 | 物理 AI 数据、仿真合成数据、模型评测、部署反馈闭环 | 更接近 reward/eval infrastructure，可服务机器人、自动驾驶和具身模型训练 |
| Flowith | 2026 年 3 月种子轮和种子+轮累计千万美元级 | Agentic OS、FlowithOS、Oracle、长程任务、自我规划/纠偏 | 国内少数偏软件 Agent 自我迭代路线的公司，重点在行为轨迹、任务拆解和云端长程执行 |
| MemoraX AI / 忆纪元 | 2026 年 4 月种子轮千万美元级；L2F 光源创业者基金、钟鼎资本等参与 | Agentic RL、内生记忆、动态学习与跨场景复用 | 直接把“记忆”和持续学习作为智能体自我更新的核心模块 |
| 中数睿智 | 2026 年 4 月 B 轮亿元级融资 | 企业级智能体操作系统、动态本体自进化、RL + Reflection | 面向企业流程自动化，强调多智能体自生成、自优化和可交付的 Agent OS |
| 云雁九宸 VArray | 2026 年 4 月天使轮千万级人民币 | 企业 Agentic OS、白盒决策链、可审计执行日志 | 把企业现场数据和可解释执行链作为后续模型/Agent 迭代数据 |
| K2 Lab | 2026 年 4 月天使轮数千万元 | AI 内容电商 Agent OS、A2A 原生工作流、任务编排和执行验证 | 垂直行业 Agent OS，适合作为长程执行与业务 reward 闭环样本 |

总体看，国内的“自我进化”并不主要表现为直接训练一个会做 AI 研究的模型，而是表现为三类工程闭环：第一，机器人和物理 AI 通过真实世界数据、仿真和强化学习不断更新；第二，Agentic OS 通过任务轨迹、执行日志和业务反馈积累可训练数据；第三，数据/评测平台把部署反馈变成 reward 和 eval。对 Scientific MA 而言，光轮智能、MemoraX AI、Flowith、中数睿智这类公司更接近“reward ledger + agent workflow + eval layer”的可借鉴对象；具身智能公司则提示真实世界 reward 的资本价值正在快速上升。

---

## 5. 目标用户与商业切入

### 5.1 目标用户定义

如果进入 AI4AI / AI4Sci 方向，目标用户不应定义为“所有想用 AI 的科学家”，而应定义为：

> 已有真实研发任务、真实实验反馈和高价值失败数据，但缺少能力把科研过程结构化为可评估、可审计、可训练数据飞轮的 discovery team。

第一阶段最合适的 ICP 是：

> 20-200 人规模，已有 wet-lab 或稳定 CRO/organ-chip 合作，正在做 biologics / protein / antibody / binder discovery，内部有 1-5 个 computational scientist，但没有完整 AI platform team 的 biotech / discovery group。

这类团队通常不会把核心科学判断外包，但会愿意把“科研过程结构化、Agent workflow、reward ledger、评测和数据治理”这类平台能力外包或共建。

### 5.2 海外潜在用户与标杆

| 类型 | 代表公司/团队 | 判断 |
|---|---|---|
| 全栈 AI-native biologics 平台 | Generate:Biomedicines、Nabla Bio、Absci、BigHat Biosciences、LabGenius、Manifold Bio、Dyno Therapeutics | 多数会自建核心平台，更适合作为标杆/潜在合作方，而不是早期 SaaS 客户 |
| AI-first drug discovery 平台 | Recursion、Xaira、Genesis Therapeutics、Terray Therapeutics、Enveda、Exscientia | 具备较强内部 AI/自动化团队，适合学习其组织形态和数据飞轮 |
| 大药企 discovery group | J&J、Sanofi、AstraZeneca、Almirall、Novo Nordisk、LG Chem 等与外部 AI-biotech 有合作的团队 | 有预算和真实任务，但销售周期长，更适合作为中后期企业级客户 |
| Organ-chip / phenotypic screening 平台 | MIMETAS、CN Bio、Vivodyne 等 | 具备高价值 phenotype reward，适合作为 reward factory 合作方 |

海外市场的核心启发是：即使大药企和成熟 biotech 有内部 AI 团队，它们仍会与 BigHat、Absci、LabGenius、Cradle 等外部平台合作，因为外部平台提供的是特定 workflow、数据生产能力和产品化基础设施，而不是简单替代内部 AI 团队。

### 5.3 中国国内目标用户分层

#### A. 最优先 ICP：中小型生物药 / 蛋白设计 / 抗体发现团队

这类团队通常拥有真实项目和实验反馈，但内部 AI platform 能力不足。它们最可能为“secure scientific memory + reward compiler + agent workflow layer”付费。

| 目标类型 | 国内代表 | 为什么适合 |
|---|---|---|
| 抗体、双抗、ADC、蛋白药物创新团队 | 复宏汉霖、百奥泰、君实生物、三生制药、迈威生物、康诺亚、泽璟制药等 | 有 biologics discovery、候选筛选、CMC/developability 和实验反馈，适合从单项目 pilot 切入 |
| ADC / 双抗 / 大分子管线密集公司 | 康方生物、荣昌生物、科伦博泰、信达生物、恒瑞医药、百济神州等 | 管线复杂、项目多、专家 review 密集，但企业级销售周期较长，更适合 lighthouse customer |
| 新型蛋白 / binder / 酶工程团队 | 合成生物、工业酶、功能蛋白、细胞因子、递送载体相关团队 | 每轮设计-实验-复盘都可形成训练信号，适合建设 Target-to-Binder / Design-Build-Test-Learn 闭环 |
| 小型 AI + wet-lab discovery 团队 | 具备少量 computational scientist 和实验协作资源的早期公司 | 自建平台成本高，愿意采购可插拔 workflow、数据治理和评测工具 |

对这类客户，第一版产品不宜包装为“大而全 AI 科研平台”，而应以具体任务进入：

- Target-to-Binder 项目记忆与候选追踪；
- 抗体/蛋白设计轮次复盘；
- assay result 与候选设计归因；
- expert review rubric 和 decision log；
- 下一轮设计建议与实验队列生成。

#### B. 企业级试点客户：大型创新药和生物药公司

大型药企和上市 biotech 通常有预算、数据和项目，但采购周期长、合规要求高、内部系统复杂。它们适合做企业级 lighthouse pilot，而不是最早期产品验证。

| 公司/类型 | 适配场景 | 切入建议 |
|---|---|---|
| 信达生物、康方生物、荣昌生物、科伦博泰、百济神州、恒瑞医药 | ADC、双抗、肿瘤免疫、抗体药物、蛋白药物 discovery | 以单个 discovery program 或单条管线做私有化 pilot |
| 复星医药/复宏汉霖、君实生物、百奥泰、三生制药 | 抗体、单抗/双抗、生物类似药和创新生物药 | 从候选筛选、实验复盘、CMC developability 评估切入 |
| CRO/CDMO 和一体化研发服务平台 | 药明生物、药明康德、康龙化成、泰格医药等 | 不一定是第一客户，但可能成为 workflow/reward data 合作伙伴 |

这类客户最关注：

- 数据不出域；
- 不用于训练其他客户模型；
- 权限、审计和合规；
- 与 ELN、LIMS、SDMS、Benchling、内部知识库、计算平台集成；
- 能否对项目周期、实验轮次、失败复用率产生明确提升。

#### C. 标杆/潜在合作/潜在竞品：国内 AI4S 与 AI 制药公司

这些公司更可能自建核心平台，但也可能在特定垂直模块上合作。它们应被视为标杆、生态伙伴或竞品，而不是默认客户。

| 公司/机构 | 公开方向 | 与我们的关系 |
|---|---|---|
| 深势科技 DP Technology | 科学大模型、药物/材料研发软件、微尺度工业基础设施 | AI4S 平台标杆，部分方向竞品，部分工具可集成 |
| 晶泰科技 XtalPi | AI + 自动化实验 + 药物发现平台 | 全栈 TechBio 标杆，更可能自建 |
| 英矽智能 Insilico Medicine | 生成式 AI 药物研发平台 | AI 制药标杆，偏小分子和临床管线 |
| 百图生科 BioMap | 生命科学大模型、蛋白/抗体/细胞治疗相关能力 | AI 生命科学基础模型标杆，可能是模型或生态合作方 |
| 星亢原 neoX Biotech | AI 生物大分子、多特异性药物设计 | 与 Target-to-Binder / biologics workflow 高度相关 |
| 分子之心 MoleculeMind | AI 蛋白质设计、蛋白/抗体生成设计平台 | 蛋白设计模型与工具标杆 |
| 百奥几何 BioGeometry | 生成式 AI 蛋白质设计 | 蛋白设计方向潜在竞品/合作方 |
| 望石智慧 StoneWise、剂泰医药 METiS、冰洲石 Accutar 等 | AI 药物研发、小分子、ADMET、生成式设计 | 部分可作为 workflow 或数据接口生态 |

对这些公司，差异化不应是“我们也有模型”，而是：

- 支持 bring-your-own-model；
- 把模型输出、专家 review、实验结果和下一轮设计串成可训练轨迹；
- 给其客户或内部项目提供 scientific memory / reward ledger / eval layer。

#### D. Reward factory 合作方：类器官、器官芯片、表型筛选和实验平台

这类公司未必直接购买完整 Agent 平台，但可提供极高价值的 phenotype reward，是 AI4Sci 闭环的关键合作对象。

| 类型 | 国内代表 | 合作价值 |
|---|---|---|
| 器官芯片 / 类器官芯片平台 | 大橡科技、丹望医疗、耀速科技/Xellar、博奥生物相关平台等 | 提供人体相关 phenotype、toxicity、efficacy reward |
| 高通量表型筛选平台 | 细胞模型、类器官、影像组学、功能读出平台 | 把表型 readout 接入候选设计闭环 |
| CRO / 预临床实验服务 | 药效、毒理、PK/PD、细胞功能实验服务商 | 作为标准化实验结果和失败数据来源 |
| 自动化实验室 / 合成生物平台 | 高通量构建、表达、纯化、酶活测试平台 | 支撑 Design-Build-Test-Learn 数据飞轮 |

这一类伙伴的价值在于让产品从“科研 Copilot”变成“带真实 reward 的科研进化系统”。

### 5.4 为什么客户会买，而不是完全自建

客户会自建核心模型和核心科学判断，但不一定愿意从零自建全套科研 Agent 基础设施。主要原因包括：

1. **交叉能力稀缺**：同时懂 protein design、wet-lab workflow、数据工程、LLMOps、Agent runtime、安全合规、ELN/LIMS 集成的人才很少。
2. **内部平台建设周期长**：一个 discovery program 的窗口可能只有 6-18 个月，自建平台可能赶不上项目节奏。
3. **内部 AI 团队资源有限**：大多数内部 AI 团队会优先做模型、pipeline 和项目支持，不会优先做实验失败归因、专家 review capture、reward normalization 和 Agent trace。
4. **产品化基础设施有复用价值**：权限、审计、状态机、trace、eval、数据 lineage、human-in-the-loop、版本管理等不是单个项目特有能力。
5. **外部平台可降低组织摩擦**：科学家继续做核心决策，平台把过程变成可复盘、可评测、可训练的组织资产。

### 5.5 数据安全与部署要求

数据泄露会是国内外客户的第一顾虑，尤其涉及 target、sequence、assay result、negative data、unpublished biology、patient-derived organoid/organ-chip data 和项目决策逻辑。因此产品必须从第一天支持：

- **No-training-by-default**：客户数据默认不用于训练通用模型或其他客户模型；
- **Dedicated tenant / VPC / 私有化部署**：SaaS 只适合轻量客户，企业客户需要专属环境；
- **Bring-your-own-model**：允许客户使用内部模型、私有模型或指定外部模型；
- **数据分级与最小权限**：target、sequence、assay、patient-derived data、项目决策分级管理；
- **全链路 audit log**：谁看过、改过、导出过、调用过模型，都可追踪；
- **加密与密钥管理**：静态和传输加密，必要时支持客户自管密钥；
- **可删除、可隔离、可迁移**：满足项目终止、合作变更和合规审计要求；
- **不跨客户混训**：跨客户学习只能沉淀为抽象 workflow、schema、rubric 和非敏感 best practice。

### 5.6 我们相对自建和通用工具的独特优势

| 选项 | 优点 | 缺口 | 我们的差异化 |
|---|---|---|---|
| 通用 Codex / Claude Code / coding agent | 强代码能力、工具调用、开发体验成熟 | 不理解科研任务状态机、实验 reward 和湿实验失败归因 | 在通用 Agent 之上提供 scientific workflow、memory、reward 和 eval |
| ELN / LIMS / SDMS | 记录实验和样本数据 | 通常不记录为什么做、为什么失败、下一轮如何训练 Agent | 把实验结果、专家判断和设计轨迹编译成训练资产 |
| 内部自建 AI 团队 | 最懂内部数据和科学目标 | 建设慢、工程化和产品化成本高 | 提供可插拔基础设施，客户保留模型、数据和 IP |
| AI 蛋白/药物设计模型公司 | 可能有强模型 | 容易绑定单一模型或服务流程 | Bring-your-own-model，关注跨模型、跨实验、跨团队的数据飞轮 |
| CRO / 实验平台 | 有实验执行能力 | 实验结果通常不回流为可训练的 Agent trajectory | 把 CRO/organ-chip/assay 结果接成 reward ledger |

产品的独特定位应是：

> Secure Scientific Memory + Reward Compiler + Agent Workflow Layer for AI-native discovery teams.

换言之，客户保留数据、模型和核心科学判断；我们提供让科研组织“越做越聪明”的底层系统。

---

## 6. 关键趋势判断

### 6.1 AI 编程是 AI4AI 的第一个杀手级应用

AI 编程工具已经经历三阶段：

1. **补全阶段**：Tabnine、早期 Copilot、Codeium 等，核心价值是节省打字和样板代码时间。
2. **对话式 IDE 阶段**：Cursor、Claude Code、Copilot Chat、Gemini Code Assist 等，核心价值是 repo 级代码理解和多文件修改。
3. **异步软件工程 Agent 阶段**：OpenAI Codex、Devin、Copilot coding agent、Jules、Replit Agent 等，核心价值是把 issue、PR、测试、重构、迁移变成可委托任务。

长期看，AI 编程会成为 AI4AI 的最大数据飞轮之一：代码任务有清晰目标、测试反馈、review 信号、错误轨迹和可执行环境，非常适合训练更强的 Agent。

### 6.2 LLMOps 的核心从“模型管理”转向“行为管理”

传统 MLOps 管模型版本、数据集、训练参数和部署流水线。LLMOps/AgentOps 更关注：

- Agent trajectory 是否可追踪；
- prompt 和工具调用是否可回归测试；
- LLM-as-judge 是否稳定；
- 成本、延迟和质量如何同时优化；
- 哪些失败可以变成下一轮训练数据；
- 生产系统是否存在 hallucination、越权、隐私泄露和安全风险。

因此，eval、trace、observability、guardrails 和 feedback loop 是未来平台的核心。

### 6.3 数据竞争从“量”转向“稀缺高质量反馈”

通用互联网数据的边际价值下降后，AI4AI 数据竞争转向：

- 专家偏好数据；
- 长链推理轨迹；
- 软件工程任务轨迹；
- 科学实验失败和成功记录；
- 机器人/自动驾驶物理交互数据；
- 合成数据与真实验证数据的闭环。

Scale AI、Mercor、Snorkel、Labelbox、NVIDIA Cosmos、Data-Juicer、光轮智能等都体现了这一趋势。

### 6.4 算力层正在纵向整合

AI 云不再只是卖 GPU 时长，而是向上整合：

- 模型训练平台；
- 推理服务；
- GPU 调度；
- 数据/实验管理；
- eval/observability；
- 开发者工具和企业治理。

CoreWeave 收购 W&B 是典型信号。未来 AI infra 的竞争不是“谁有更多卡”，而是“谁能让单位 token、单位实验、单位 Agent 任务的成本更低、质量更高、反馈更快”。

### 6.5 安全评测会成为 AI4AI 的刚性环节

随着模型具备代码生成、工具调用、长期任务执行和自我改进能力，“AI 能否安全地改进 AI”成为核心治理问题。METR 的长任务能力评估、NIST/UK AISI 的前沿模型安全评测、MLCommons AILuminate 的风险基准、EU GPAI Code 都在构建外部约束。

### 6.6 AI for Science 是 AI4AI 的高壁垒延展

AI for Science 不只是应用 AI 到科学，也会反哺 AI 研发：

- 自动发现更高效算法；
- 自动设计实验和验证假设；
- 用科学数据训练多模态推理模型；
- 用真实实验 reward 训练科研 Agent；
- 把失败实验和专家判断沉淀为高价值数据。

DeepMind AlphaEvolve、Microsoft Discovery、Sakana AI Scientist、FutureHouse、上海 AI Lab Intern-Discovery、深势科技等都值得持续跟踪。

### 6.7 AI 自我迭代从研究命题进入资本窗口

2026 年 Q1 以来，Recursive Superintelligence、Ineffable Intelligence、Ricursive Intelligence、Mirendil、General Intuition、AMI Labs 等公司获得大额早期融资，说明资本市场开始把“AI 是否能改进 AI”从长期研究命题当成可下注的公司形态。

这批融资不是简单投“更大模型”，而是投四种闭环假设：

- **AI 自动化 AI 研究**：Recursive Superintelligence、Mirendil 试图让 Agent 参与模型、算法、代码和实验流程，目标是提高 AI lab 的研究吞吐。
- **经验驱动强化学习**：Ineffable Intelligence 以 David Silver 为核心，强调从环境交互中学习，而不是继续依赖人类文本和模仿数据。
- **训练环境与评测基础设施**：Deeptune、AfterQuery、Prime Intellect 把环境、可验证任务、rollout、grader 和 eval 变成 AI lab 的生产资料。
- **世界模型与物理反馈**：AMI Labs、General Intuition、Periodic Labs 以及中国的极佳视界、星海图、千寻智能、自变量机器人等，把游戏、机器人、物理实验和真实部署反馈变成可训练经验。

因此，AI4AI 的竞争正在从“谁有更强工具”升级为“谁拥有可扩展的经验生产系统”。如果某个系统能稳定地产生任务、行动、反馈、评测、修正和再训练轨迹，它就可能成为下一代模型能力提升的基础设施。

### 6.8 强化学习的新信号：从偏好对齐转向环境学习

David Silver 创办 Ineffable Intelligence 是 2026 年强化学习路线的热点事件起点。其核心观点是：语言模型主要学习人类知识的沉积物，而通向更强智能的路径应是让 Agent 在环境中行动、试错、获得反馈，并从自身经验中发现知识。

围绕这一事件，可以看到 2026 年 Q1 以来几条清晰信号：

- **RLHF 之后是 RLVR / verifier reward**：数学、代码、工具调用、浏览器操作和多步任务可以用测试、规则、grader 或环境状态给出更客观奖励。
- **环境成为稀缺资产**：训练 Agent 不只需要数据集，还需要可执行环境、任务生成器、沙盒、状态记录和自动评分。
- **长程 rollout 成为系统工程问题**：多轮工具调用、浏览器使用、代码修改和真实工作流会产生大量轨迹，训练系统必须处理异步 rollout、失败回放、成本控制和安全边界。
- **安全也需要 RL**：当 Agent 能通过强化学习变强时，诚实、可纠正、透明、拒绝越权、避免 reward hacking 等行为也需要被设计成可训练和可评测的 reward。
- **物理世界是更高价值的 reward source**：机器人、自动驾驶、材料实验、蛋白设计和器官芯片的反馈比通用文本偏好更稀缺，也更可能形成垂直壁垒。

对 Scientific MA 来说，这意味着“Scientific Memory + Reward Ledger + Agent Workflow Layer”不是普通项目管理工具，而是面向科研 Agent 自我改进的训练基础设施：每个假设、候选设计、专家 review、实验 readout、失败归因和下一轮决策，都应被结构化为可回放、可评分、可学习的 trajectory。

---

## 7. 对 AI4Sci / Scientific MA 的启发

结合现有 AI4Sci proposal，AI4AI 产业调研对 Frontis Science Horizon 的启发如下：

1. **不要把 AI4Sci 做成单点 Copilot**。市场上通用 Copilot 会快速商品化，长期壁垒应来自真实科研任务轨迹、实验 reward、专家反馈和组织记忆。
2. **Scientific Memory 是关键资产**。行业正在从 prompt 工具走向可追踪、可评测、可训练的 Agent trajectory。科研场景应优先沉淀假设、证据、候选、实验、失败、review 和决策。
3. **Reward Ledger 比单个模型更重要**。蛋白设计、器官芯片、binding assay、toxicity、phenotype readout 都应作为可审计 reward，而不是散落在实验记录里。
4. **评测体系需要先行**。参考 OpenCompass、METR、MLCommons、Braintrust、LangSmith 等，科研 Agent 应有任务级 benchmark、专家 rubric、cost/latency/safety 指标和回归测试。
5. **数据闭环决定壁垒**。外部模型和 Agent 框架可以采购或接入，但真实科研失败轨迹、wet-lab feedback 和专家偏好很难复制。
6. **第一场景应聚焦可验证闭环**。Target-to-Binder + organ-chip phenotype reward 是合理 wedge，因为它同时具备长链任务、专家判断、计算验证和真实实验反馈。
7. **不要只卖 Agent，要卖可训练环境**。Ineffable、Prime Intellect、Deeptune、AfterQuery 的共同信号是：高价值不只在 Agent 本身，而在能让 Agent 反复试错、评分、回放和改进的 environment/eval/reward infrastructure。科研场景应优先把 assay、organ-chip、expert review 和决策 rubric 产品化为训练环境。

---

## 8. 风险与不确定性

| 风险 | 说明 | 应对思路 |
|---|---|---|
| 算力成本和供应波动 | GPU/ASIC、能源和数据中心投入巨大，客户集中度高 | 避免重资产早期投入，优先抽象可迁移的训练/推理接口 |
| AI 编程工具价格战 | 基础模型厂商、IDE 厂商和云厂商同时下场 | 不直接做通用 coding 工具，聚焦科研任务状态机和领域数据 |
| Benchmark 被刷题 | 通用评测会迅速被优化，失去区分度 | 建立私有、动态、任务真实的科研 eval |
| 数据版权和隐私 | 训练数据、文献、实验数据和患者相关数据有合规风险 | 数据 lineage、权限、审计和脱敏机制前置 |
| 合成数据失真 | 合成数据可能放大偏差，不能替代真实验证 | 合成数据只作为候选生成和覆盖长尾，必须接入 wet-lab/专家验证 |
| Agent 安全与越权 | 工具调用、代码执行和自动实验设计有安全边界 | sandbox、human-in-the-loop、权限分级和审批协议 |
| 中国生态国际影响力不足 | 国产评测和开源项目在全球中立性上仍需加强 | 国内外 benchmark 双轨，保留对国际开源标准的兼容 |

---

## 9. 建议持续跟踪清单

### 全球

- **算力/云**：NVIDIA、CoreWeave、Lambda、Crusoe、Cerebras、Groq、Together AI、Fireworks、Baseten、Modular。
- **AI 编程**：OpenAI Codex、Claude Code、GitHub Copilot、Cursor、Devin、Replit、Lovable、Vercel v0、Bolt、Augment、Sourcegraph/Amp。
- **Agent/LLMOps**：LangChain/LangGraph/LangSmith、LlamaIndex、CrewAI、Arize、Braintrust、Langfuse、Galileo、W&B/Weave、Datadog。
- **数据**：Scale AI、Snorkel、Labelbox、Mercor、Databricks、Snowflake、Hugging Face、NVIDIA Cosmos、Gretel、Mostly AI。
- **AI 自我迭代/Agentic RL**：Recursive Superintelligence、Ineffable Intelligence、Ricursive Intelligence、Mirendil、Deeptune、AfterQuery、Prime Intellect、General Intuition、AMI Labs、Periodic Labs、Core Automation。
- **科研/安全**：Google DeepMind、OpenAI、Anthropic、Microsoft Research、Sakana AI、FutureHouse、METR、NIST CAISI、UK AISI、MLCommons、EU AI Office。

### 中国

- **云与基础设施**：华为昇腾/华为云、阿里云 PAI、百度智能云、火山引擎、腾讯云、商汤 SenseCore。
- **AI 编程/Agent**：通义灵码、百度 Comate、Trae、MarsCode、华为 CodeArts、腾讯 CodeBuddy、CodeGeeX、DeepSeek Coder、Dify、MetaGPT。
- **评测/开源**：上海 AI Lab/OpenCompass/OpenMMLab/InternLM、智源/FlagEval/FlagOpen、ModelScope、SuperCLUE、信通院。
- **数据/合成数据**：海天瑞声、数据堂、Testin 云测、龙猫数据、整数智能、Data-Juicer、光轮智能、51Sim、卓印智能。
- **自我进化/具身世界模型/Agentic OS**：自变量机器人、星海图、极佳视界、千寻智能、智平方、灵心巧手、Flowith、MemoraX AI、云雁九宸、中数睿智、K2 Lab。
- **AI4Sci**：上海 AI Lab Intern-Discovery、深势科技、北京科学智能研究院、北大科学智能学院、清华 AIR、中科院相关团队。

---

## 10. 参考来源

### 算力、云与推理

- [NVIDIA TensorRT-LLM](https://developer.nvidia.com/tensorrt-llm)
- [NVIDIA Run:ai](https://blogs.nvidia.com/blog/runai/)
- [NVIDIA Cosmos](https://www.nvidia.com/en-us/ai/cosmos/)
- [CoreWeave completes acquisition of Weights & Biases](https://www.coreweave.com/blog/coreweave-completes-acquisition-of-weights-biases)
- [Lambda raises over $1.5B](https://lambda.ai/blog/lambda-raises-over-1.5b-from-twg-global-usit-to-build-superintelligence-cloud-infrastructure)
- [Together AI Series B](https://www.together.ai/blog/together-ai-announcing-305m-series-b)
- [Fireworks AI Series C](https://fireworks.ai/blog/series-c)
- [vLLM Production Stack](https://vllm.ai/blog/2025-01-21-stack-release)
- [SGLang GitHub](https://github.com/sgl-project/sglang)
- [Modular MAX/Mojo financing](https://www.modular.com/blog/modular-raises-250m-to-scale-ais-unified-compute-layer)

### AI 编程与 Agent

- [GitHub Copilot](https://github.com/features/copilot)
- [GitHub Agent HQ](https://github.blog/news-insights/company-news/welcome-home-agents/)
- [OpenAI Codex App](https://openai.com/index/introducing-the-codex-app/)
- [OpenAI Codex GA](https://openai.com/index/codex-now-generally-available/)
- [Anthropic Claude Code GA](https://www.anthropic.com/news/claude-4)
- [Anthropic Model Context Protocol](https://www.anthropic.com/news/model-context-protocol)
- [Cursor Series D](https://cursor.com/blog/series-d)
- [Cognition Devin](https://devin.ai/)
- [Cognition acquires Windsurf](https://cognition.ai/blog/windsurf)
- [Replit Agent](https://replit.com/agent4)
- [Lovable Series B](https://lovable.dev/blog/series-b)
- [Vercel v0](https://v0.app/)
- [AWS Q Developer](https://aws.amazon.com/q/developer/)
- [Google Jules](https://jules.google/)
- [Google ADK](https://developers.googleblog.com/en/agent-development-kit-easy-to-build-multi-agent-applications/)

### LLMOps、评测与可观测性

- [LangChain Series B](https://www.langchain.com/blog/series-b)
- [LangSmith](https://www.langchain.com/langsmith)
- [LlamaIndex Series A](https://www.llamaindex.ai/blog/announcing-our-series-a-and-llamacloud-general-availability)
- [CrewAI](https://crewai.com/)
- [Microsoft Agent Framework](https://learn.microsoft.com/en-us/agent-framework/overview/)
- [Arize AI Series C](https://arize.com/blog/arize-ai-raises-70m-series-c-to-build-the-gold-standard-for-ai-evaluation-observability/)
- [Braintrust Series B](https://www.braintrust.dev/blog/announcing-series-b)
- [Langfuse](https://langfuse.com/)
- [Galileo Series B](https://galileo.ai/blog/announcing-our-series-b)
- [W&B Weave](https://weave-docs.wandb.ai/)
- [Datadog LLM Observability](https://www.datadoghq.com/product/llm-observability/)
- [Promptfoo](https://www.promptfoo.dev/)
- [Ragas](https://docs.ragas.io/)
- [DeepEval](https://github.com/confident-ai/deepeval)

### AI 自我迭代、Agentic RL 与世界模型

- [Recursive Superintelligence emerges from stealth with $650M raise](https://tech.eu/2026/05/13/recursive-superintelligence-emerges-from-stealth-with-650m-raise/)
- [Recursive Superintelligence](https://www.recursive.com/)
- [Recursive Superintelligence: First steps toward automated AI research](https://www.recursive.com/articles/first-steps-toward-automated-ai-research)
- [Ineffable Intelligence](https://www.ineffable.ai/)
- [WIRED: David Silver's Ineffable Intelligence](https://www.wired.com/story/david-silver-ai-ineffable-intelligence-reinforcement-learning/)
- [Sequoia: Partnering with Ineffable Intelligence](https://sequoiacap.com/article/partnering-with-ineffable-intelligence-a-superlearner-for-the-era-of-experience/)
- [TechCrunch: David Silver raised $1.1B for Ineffable Intelligence](https://techcrunch.com/2026/04/27/deepminds-david-silver-just-raised-1-1b-to-build-an-ai-that-learns-without-human-data/)
- [NVIDIA: Ineffable Intelligence reinforcement learning infrastructure](https://blogs.nvidia.com/blog/ineffable-intelligence-reinforcement-learning-infrastructure/)
- [Ricursive Intelligence raises $300M Series A](https://www.prnewswire.com/news-releases/ricursive-intelligence-raises-300-million-series-a-at-4-billion-valuation-to-accelerate-ai-driven-semiconductor-design-302670061.html)
- [Felicis: Ricursive Intelligence](https://www.felicis.com/blog/ricursive-intelligence-a-step-change-on-the-path-to-agi)
- [Mirendil](https://mirendil.com/)
- [Kleiner Perkins: Mirendil](https://www.kleinerperkins.com/perspectives/mirendil-building-the-system-that-builds-systems/)
- [a16z: Investing in Deeptune](https://a16z.com/announcement/investing-in-deeptune/)
- [Deeptune](https://deeptune.com/)
- [AfterQuery: Human expertise reimagined](https://www.afterquery.com/blog/human-expertise-reimagined)
- [AfterQuery Research](https://www.afterquery.com/research)
- [Prime Intellect Lab](https://www.primeintellect.ai/blog/lab)
- [Prime Intellect general-agent](https://www.primeintellect.ai/blog/general-agent)
- [Prime Intellect: RL at 1T scale](https://www.primeintellect.ai/blog/rl-at-1t-scale)
- [General Intuition](https://www.generalintuition.com/)
- [Axios: General Intuition AI gaming](https://www.axios.com/2026/06/26/general-intuition-ai-gaming)
- [TechCrunch: Yann LeCun's AMI Labs raises $1.03B](https://techcrunch.com/2026/03/09/yann-lecuns-ami-labs-raises-1-03-billion-to-build-world-models/)
- [Hugging Face TRL v1.0](https://huggingface.co/blog/trl-v1)
- [OpenAI Reinforcement Fine-Tuning guide](https://developers.openai.com/api/docs/guides/reinforcement-fine-tuning)
- [OpenAI beneficial-trait RL](https://alignment.openai.com/beneficial-rl/)

### 数据、合成数据与 AutoML

- [Scale AI Series F](https://scale.com/blog/scale-ai-series-f)
- [Scale AI company evolution](https://scale.com/blog/scale-ai-announces-next-phase-of-company-evolution)
- [Snorkel AI Series D](https://snorkel.ai/blog/building-the-ai-data-development-platform-for-specialized-ai/)
- [Labelbox](https://labelbox.com/)
- [Databricks acquires MosaicML](https://www.databricks.com/company/newsroom/press-releases/databricks-signs-definitive-agreement-acquire-mosaicml-leading-generative-ai-platform)
- [Databricks Lilac](https://www.databricks.com/blog/lilac-joins-databricks-simplify-unstructured-data-evaluation-generative-ai)
- [Snowflake acquires TruEra](https://www.snowflake.com/en/blog/snowflake-acquires-truera-to-bring-llm-ml-observability-to-data-cloud/)
- [Hugging Face Hub](https://huggingface.co/docs/hub/en/index)
- [Gretel](https://gretel.ai/)
- [Mostly AI](https://mostly.ai/)
- [Tonic.ai](https://www.tonic.ai/)
- [Parallel Domain](https://paralleldomain.com/)
- [Google Vertex AI AutoML](https://cloud.google.com/vertex-ai/docs/training/automl-api)
- [Microsoft NNI](https://github.com/microsoft/nni)
- [H2O Driverless AI](https://h2o.ai/platform/ai-cloud/make/h2o-driverless-ai/)

### 目标用户、合作与标杆来源

- [Generate:Biomedicines](https://generatebiomedicines.com/)
- [Nabla Bio](https://www.nabla.bio/)
- [Absci Technology](https://www.absci.com/technology/)
- [BigHat Biosciences](https://www.bighatbio.com/)
- [LabGenius](https://labgeniustx.com/)
- [Recursion](https://www.recursion.com/)
- [Xaira Therapeutics](https://www.xaira.com/)
- [Manifold Bio](https://www.manifold.bio/)
- [Dyno Therapeutics Partnerships](https://www.dynotx.com/partnerships)
- [Cradle Bio Platform](https://www.cradle.bio/platform)
- [Benchling Trust](https://www.benchling.com/trust)
- [MIMETAS](https://mimetas.com/)
- [CN Bio](https://cn-bio.com/)
- [Vivodyne](https://www.vivodyne.com/)
- [Xellar Biosystems](https://www.xellar.com/)

### 科研、开源、安全与标准

- [Google DeepMind AlphaEvolve](https://deepmind.google/blog/alphaevolve-a-gemini-powered-coding-agent-for-designing-advanced-algorithms/)
- [Google DeepMind AlphaFold](https://deepmind.google/science/alphafold/)
- [Microsoft Discovery](https://azure.microsoft.com/en-us/blog/transforming-rd-with-agentic-ai-introducing-microsoft-discovery/)
- [Microsoft MatterGen](https://www.microsoft.com/en-us/research/blog/mattergen-a-new-paradigm-of-materials-design-with-generative-ai/)
- [Sakana AI Scientist](https://sakana.ai/ai-scientist/)
- [FutureHouse](https://www.futurehouse.org/)
- [Allen AI OLMo](https://allenai.org/olmo)
- [Stanford AI Index](https://hai.stanford.edu/ai-index)
- [Stanford HELM](https://crfm.stanford.edu/helm/)
- [LMArena](https://lmarena.ai/)
- [METR long-task evaluation](https://metr.org/blog/2025-03-19-measuring-ai-ability-to-complete-long-tasks/)
- [NIST CAISI](https://www.nist.gov/caisi)
- [UK AI Security Institute Frontier AI Trends](https://www.aisi.gov.uk/frontier-ai-trends-report)
- [MLCommons AILuminate](https://mlcommons.org/ailuminate/)
- [EU AI Office](https://digital-strategy.ec.europa.eu/en/policies/ai-office)

### 中国相关来源

- [阿里云 PAI](https://www.aliyun.com/product/pai)
- [阿里云百炼](https://www.aliyun.com/product/bailian)
- [通义灵码](https://lingma.aliyun.com/)
- [ModelScope](https://www.modelscope.cn/)
- [AgentScope](https://github.com/modelscope/agentscope)
- [百度千帆](https://cloud.baidu.com/product-s/qianfan_home)
- [百度 Comate](https://comate.baidu.com/zh)
- [华为云 ModelArts](https://www.huaweicloud.com/product/modelarts.html)
- [华为 CodeArts](https://codearts.huaweicloud.com/)
- [火山引擎](https://www.volcengine.com/)
- [Trae](https://www.trae.ai/)
- [MarsCode](https://www.marscode.cn/)
- [Dify](https://dify.ai/zh)
- [CodeGeeX](https://codegeex.cn/)
- [DeepSeek Coder](https://github.com/deepseek-ai/DeepSeek-Coder)
- [OpenCompass](https://opencompass.org.cn/)
- [OpenCompass GitHub](https://github.com/open-compass/opencompass)
- [上海人工智能实验室](https://www.shlab.org.cn/)
- [Intern-Discovery](https://discovery.intern-ai.org.cn/)
- [北京智源人工智能研究院](https://www.baai.ac.cn/)
- [FlagEval](https://flageval.baai.ac.cn/)
- [Data-Juicer](https://github.com/datajuicer/data-juicer)
- [海天瑞声](https://www.speechocean.com/)
- [数据堂](https://www.datatang.com/)
- [Testin 云测](https://www.testin.cn/)
- [深势科技](https://www.dp.tech/)
- [晶泰科技 XtalPi](https://www.xtalpi.com/)
- [英矽智能 Insilico Medicine](https://insilico.com/)
- [百图生科 BioMap](https://www.biomap.com/)
- [星亢原 neoX Biotech](https://www.neoxbiotech.com/)
- [分子之心 MoleculeMind](https://www.moleculemind.com/)
- [百奥几何 BioGeometry](https://www.biogeom.com/zh/)
- [信达生物 Pipeline](https://www.innoventbio.com/product-pipeline)
- [康方生物 Pipeline](https://www.akesobio.com/en/pipeline)
- [荣昌生物 Pipeline](https://www.remegen.com/pipeline)
- [复宏汉霖 Pipeline](https://www.henlius.com/en/Products)
- [君实生物 Pipeline](https://www.junshipharma.com/en/pipeline)
- [北京科学智能研究院](https://www.aisi.ac.cn/)
- [北大科学智能学院](https://ai4s.pkusz.edu.cn/)
- [投资界：自变量机器人 A++ 轮融资 10 亿元](https://news.pedaily.cn/202601/559733.shtml)
- [36氪：星海图完成 10 亿元 B 轮融资](https://36kr.com/p/3678199520846464)
- [证券时报：星海图完成 20 亿元 B+ 轮融资](https://www.stcn.com/article/detail/3722811.html)
- [36氪：极佳视界完成 10 亿元 B2 轮融资](https://36kr.com/p/3859841488180487)
- [中关村科学城：极佳视界完成新一轮融资](https://www.ncsti.gov.cn/kjdt/yqdy/yqdt/202604/t20260416_244087.html)
- [21 财经：千寻智能连续两轮融资近 20 亿元](https://www.21jingji.com/article/20260224/herald/37b0862cfae4d90c1bfbd024d3fe4c13.html)
- [投资界：千寻智能 A+ 轮融资 15 亿元](https://news.pedaily.cn/202606/564786.shtml)
- [量子位：智平方完成 B 轮系列融资](https://www.qbitai.com/2026/02/382004.html)
- [证券时报：灵心巧手完成近 15 亿元 B 轮融资](https://www.stcn.com/article/detail/3641823.html)
- [证券时报：灵心巧手完成 B+ 轮融资](https://www.stcn.com/article/detail/3877371.html)
- [中关村科学城：光轮智能完成新一轮融资](https://www.ncsti.gov.cn/kjdt/scyq/zgckxc/zgcdt/202606/t20260601_248418.html)
- [智东西：Flowith 完成千万美元级种子轮及种子+轮融资](https://zhidx.com/p/537762.html)
- [36氪欧洲：MemoraX AI 完成千万美元种子轮融资](https://eu.36kr.com/zh/p/3785834045583875)
- [新华网：中数睿智完成 B 轮融资](https://www.news.cn/tech/20260427/34e2c8e0b5c44c13a29d21a1465bb0dd/c.html)
- [新华网：云雁九宸完成天使轮融资](https://www.xinhuanet.com/tech/20260424/74b99a7a974649ed892e69bbfc29669f/c.html)
- [新华日报：K2 Lab 获数千万元天使轮融资](https://www.xhby.net/content/s69e05112e4b016f79cfdce14.html)
