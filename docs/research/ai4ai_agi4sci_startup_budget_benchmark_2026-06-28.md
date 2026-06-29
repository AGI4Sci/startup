# AI4AI / AGI4Sci 头部创业公司资源预算与 HC 对标

**调研日期**：2026-06-28
**用途**：为 `site/index.html` 中“所需资源支持”提供创业公司口径的预算、HC、算力、API、存储、科学软件、湿实验验证对标。
**口径说明**：公开资料很少披露单个部门预算。本文用头部 AI4AI / AGI4Sci / AI4Bio 创业公司的融资、团队规模、平台形态、实验设施和公开云价做推断。文中“事实”来自公开资料，“推断”为基于公开事实的预算判断。

---

## 0. Executive Summary

不建议用字节、阿里、腾讯、京东等大厂 AI 基建预算直接对标 AI4AI / AI4Sci 第一阶段资源。大厂资本开支是集团级、云基础设施级，而当前更合适的参照是头部 AI4AI / AGI4Sci / AI4Bio 创业公司的第一年部门预算。

推荐把第一年资源分成三档：

| 档位 | 适合阶段 | 年度总预算含薪酬 | 典型 HC | 常态 GPU | 峰值 GPU | 说明 |
|---|---|---:|---:|---:|---:|---|
| 保守档 | 先做平台、数据、agent workflow、少量 wet validation | 约 400-1,100 万美元 | 8-12 FTE + 2-4 实习 | 8-16 H200 等效卡 / 月 | 32-64 H200 等效卡 / 月 | 适合 pre-seed / seed 验证，不适合承担关键 foundation model 训练 |
| 标准档 | 头部创业公司第一年部门配置 | 约 1,500-4,500 万美元 | 20-35 FTE + 5-10 实习 | 40-80 H200 等效卡 / 月 | 160-320 H200 等效卡 / 月 | 适合 1-2 条真实项目闭环 + 1 个关键 ML benchmark |
| 进取档 | 已有 3 亿美元级融资，承担自研模型 + wet-lab 闭环 | 约 6,000-17,000 万美元 | 50-90 FTE + 10-20 实习 | 160-320 H200 等效卡 / 月 | 512-1,024 H200 等效卡 / 月 | 接近 Lila / Periodic / Xaira 式重资产路径 |

如果只按头部创业公司对标，本项目第一阶段可以采用标准档偏中位。但结合本项目当前更现实的组织节奏、客户验证和预算约束，页面默认建议采用 **5200 万元人民币 / 年验证版**：

- 全职员工：6 FTE；
- 实习生 / 访问学生：10-14 HC；
- GPU：常态约 64 张 H200 等效卡 / 月，峰值约 128-160 张 H200 等效卡 / 月；
- 模型 API：800 万人民币 / 年；
- 存储：80-150TB 热数据、50-100TB scratch / feature store、0.5-1.5PB 对象 / 归档；
- 科学软件 / 数据库：300 万人民币 / 年；
- Wet-lab 验证：1000 万人民币 / 年；
- 顾问、IP 和合作成本：不单列预算，必要工作并入全职团队职责、实验项目合同或数据库 / 软件采购；
- 含薪酬年度总预算：约 5200 万人民币 / 年。

标准档偏中位可作为第二阶段扩张口径：当付费项目、数据回流和实验验证节奏都成立，再升级到 8000 万-1.5 亿元人民币 / 年。若第一年明确要自训大型生命科学 foundation model、搭建自有自动化实验平台或同时跑多个 wet-lab 项目，则应上调到进取档。

---

## 1. 海外 AGI4Sci / AI Scientist 对标

| 公司 | 公开事实 | 团队 / 平台 / 设施 | 对预算的含义 |
|---|---|---|---|
| Lila Sciences | 2025 年 200M 美元 seed；2025 年 10 月完成 350M 美元 Series A，总融资 550M 美元。定位 scientific superintelligence 与 autonomous labs。来源：[Lila Series A](https://www.lila.ai/news/announcing-the-close-of-our-series-a)、[Flagship Pioneering](https://www.flagshippioneering.com/news/press-release/flagship-pioneering-unveils-lila-sciences-to-build-superintelligence-in-science) | 覆盖 life / chemical / materials science；强调 AI 生成假设、设计并运行实验、实时学习；官网领导层包括 CEO、CTO、Chief Robotics Officer、Chief Autonomous Science Officer。来源：[Lila Team](https://www.lila.ai/team) | 这是“AI 模型 + 自有自动化实验工厂 + 多领域平台”的重资产上限样本。若对标 Lila，预算不能只配模型团队，必须覆盖实验自动化、仪器、运维、数据工程和企业交付。 |
| Periodic Labs | 2025 年出 stealth，300M 美元 seed，目标是 create an AI scientist。来源：[TechCrunch](https://techcrunch.com/2025/09/30/former-openai-and-deepmind-researchers-raise-whopping-300m-seed-to-automate-science/)、[a16z](https://a16z.com/announcement/investing-in-periodic-labs/) | 从 physical sciences / materials 起步，官网强调 autonomous laboratories；团队背景覆盖 ChatGPT、DeepMind GNoME、OpenAI Operator、MatterGen 等。来源：[Periodic](https://periodic.com/) | 300M 美元 seed 说明顶级 AI scientist 公司会一次性前置顶尖人才、实验设施和算力预算。适合作为进取档参照。 |
| FutureHouse / Edison Scientific | FutureHouse 为 AI Scientist 非营利组织；Edison Scientific 为 2025 年商业化 spinout，获得 70M 美元 seed。来源：[FutureHouse](https://www.futurehouse.org/about)、[Edison Scientific](https://www.futurehouse.org/news/announcing-edison-scientific)、[FinSMEs](https://www.finsmes.com/2025/12/edison-scientific-raises-70m-in-seed-funding.html) | FutureHouse 在 SF Dogpatch 有约 3,000 sq ft wet lab；Edison 的 Kosmos 面向 biopharma R&D，可读文献、分析数据、生成假设并执行 workflow。来源：[Edison Kosmos](https://edisonscientific.com/) | 这是 agent-first、相对轻资产的 AI Scientist 参照。适合作为标准档下限：重点配软件、企业集成、数据和少量 wet-lab 验证。 |
| Emerald Cloud Lab | Austin 设施约 105,000 sq ft，230+ 类仪器；CMU Cloud Lab 为 40M 美元项目，基于 ECL 软件架构。来源：[ECL](https://www.emeraldcloudlab.com/)、[PRNewswire](https://www.prnewswire.com/news-releases/emerald-cloud-lab-to-relocate-state-of-the-art-facility-from-south-san-francisco-to-austin-301758704.html)、[CMU](https://www.cmu.edu/news/stories/archives/2021/august/first-academic-cloud-lab.html) | 高度自动化、远程控制 cloud lab；更像实验数据工厂，不是 AI Scientist 公司。 | 提醒自建 wet-lab factory 是高 CAPEX、高运维复杂度路线。第一阶段若不自建实验室，应通过外部 partner 网络获得 wet reward。 |
| Strateos | 2021 年 Series B 56.1M 美元；曾运营 Menlo Park 与 San Diego SmartLab Studios，200+ instruments；后转向 on-site/private cloud labs。来源：[BusinessWire](https://www.businesswire.com/news/home/20210608005436/en/Strateos-Closes-%2456-Million-Series-B-Financing-to-Accelerate-the-Roll-Out-of-its-SmartLab-of-the-Future-Platform)、[FierceBiotech](https://www.fiercebiotech.com/medtech/strateos-scores-56m-to-smarten-up-its-smartlab-platform-for-robotic-remote-r-d-work) | Remote access labs / SmartLab / lab control software；Lilly Life Sciences Studio 约 11,500 sq ft、100+ instruments。来源：[Lilly-Strateos](https://investor.lilly.com/news-releases/news-release-details/eli-lilly-and-company-collaboration-strateos-inc-launch-remote) | 说明纯 cloud lab 商业化不容易，利用率、客户定制、交付效率和资本效率都是风险。 |

---

## 2. 海外 AI4Bio / Protein / AI Drug Discovery 对标

| 公司 | 公开事实 | 团队 / 平台 / 闭环 | 对预算的含义 |
|---|---|---|---|
| EvolutionaryScale | 2024 年 seed 142M 美元；ESM3 为 98B 参数蛋白模型，训练量超过 1e24 FLOPS；LinkedIn 规模 11-50。来源：[ESM3](https://www.evolutionaryscale.ai/blog/esm3-release)、[Amazon](https://press.aboutamazon.com/aws/2024/6/evolutionaryscale-launches-with-esm3-a-milestone-ai-model-for-biology)、[LinkedIn](https://www.linkedin.com/company/evolutionaryscale) | 更像 frontier protein foundation model lab；公开信息未显示自营 wet-lab 闭环。2025 年团队加入 Biohub。来源：[Gunderson](https://www.gunder.com/en/news-insights/client-news/gunderson-client-evolutionaryscale-team-joins-biohub-in-strategic-transaction-with-chan-zuckerberg-initiative) | 说明纯模型团队可以很精干，但训练预算和云资源强度高。若本项目不自训同级别 foundation model，不应直接按 EvolutionaryScale 算力上限配置。 |
| Xaira Therapeutics | 2024 年 launch，committed capital 超 1B 美元；LinkedIn 规模 51-200。来源：[BusinessWire](https://www.businesswire.com/news/home/20240423707240/en/Xaira-Therapeutics-Launches-to-Deliver-Transformative-Medicines-by-Advancing-and-Harnessing-AI-for-Drug-Discovery-and-Development)、[LinkedIn](https://www.linkedin.com/company/xaira-therapeutics) | AI-native integrated biotech，覆盖生物理解、分子设计、数据生成和 therapeutic development；2026 发布 X-Cell。来源：[Xaira approach](https://www.xaira.com/our-approach)、[X-Cell](https://www.businesswire.com/news/home/20260317710096/en/Xaira-Therapeutics-Launches-X-Cell-Its-First-Virtual-Cell-Model-Trained-on-the-Largest-Ever-Genome-Wide-Perturbation-Dataset-X-AtlasPisces) | 最高资本强度样本。若做模型 + 数据生成 + 实验 + 临床开发全栈，百人级团队也可能需要数亿美元预算。 |
| Generate:Biomedicines | 2023 年 Series C 273M 美元，累计股权融资近 700M 美元；2026 年 IPO gross 400M 美元；公开摘要显示 2025 年末 312 employees。来源：[Generate Series C](https://generatebiomedicines.com/media-center/series-c-financing-announcement)、[Generate IPO](https://generatebiomedicines.com/media-center/generate-biomedicines-inc-announces-pricing-of-initial-public-offering)、[TradingView IPO summary](https://www.tradingview.com/news/tradingview%3A372d767ce01fc%3A0-generate-biomedicines-clinical-stage-generative-biology-company-designing-ai-engineered-protein-therapeutics-files-for-nasdaq-ipo/) | Chroma 蛋白生成模型；Generate Platform 采用 generate-build-measure-learn 闭环；Andover CryoEM lab 支撑结构数据回流。来源：[Chroma Nature](https://generatebiomedicines.com/media-center/generatebiomedicines-announces-publication-of-its-chroma-model-in-nature)、[CryoEM lab](https://generatebiomedicines.com/media-center/generatebiomedicines-unveils-state-of-the-art-cryoem-laboratory-to-accelerate-generative-ai-drug-discovery-and-development) | 成熟蛋白药物平台一旦进入临床后期，预算会向传统 biotech 靠拢。第一阶段不建议按 Generate 全公司规模配置。 |
| Cradle | 2024 年 Series B 73M 美元，累计超过 100M 美元；LinkedIn 规模 51-200。来源：[Cradle Series B](https://www.cradle.bio/blog/series-b)、[LinkedIn](https://hr.linkedin.com/company/cradlebio) | AI-powered protein engineering platform，自营 Amsterdam wet lab，模型版本 A/B test，实验 turnaround 从数月缩到数周。来源：[Cradle Lab](https://www.cradle.bio/lab) | 适合作为中低资本强度参照：软件平台 + wet-lab 数据飞轮，但不承担临床管线全成本。 |
| Genesis Molecular AI | 2023 年 Series B 200M 美元，累计超过 280M 美元；2024 年 Gilead 披露 Genesis 已融资超过 300M 美元；LinkedIn 规模 51-200。来源：[BioPharma Dive](https://www.biopharmadive.com/news/genesis-series-b-ai-drug-discovery/691348/)、[Gilead](https://www.gilead.com/news/news-details/2024/gilead-and-genesis-therapeutics-announce-strategic-collaboration-to-discover-and-develop-novel-therapies)、[LinkedIn](https://www.linkedin.com/company/genesis-molecular-ai) | GEMS 集成 language models、diffusion models、physical ML simulations；有 San Diego integrated lab。来源：[Genesis](https://www.genesis.ml/about) | 约百人级、3 亿美元级融资，是“AI + physics + 小分子管线”的中等偏重资本样本。 |
| Iambic | 2023 年 Series B 100M 美元，2024 年 extension 50M 美元，2025 年 oversubscribed round 超 100M 美元。来源：[Iambic Series B](https://www.iambic.ai/post/series-b)、[Iambic extension](https://www.iambic.ai/post/iambic-therapeutics-closes-50-million-series-b-extension-to-broaden-its-pipeline-of-ai-discovered-clinical-oncology-programs)、[Iambic 2025](https://www.iambic.ai/post/iambic-raises-over-100-million) | Enchant、NeuralPLexer；physics-informed AI + automated experimental execution，design-make-test 可达 weekly cadence。来源：[Iambic](https://www.iambic.ai/) | 进入临床后，预算核心不只是 GPU，还包括 wet lab、CMC、临床前、专利、BD 和管线管理。 |
| Insilico Medicine | 2025 年港股上市，IPO raised 22.77 亿港元；2025 年末 cash / bank balances 393.3M 美元；员工与顾问 317，其中 professionals 247。来源：[Insilico IPO](https://insilico.com/news/p010170up1-insilico-medicine-lists-on-hong-kong-sto)、[Insilico 2025 annual](https://insilico.com/news/ohz9ozx0t1-insilico-medicine-announces-2025-annual)、[annual PDF](https://newsfile.futunn.com/public/NN-PersistNoticeAttachment/7781/20260329/12075811-0.PDF) | Pharma.AI 覆盖 Biology42、Chemistry42、Science42；IPO 用途中 15% 投入新 generative AI models，12% 用于 automated lab 扩展。 | 上市 AI drug discovery 公司强参考。预算必须包含管线、BD、自动化实验和合规，不适合作为纯软件部门下限。 |

---

## 3. 国内 AI4Sci / AI Drug Discovery 对标

| 公司 | 公开事实 | 团队 / 平台 / 闭环 | 对预算的含义 |
|---|---|---|---|
| 深势科技 DP Technology | 2018 年成立，定位 AI for Science，做 AI Scientist 与 Science as a Service；2025 年 C 轮超 8 亿元；36Kr 项目库列示 2023 年 B+ 超 7 亿元、2024 年 B++ 数亿元、2025 年 C 轮超 8 亿元。来源：[DP Technology](https://www.dp.tech/)、[36Kr PitchHub](https://pitchhub.36kr.com/project/1678547907048450) | 产品矩阵包括玻尔科研空间站、勒贝格智算、Hermite、RiDYMO、Uni-Lab、SciMaster；官网强调读文献、做计算、做实验闭环。 | 国内“AI4Sci 基础设施 / 工业软件平台”参照。预算应重点配算法、HPC、数据工程、产品化和行业解决方案，wet-lab 可通过 partner 网络逐步加深。 |
| 晶泰科技 XtalPi | 2015 年成立，港股 2228.HK；上市前累计融资约 7.32B 美元；2024 年营收 2.66 亿元，研发开支 4.18 亿元；2024 年全球员工 809 人，其中全职 753 人。来源：[XtalPi annual report](https://ir.xtalpi.com/media/bdkhnvuu/2025040702144_c.pdf)、[PharmCube](https://bydrug.pharmcube.com/news/detail/0fc6bacad5554b47191848792855e59b) | 自建 AI + 机器人实验室，自动化平台每月积累 20 万+反应过程数据；有 AI 小分子、抗体结构预测、固态研发和智能机器人实验室方案。 | 国内重资产平台型上限样本。若对标晶泰，不能只配 AI 团队，还要配自动化实验设备、化学/生物/材料实验运营团队和 BD 交付团队。 |
| 百图生科 BioMap | 2020 年由李彦宏、刘维创立；两轮融资总额超 2 亿美元；BusinessWire 披露 300+ experts 国际跨职能团队；媒体曾称 200+ 员工。来源：[ChinaVenture](https://www.chinaventure.com.cn/news/80-20260321-390594.html)、[PHIRDA](https://www.phirda.com/artilce_41943.html?module=trackingCodeGenerator)、[BusinessWire](https://www.businesswire.com/news/home/20231010485897/en/BioMap-Establishes-a-Strategic-Collaboration-with-Sanofi-to-Co-Develop-AI-Modules-to-Accelerate-Drug-Discovery-for-Biotherapeutics) | xTrimo V3 为 210B 参数生命科学基础模型，覆盖蛋白质 / DNA / RNA 等模态和 200+ 任务；与 Sanofi 合作潜在总额超 10 亿美元。 | 生命科学大模型 + MaaS / 平台授权样本。预算重点在大模型训练、数据、算法科学家和行业 BD，wet-lab 用于验证与数据飞轮。 |
| 英矽智能 Insilico Medicine | 2014 年成立，2025 年港股上市，IPO 募资 22.77 亿港元；2025 年收入 5624 万美元，IPO 后 cash / bank balances 393.3M 美元；研发约 249 人，占总人数约 78%。来源：[Sina](https://finance.sina.com.cn/stock/hkstock/hkzmt/2025-11-12/doc-infxcctk5054609.shtml)、[Insilico IPO](https://insilico.com/news_sc/yv1sumnn21-aibiotech-ipo)、[Insilico annual](https://insilico.com/news/ohz9ozx0t1-insilico-medicine-announces-2025-annual) | Pharma.AI 覆盖 Biology42、Chemistry42、Science42；Life Star 1/2 自动化实验室打通计算设计到实验验证的干湿闭环；累计 28 个 PCC、10 个临床项目。 | “AI 平台 + 自研管线 + 授权交易”样本。HC 不一定最大，但临床、BD、法务、管线管理和现金储备要求高于纯软件平台。 |
| 剂泰科技 / METiS | 2019 年成立，由晶泰孵化；2022 年连续两轮融资合计 1.5 亿美元；2026 年报道累计融资超 3 亿美元；官网披露 2025 年完成 4 亿元 D 轮。来源：[PharmCube](https://www.pharmcube.com/news/wechat?esid=ed0f405dfa852a0404730e65e99f234a&tag_id=10)、[XtalPi](https://www.xtalpi.com/innovation-42/)、[21世纪经济报道](https://www.21jingji.com/article/20260421/herald/625f573d85e171125cc6ebe3a8592f98.html)、[METiS](https://metistechbio.com/) | 专注 AI 驱动药物制剂、纳米递送、LNP / mRNA 递送；结合高通量实验、AI 算法、量子化学 / 分子动力学模拟；支持 30+ 药企 / biotech 平台合作。 | 垂直环节深挖型样本。HC 可更精干，但湿实验、动物/临床前、CMC、BD 授权能力是刚性资源。 |

---

## 4. 资源预算三档模型

以下为部门预算，不是整家公司预算；薪酬单列。美元口径仅为方便与公开融资和云价对齐。

| 资源项 | 保守档 | 标准档 | 进取档 |
|---|---:|---:|---:|
| HC 全职 / 实习 | 8-12 FTE / 2-4 实习 | 20-35 FTE / 5-10 实习 | 50-90 FTE / 10-20 实习 |
| GPU H200 等效卡 / 月：常态 / 峰值 | 8-16 / 32-64 | 40-80 / 160-320 | 160-320 / 512-1,024 |
| GPU 年预算 | 0.4-1.5M 美元 | 2-7M 美元 | 8-30M 美元 |
| CPU / 内存 | 常态 0.5k-1k vCPU、2-4TB RAM；峰值 5k vCPU、16-32TB RAM | 常态 2k-5k vCPU、8-20TB RAM；峰值 20k-60k vCPU、64-200TB RAM | 常态 8k-20k vCPU、32-80TB RAM；峰值 100k-250k vCPU、0.3-1PB 分布式 RAM |
| CPU / 内存年预算 | 0.2-0.8M 美元 | 0.8-3M 美元 | 3-12M 美元 |
| 存储 | 50-150TB 热数据 + 0.5-1.5PB 对象 / 归档 | 300-800TB 热数据 + 2-8PB 对象 / 归档 | 1-3PB 热数据 + 10-30PB 对象 / 归档 |
| 存储年预算 | 0.1-0.5M 美元 | 0.5-2.5M 美元 | 2-10M 美元 |
| AI API 月预算 | 5k-30k 美元 / 月 | 50k-250k 美元 / 月 | 300k-1.5M 美元 / 月 |
| 科学软件 / 数据库 | 50k-200k 美元 / 年 | 300k-1M 美元 / 年 | 1-4M 美元 / 年 |
| Wet-lab 验证预算 | 0.5-2M 美元 / 年 | 3-10M 美元 / 年 | 15-50M 美元 / 年 |
| 资源总预算，不含薪酬 | 1.2-5M 美元 / 年 | 7-27M 美元 / 年 | 33-124M 美元 / 年 |
| 加上 loaded payroll 后 | 约 4-11M 美元 / 年 | 约 15-45M 美元 / 年 | 约 60-170M 美元 / 年 |

### 4.1 GPU / API / 训练成本参照

- H200 公共云价大致落在 3.5-5.7 美元 / GPU-hour：Nebius H200 4.50 美元，RunPod H200 4.39 美元，Crusoe H200 4.29 美元，Hyperstack H200 SXM 3.50 美元；AWS P5e / P5en H200 capacity block 在约 5 美元上下。来源：[Nebius](https://docs.nebius.com/compute/resources/pricing)、[RunPod](https://www.runpod.io/pricing)、[Crusoe](https://www.crusoe.ai/cloud/pricing)、[Hyperstack](https://www.hyperstack.cloud/gpu-pricing)、[AWS Capacity Blocks](https://aws.amazon.com/ec2/capacityblocks/pricing/)
- 1 张 H200 等效卡 / 月按 720 GPU-hour 折算。稳态混合采购可按 3.0k-4.5k 美元 / 卡月，峰值保供按 4.5k-7.9k 美元 / 卡月。
- API 参考：OpenAI、Anthropic、Gemini 均按 input / output tokens 计费，生产环境更适合用月度 API budget envelope 管理。来源：[OpenAI pricing](https://developers.openai.com/api/docs/pricing)、[Claude pricing](https://platform.claude.com/docs/en/about-claude/pricing)、[Gemini pricing](https://ai.google.dev/gemini-api/docs/pricing)
- 训练成本参照：DeepSeek-V3 报告披露全训练 2.788M H800 GPU-hours；Stanford AI Index 曾估算 GPT-4 和 Gemini Ultra 训练算力成本分别约 78M 和 191M 美元级别。来源：[DeepSeek-V3](https://arxiv.org/abs/2412.19437)、[Stanford AI Index](https://hai.stanford.edu/news/ai-index-state-ai-13-charts)、[Epoch AI trends](https://epoch.ai/trends)

---

## 5. 对本项目第一阶段预算的建议

### 5.1 推荐默认档

建议采用 **5200 万元 / 年验证版**，而不是大厂部门级，也不是头部 AI4Sci 创业公司的重资产标准档。核心假设是：第一年先验证可收费项目闭环和关键 benchmark，不自训大型 foundation model，不自建自动化 wet-lab。

| 资源项 | 推荐口径 |
|---|---:|
| 全职员工 | 6 FTE |
| 实习生 / 访问学生 | 10-14 HC |
| GPU 常态 | 约 64 张 H200 等效卡 / 月 |
| GPU 峰值 | 约 128-160 张 H200 等效卡 / 月 |
| CPU / 内存 | 常态 800-2,000 vCPU、3-8TB RAM；峰值 8,000-20,000 vCPU、24-64TB RAM |
| AI API | 800 万人民币 / 年 |
| 存储 | 80-150TB 热数据 + 50-100TB scratch / feature store + 0.5-1.5PB 对象 / 归档 |
| 科学软件 / 数据库 | 300 万人民币 / 年 |
| Wet-lab 验证 | 1000 万人民币 / 年 |
| 顾问 / IP / 合作 | 不单列预算 |
| 年度总预算，含薪酬 | 约 5200 万人民币 |

建议的预算拆分：

| 类别 | 年预算 |
|---|---:|
| 全职团队 | 1000 万人民币 |
| 实习 / 访问学生 | 500 万人民币 |
| GPU 算力 | 1100 万人民币 |
| CPU / 存储 / 调度 | 500 万人民币 |
| 模型 API | 800 万人民币 |
| 外部实验验证 | 1000 万人民币 |
| 科学软件 / 数据库 | 300 万人民币 |

### 5.2 为什么不是大厂部门口径

国内外大厂 AI 基建投入是集团级、云级或基础设施级，不适合直接用于本项目第一阶段部门预算。本项目当前更适合对标：

- Edison / FutureHouse：agent-first、轻资产、少量 wet lab；
- Cradle：软件平台 + 自营 wet lab + 蛋白工程数据飞轮；
- 深势科技：AI4Sci 平台、HPC、科学工具和行业解决方案；
- 百图生科 / EvolutionaryScale：生命科学基础模型和多模态数据；
- Lila / Periodic / Xaira：进取档上限。

### 5.3 关键假设

1. GPU 预算不含大额 egress、专线、企业支持、Kubernetes / Slurm 运维、安全合规和闲置浪费；5200 万版本应优先使用云、租赁、合作方算力和短期峰值额度。
2. H200 等效是采购预算单位，不是严格性能等价；H100、B200、spot / preemptible 可按价格和显存需求折算。
3. API 预算用于科学 agent、文献 RAG、代码、评估和部分推理，不包含大规模面向客户的生产推理。
4. Wet-lab 预算只覆盖早期验证、合成、表达、binding / cell assay 和小规模 phenotype pilot；不含大规模 omics / perturb-seq、GLP tox、IND-enabling 和临床。
5. 科学软件 / 数据库多为 quote-based，公开定价有限；这里按 Benchling、CAS、Reaxys、Cortellis、Schrodinger 等企业采购经验做区间推断。来源：[Benchling pricing](https://www.benchling.com/pricing)、[CAS SciFinder](https://www.cas.org/solutions/cas-scifinder-discovery-platform)、[Reaxys](https://www.elsevier.com/products/reaxys)、[Cortellis](https://clarivate.com/life-sciences-healthcare/cortellis/)

---

## 6. 对 `site/index.html` 的推荐写法

当前页面建议不要写“大厂对标”，也不要默认写成 Lila / Periodic 那种重资产路线，而写：

> 按本项目当前阶段，建议采用 5200 万元 / 年验证版：用小而完整的核心团队，配常态 64 张 H200，把第一年重点压到 1 条可收费项目闭环、1 个关键 ML benchmark 和必要的外部实验验证上。

页面中的拆分可以写：

> 建议拆成：全职团队 1000 万，实习 / 访问学生 500 万，GPU 算力 1100 万，CPU / 存储 / 调度 500 万，模型 API 800 万，外部实验验证 1000 万，科学软件与数据库 300 万，合计 5200 万。顾问、IP 和合作成本不单列，必要工作并入全职团队职责、实验项目合同或数据库 / 软件采购。

---

## 7. 参考来源

### AGI4Sci / AI Scientist

- [Lila Sciences Series A](https://www.lila.ai/news/announcing-the-close-of-our-series-a)
- [Flagship Pioneering unveils Lila Sciences](https://www.flagshippioneering.com/news/press-release/flagship-pioneering-unveils-lila-sciences-to-build-superintelligence-in-science)
- [Periodic Labs](https://periodic.com/)
- [TechCrunch: Periodic Labs $300M seed](https://techcrunch.com/2025/09/30/former-openai-and-deepmind-researchers-raise-whopping-300m-seed-to-automate-science/)
- [FutureHouse](https://www.futurehouse.org/about)
- [Edison Scientific](https://www.futurehouse.org/news/announcing-edison-scientific)
- [Emerald Cloud Lab](https://www.emeraldcloudlab.com/)
- [CMU Cloud Lab](https://www.cmu.edu/news/stories/archives/2021/august/first-academic-cloud-lab.html)
- [Strateos Series B](https://www.businesswire.com/news/home/20210608005436/en/Strateos-Closes-%2456-Million-Series-B-Financing-to-Accelerate-the-Roll-Out-of-its-SmartLab-of-the-Future-Platform)

### AI4Bio / AI Drug Discovery

- [EvolutionaryScale ESM3](https://www.evolutionaryscale.ai/blog/esm3-release)
- [Xaira launch](https://www.businesswire.com/news/home/20240423707240/en/Xaira-Therapeutics-Launches-to-Deliver-Transformative-Medicines-by-Advancing-and-Harnessing-AI-for-Drug-Discovery-and-Development)
- [Generate:Biomedicines Series C](https://generatebiomedicines.com/media-center/series-c-financing-announcement)
- [Generate:Biomedicines IPO](https://generatebiomedicines.com/media-center/generate-biomedicines-inc-announces-pricing-of-initial-public-offering)
- [Cradle Series B](https://www.cradle.bio/blog/series-b)
- [Genesis Series B](https://www.biopharmadive.com/news/genesis-series-b-ai-drug-discovery/691348/)
- [Iambic Series B](https://www.iambic.ai/post/series-b)
- [Insilico Medicine IPO](https://insilico.com/news/p010170up1-insilico-medicine-lists-on-hong-kong-sto)

### 中国 AI4Sci / AI Drug Discovery

- [深势科技](https://www.dp.tech/)
- [深势科技 PitchHub](https://pitchhub.36kr.com/project/1678547907048450)
- [晶泰科技 2024 年报](https://ir.xtalpi.com/media/bdkhnvuu/2025040702144_c.pdf)
- [百图生科 x Sanofi](https://www.businesswire.com/news/home/20231010485897/en/BioMap-Establishes-a-Strategic-Collaboration-with-Sanofi-to-Co-Develop-AI-Modules-to-Accelerate-Drug-Discovery-for-Biotherapeutics)
- [英矽智能 2025 年报新闻](https://insilico.com/news/ohz9ozx0t1-insilico-medicine-announces-2025-annual)
- [剂泰科技](https://metistechbio.com/)

### 算力 / API / 软件

- [AWS Capacity Blocks](https://aws.amazon.com/ec2/capacityblocks/pricing/)
- [Nebius pricing](https://docs.nebius.com/compute/resources/pricing)
- [RunPod pricing](https://www.runpod.io/pricing)
- [Crusoe pricing](https://www.crusoe.ai/cloud/pricing)
- [Hyperstack pricing](https://www.hyperstack.cloud/gpu-pricing)
- [OpenAI API pricing](https://developers.openai.com/api/docs/pricing)
- [Claude pricing](https://platform.claude.com/docs/en/about-claude/pricing)
- [Gemini API pricing](https://ai.google.dev/gemini-api/docs/pricing)
- [DeepSeek-V3 technical report](https://arxiv.org/abs/2412.19437)
- [Stanford AI Index](https://hai.stanford.edu/news/ai-index-state-ai-13-charts)
- [Epoch AI trends](https://epoch.ai/trends)
