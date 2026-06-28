# AGI 加速生命科学发现公司图谱调研报告

**调研日期**：2026-06-28  
**主题**：AGI / Agentic AI / Foundation Models 加速科学发现，聚焦生命科学、药物发现、蛋白设计、自动化实验与科研智能体  
**用途**：作为 AI4Sci / Science Agent Evolution Infrastructure 的 related work 与市场参照

---

## 0. Executive Summary

当前市场上严格意义的“AGI 独立完成科学发现”还没有被充分证明。已经开始商业化落地的是更具体的一组能力：

1. **生物基础模型**：结构预测、蛋白语言模型、分子生成、抗体设计、RNA / gene editor 设计。
2. **科研 Agent**：文献推理、假设生成、实验设计、工具调用、多 Agent 协作。
3. **自动化湿实验闭环**：机器人实验室、云实验室、高通量数据生成、实验结果反馈模型。
4. **专有数据与临床数据平台**：多组学、病理、真实世界数据、临床试验数据。
5. **药企研发工作流集成**：从单点 AI 工具进入靶点发现、DMTA、临床开发、监管、安全和商业化流程。

生命科学里的“AGI for science”正在从单模型叙事转向系统叙事：

```text
通用推理模型
  + 生物基础模型
  + 科学工具调用
  + 自动化实验
  + 专有数据
  + 专家反馈
  + 临床 / 监管工作流
  = 可持续进化的科研智能系统
```

对 AI4Sci 基础设施的启发是：壁垒不应只放在某个蛋白生成模型上，而应放在 **Scientific Memory、Trajectory、Reward、Verifier、Wet-lab Feedback、Human Expert Review** 的完整闭环上。

---

## 1. 调研口径与分类

本文将“AGI 加速科学发现”按市场可验证形态拆成五类。

| 类别 | 典型能力 | 代表公司 |
|---|---|---|
| 端到端 AI 药物发现 | 靶点发现、分子设计、虚拟筛选、自动化 DMTA、临床前管线 | Isomorphic Labs、Recursion/Exscientia、Insilico Medicine、Xaira、insitro、Schrodinger、Relay、Iambic、Genesis、Terray、Valo、XtalPi |
| 生成式生物学 / 蛋白抗体设计 | 蛋白语言模型、抗体设计、酶工程、RNA 设计、AI gene editor | Generate:Biomedicines、Absci、BigHat、Cradle、EvolutionaryScale、Profluent、Chai Discovery、Nabla Bio、LabGenius、Inceptive、A-Alpha Bio |
| AI Scientist / 自驱动实验室 | 科研 Agent、实验规划、机器人湿实验、云实验室、自动化数据生成 | Lila Sciences、FutureHouse/Edison Scientific、Emerald Cloud Lab、Strateos、Ginkgo Bioworks、Culture Biosciences、Automata、Synthace、Arctoris |
| 大厂与基础设施 | 生物模型、GPU / 云、agentic R&D 平台、数据底座、合规流程 | Google DeepMind / Isomorphic、NVIDIA BioNeMo、Microsoft Discovery、OpenAI、Anthropic、AWS HealthOmics、Oracle、Databricks、Benchling、Veeva |
| 临床数据 / 真实世界数据 / 诊断 | 多模态患者数据、病理图像、真实世界证据、临床试验优化 | Tempus AI、Owkin、PathAI、Paige、Freenome、SOPHiA Genetics |

---

## 2. 核心市场判断

### 2.1 AI 药物发现已经进入“临床和现金流验证期”

2018-2022 年左右，市场更多验证的是“AI 能不能用于发现新靶点、新分子”。2023 年之后，问题逐渐变成：

- 是否有候选药物进入临床？
- 是否有 Phase 1 / Phase 2 信号？
- 大药企是否愿意支付 upfront，而不只是承诺后端里程碑？
- 平台是否能产生持续收入？
- 失败项目是否能被系统性学习，而不是一次性归零？

代表信号：

- **Insilico Medicine** 的 rentosertib 已有 IPF Phase 2a 数据，是 AI 发现 / 设计药物临床 PoC 的代表案例之一。
- **Generate:Biomedicines** 的 AI-engineered anti-TSLP 抗体 GB-0895 已进入全球 Phase 3，是生成式蛋白药最靠近后期临床验证的案例之一。
- **Recursion + Exscientia** 的合并说明行业进入整合阶段，单一平台叙事需要规模、数据和临床管线支撑。
- **BenevolentAI** 等公司的失败提醒市场：AI 可以提高搜索效率，但不能消除临床失败、毒性、剂量、患者分层和终点设计风险。

### 2.2 自动化实验室是“AGI for science”的关键基础设施

生命科学中的 AI 系统不是只靠文献和公开数据库就能持续进化。真正稀缺的是：

- 标准化实验协议；
- 可编程仪器；
- 可复现实验轨迹；
- 高通量阴性数据；
- 专家修正；
- 实验失败原因；
- 与候选设计直接绑定的 reward。

因此，Lila Sciences、Emerald Cloud Lab、Strateos、Ginkgo Bioworks、Culture Biosciences、Automata、Synthace 等公司的价值并不只是“自动化替代人工”，而是把湿实验变成 AI 可调用、可记录、可训练的数据生产系统。

### 2.3 大厂不是传统药企，但正在成为生命科学研发操作系统的一部分

Google DeepMind、NVIDIA、Microsoft、OpenAI、Anthropic、AWS、Oracle、Databricks、Benchling、Veeva 的角色不是都去做药，而是分布在：

- 模型层；
- 算力层；
- 科学工具调用层；
- 企业研发工作流；
- 临床与监管数据平台；
- 合规与安全治理。

这意味着未来的生命科学 AI 竞争不会只是 biotech 之间竞争，也会是 biotech、云厂商、基础模型公司、药企、实验自动化平台共同构成的生态竞争。

---

## 3. 代表公司总览

### 3.1 端到端 AI 药物发现

| 公司 | 总部 / 成立 | 核心技术 | 生命科学应用 | 商业化与验证 |
|---|---:|---|---|---|
| Isomorphic Labs | 英国伦敦，2021 | AlphaFold 体系延展、多模态药物设计、AI-first drug design | 小分子、生物药、分子胶、抗体、肽 | 与 Lilly、Novartis、J&J 等药企合作；Alphabet / DeepMind 系商业化主体 |
| Recursion + Exscientia | 美国盐湖城 / 英国牛津，2013 / 2012 | 表型组学、自动化湿实验、生成化学、Recursion OS | 肿瘤、罕见病、神经、免疫 | 2024 年合并，上市公司，具备临床管线和大型药企合作 |
| Insilico Medicine | 香港 / 波士顿等，2014 | PandaOmics、Chemistry42、Pharma.AI、自动化实验 | 纤维化、肿瘤、免疫、代谢、疼痛 | rentosertib 有 IPF Phase 2a 数据；与 Lilly、SK Biopharm 等合作 |
| Xaira Therapeutics | 美国湾区，2024 | 端到端 AI 药物发现、数据生成、产品开发 | 靶点、分子、患者分层 | 以超 10 亿美元启动，临床验证仍待兑现 |
| insitro | 美国南旧金山，2018 | 遗传锚定多模态数据、机器学习疾病模型 | 神经、代谢、ALS 等 | 与 BMS 等药企合作，强调人源数据和疾病建模 |
| Schrodinger | 美国纽约，1990 | 物理计算、FEP、分子建模、ML | 小分子药物设计 | 软件收入 + 自有管线 + 药企合作，商业模式较成熟 |
| Relay Therapeutics | 美国剑桥，2016 | 蛋白动态、分子动力学、结构驱动药物设计 | 精准小分子 | 多个临床项目，代表 physics-based AI drug discovery |
| Iambic Therapeutics | 美国圣地亚哥，2019 | NeuralPLexer、Enchant、结构预测与生成模型 | 小分子设计 | 与 Takeda 等合作，已有早期临床项目 |
| Genesis Molecular AI | 美国湾区，2019 | 扩散模型、物理模拟、小 / 中分子生成 | 肿瘤、免疫 | 与 Incyte 等合作 |
| Terray Therapeutics | 美国洛杉矶，约 2018 | 超高通量微阵列、生成式 AI、TerraBind | 难成药靶点、小分子 | BMS、Calico 合作；Series B 资金支持 |
| Valo Health | 美国 Lexington，2019 | Opal 平台、人源数据、AI 药物发现 | 心代谢、肥胖、2 型糖尿病 | 与 Novo Nordisk 扩大合作 |
| XtalPi | 中国 / 美国，2015 | AI + 机器人实验 + 量子物理计算 | 药物发现、固态研究、材料、自动化实验 | 港股上市，代表中国 AI + robotics drug discovery 公司 |

### 3.2 生成式生物学、蛋白与抗体设计

| 公司 | 核心方向 | 价值点 | 商业化状态 |
|---|---|---|---|
| Generate:Biomedicines | 生成式蛋白药、抗体工程 | 用 AI 设计蛋白药物，GB-0895 进入 Phase 3 | 临床验证靠前，已 IPO |
| Absci | AI-native antibody creation | de novo 抗体设计 + 湿实验闭环 | 与 AstraZeneca 等合作 |
| BigHat Biosciences | AI 抗体设计 | Milliner 平台，快速设计-实验-学习循环 | 与 AbbVie、Lilly、J&J 等合作 |
| Cradle | 生成式蛋白工程 SaaS | 让药企和工业客户优化蛋白、酶、抗体 | 服务多家 Top pharma，Series B 后增长较快 |
| EvolutionaryScale | ESM3 蛋白语言模型 | 序列、结构、功能联合生成 | 生物基础模型代表，由 Meta ESM 团队衍生 |
| Profluent Bio | AI 生成蛋白 / gene editor | OpenCRISPR-1 等 AI-generated gene editor | 偏平台与基因编辑工具 |
| Chai Discovery | 抗体与结构模型 | Chai 系列模型用于结构预测和抗体设计 | 生物模型层新玩家 |
| Nabla Bio | 蛋白 / 抗体设计 | 聚焦难靶点、跨膜蛋白等 | 与药企合作型平台 |
| LabGenius | 抗体 / 多特异性抗体 | AI + robotics + synthetic biology 闭环 | 与 Sanofi、LG Chem 等合作 |
| Inceptive | RNA / sequence-based medicines | foundation models of life 用于 RNA 药物 | 与 Alnylam 合作 |
| A-Alpha Bio | 蛋白互作数据平台 | AlphaSeq 大规模 PPI 数据，训练模型 | 数据平台与合作开发模式 |

### 3.3 AI Scientist 与自驱动实验室

| 公司 | 定位 | 核心能力 | 与 AI4Sci 的关系 |
|---|---|---|---|
| Lila Sciences | AI Science Factory | 科学超级智能、实验工厂、模型-实验闭环 | 最接近“AI scientist + wet lab factory”的公司叙事 |
| FutureHouse / Edison Scientific | AI Scientist agent | 文献推理、实验规划、多 Agent 科研系统 | 代表科研 Agent 的独立路线 |
| Emerald Cloud Lab | 云实验室 | 远程设计、执行、分析实验，200+ 仪器 | 把湿实验变成可编程资源 |
| Strateos | Robotic cloud lab | 远程机器人实验室、on-site private cloud labs | 药企自动化实验基础设施 |
| Ginkgo Bioworks | 合成生物学 foundry / autonomous labs | 自动化实验、数据生成、细胞工程 | 从生物 foundry 转向 AI-ready 数据生成 |
| Culture Biosciences | 云连接生物反应器 | 生物工艺实验、在线数据、AI 优化 | 生物制造 / 工艺开发数据闭环 |
| Automata | 实验室自动化平台 | LINQ 模块化实验室自动化 | AI-ready wet lab 硬件和编排层 |
| Synthace | Computer-aided biology | 实验设计、DOE、元数据结构化 | 实验轨迹与结构化数据层 |
| Arctoris | 自动化 wet-lab CRO | 机器人实验与 ML 协同 | CRO 形态的 AI wet-lab 执行层 |

### 3.4 大厂、基础模型与基础设施

| 机构 / 公司 | 主要布局 | 重要性 |
|---|---|---|
| Google DeepMind / Isomorphic Labs | AlphaFold 3、AlphaFold Server、AI co-scientist、药物发现商业化 | 数字生物学标杆，从结构预测走向药物发现 |
| NVIDIA | BioNeMo、NIM、GPU、BioAI agent toolkit | 算力 + 模型 + 工具调用层 |
| Microsoft | Microsoft Discovery、AI for Science、BioEmu | 企业级 agentic R&D 平台和科学模拟 |
| OpenAI | 生命科学模型与科研工作流、与 Moderna / Retro / Ginkgo 等合作 | 通用推理模型进入生命科学研发流程 |
| Anthropic | Claude for Life Sciences、科研工具连接 | 科研 assistant / agent 编排层 |
| AWS | HealthOmics、Bedrock、专业模型托管 | 云端 bioFM 与药物发现基础设施 |
| Oracle | Life Sciences AI Data Platform、OCI | 生命科学数据平台与算力 |
| Databricks | Genesis Workbench、MCP / agentic drug discovery | 企业数据湖 + AI agent 工作流 |
| Benchling | ELN / LIMS / R&D Cloud | 实验数据系统 of record |
| Veeva | Vault AI、临床、监管、安全、质量流程 | 生命科学合规业务流程入口 |

### 3.5 临床、多模态数据与真实世界证据

| 公司 | 核心资产 | 价值 |
|---|---|---|
| Tempus AI | 去标识化患者记录、多组学、肿瘤数据、AI 模型 | 药企临床开发和真实世界数据平台 |
| Owkin | 多模态患者数据、联邦学习、K Pro / AI agents | 肿瘤和药物研发数据合作 |
| PathAI | AI 病理 | 临床试验病理终点、诊断和药物开发 |
| Paige | 数字病理 foundation model | 病理图像模型和肿瘤诊断 |
| Freenome | 多组学早筛 | AI + multiomics 早癌检测 |
| SOPHiA Genetics | 基因组与临床数据平台 | 医院和药企数据网络 |

---

## 4. 重点公司案例

### 4.1 Isomorphic Labs

**定位**：Alphabet / DeepMind 体系下的 AI-first 药物发现公司。  
**技术路线**：将 AlphaFold 体系从蛋白结构预测扩展到多分子相互作用和药物设计，包括小分子、生物药、抗体、肽和分子胶等。  
**商业验证**：与 Eli Lilly、Novartis、Johnson & Johnson 等药企开展合作。  
**判断**：它的优势是顶级模型、人才和 Alphabet 生态；短板是公开临床验证仍处早期。

参考：

- [Google DeepMind: AlphaFold 3](https://blog.google/innovation-and-ai/products/google-deepmind-isomorphic-alphafold-3-ai-model/)
- [Isomorphic Labs partnerships](https://www.isomorphiclabs.com/partnerships)
- [Isomorphic Labs 与 Johnson & Johnson 合作](https://www.isomorphiclabs.com/articles/isomorphic-labs-enters-into-a-research-collaboration-with-johnson-johnson)

### 4.2 Recursion + Exscientia

**定位**：上市 AI 药物发现平台，2024 年完成 Recursion 与 Exscientia 合并。  
**技术路线**：Recursion OS、自动化高通量湿实验、表型组学、转录组 / 蛋白组 / ADME 数据、生成化学、BioHive 超算。  
**商业验证**：Roche / Genentech、Sanofi、Bayer 等合作，拥有多个临床和临床前项目。  
**风险提示**：上市公司披露显示仍处高投入阶段，且已有项目停项，说明 AI 药物发现仍受临床转化风险制约。  
**判断**：Recursion 是“自动化实验 + 数据规模 + AI 平台 + 临床管线”路线的代表。

参考：

- [Recursion and Exscientia merger](https://ir.recursion.com/news-releases/news-release-details/recursion-and-exscientia-two-leaders-ai-drug-discovery-space/)
- [Recursion platform](https://www.recursion.com/platform)

### 4.3 Insilico Medicine

**定位**：AI 药物发现代表公司，横跨靶点发现、分子生成、自动化实验与临床管线。  
**技术路线**：PandaOmics 做靶点发现，Chemistry42 做生成化学，Pharma.AI 做平台化研发。  
**商业验证**：rentosertib 在 IPF Phase 2a 中出现临床信号；与 Lilly、SK Biopharmaceuticals 等合作。  
**判断**：它是少数能将“AI 发现 / AI 设计”与人体临床 PoC 关联起来讲清楚的公司之一。

参考：

- [Insilico Medicine](https://insilico.com/)
- [Nature Medicine: rentosertib Phase 2a](https://www.nature.com/articles/s41591-025-03743-2)

### 4.4 Generate:Biomedicines

**定位**：生成式蛋白药公司。  
**技术路线**：用生成式 AI 设计蛋白、抗体等治疗分子。  
**商业验证**：GB-0895 是 AI-engineered long-acting anti-TSLP antibody，已启动全球 Phase 3 研究。  
**判断**：如果 GB-0895 进入后期临床并成功，将成为生成式生物学商业化的强验证。

参考：

- [Generate:Biomedicines Phase 3 announcement](https://generatebiomedicines.com/media-center/generatebiomedicines-to-initiate-global-phase-3-studies-of-gb-0895-a-long-acting-anti-tslp-antibody-for-severe-asthma-engineered-with-ai)

### 4.5 Lila Sciences

**定位**：以 AI Science Factory 为核心叙事的科学超级智能公司。  
**技术路线**：AI agent + 生物 / 化学 / 材料实验工厂 + 数据闭环。  
**生命科学应用**：遗传药物、抗体、蛋白结合物、UTR、CAR-T 等。  
**判断**：Lila 是最值得关注的“AGI for science”新公司之一，因为它不只强调模型，而是强调物理实验闭环。

参考：

- [Lila Sciences](https://www.lila.ai/)
- [Lila Sciences: therapeutics](https://www.lila.ai/industries/therapeutics)

### 4.6 FutureHouse / Edison Scientific

**定位**：AI Scientist 和科研 Agent。  
**技术路线**：面向文献检索、综述、假设生成、前人工作判断、化学实验规划等科研任务的多 Agent 系统。  
**商业化**：FutureHouse 偏非营利研究，Edison Scientific 承接商业化部署。  
**判断**：代表“科研认知劳动自动化”路线，对 Science Agent OS 有直接参照价值。

参考：

- [FutureHouse](https://www.futurehouse.org/)
- [FutureHouse AI agents platform](https://www.futurehouse.org/research-announcements/launching-futurehouse-platform-ai-agents)
- [Edison Scientific announcement](https://www.futurehouse.org/research-announcements/announcing-edison-scientific)

### 4.7 EvolutionaryScale

**定位**：蛋白语言模型公司，由 Meta ESM 相关团队衍生。  
**技术路线**：ESM3 同时建模蛋白序列、结构和功能，用于生成和设计新蛋白。  
**判断**：代表“生物基础模型公司”路线，不一定自己做完整药物管线，但可能成为生物设计的基础模型供应商。

参考：

- [EvolutionaryScale: ESM3](https://www.evolutionaryscale.ai/blog/esm3-release)
- [Meta ESM Atlas](https://ai.meta.com/blog/protein-folding-esmfold-metagenomics/)

### 4.8 Absci、BigHat、Cradle、LabGenius

这些公司共同代表“蛋白 / 抗体设计 + 湿实验闭环”的中间层玩家：

- **Absci**：de novo antibody design，强调 data to train、AI to create、wet lab to validate。
- **BigHat**：Milliner 平台，AI 抗体设计与快速实验循环。
- **Cradle**：生成式蛋白工程 SaaS，服务药企和工业蛋白工程。
- **LabGenius**：EVA 平台，AI / ML + robotics + synthetic biology 做抗体发现。

它们的共同启发是：蛋白设计不是一次生成候选，而是多轮约束优化，包括 binding、specificity、stability、developability、expression、toxicity、manufacturability 等多目标 reward。

参考：

- [Absci technology](https://www.absci.com/technology/)
- [Absci-AstraZeneca collaboration](https://investors.absci.com/news-releases/news-release-details/absci-announces-collaboration-astrazeneca-advance-ai-driven)
- [BigHat technology](https://www.bighatbio.com/technology)
- [Cradle Series B](https://www.cradle.bio/blog/series-b)
- [LabGenius](https://labgeniustx.com/)

---

## 5. 商业化验证与失败案例

### 5.1 已经被验证的部分

1. **药企愿意为 AI 平台付费**  
   Isomorphic、Schrodinger、Insilico、Valo、Absci、BigHat、Genesis、Terray 等公司都有大药企合作。

2. **AI 发现 / 设计候选物可以进入临床**  
   Insilico、Recursion、Schrodinger、Generate、Iambic 等已有临床阶段资产。

3. **自动化实验和数据平台有独立价值**  
   Emerald Cloud Lab、Strateos、Ginkgo、Synthace、Automata、Benchling、Tempus 等说明即使不拥有药物管线，实验 / 数据 / 工作流基础设施也有商业空间。

4. **大模型正在进入药企组织流程**  
   OpenAI、Anthropic、Microsoft、Google Cloud、AWS、Oracle、Veeva、Benchling 等都在将 agent / AI assistant 接入生命科学工作流。

### 5.2 仍未充分验证的部分

1. **AI 是否显著提高 Phase 2 / Phase 3 成功率**  
   目前多数案例仍处早期临床或临床前阶段。

2. **headline deal value 是否能转化为真实收入**  
   大额合作常包含大量后端里程碑，不能直接等同于现金收入。

3. **平台是否能持续产出多个有效管线**  
   单个 PoC 不等于平台可复制。

4. **AI Scientist 是否能自主提出并完成高价值科学发现**  
   当前更多是辅助、编排、检索、设计和实验优化，还没有充分证明完全自主科学发现。

### 5.3 失败与风险

| 风险 | 说明 |
|---|---|
| 临床失败 | AI 可提高搜索效率，但不能消除人体复杂性、毒性、剂量、终点设计和患者分层风险 |
| 数据偏差 | 公开数据、历史实验数据和医院数据都可能存在偏差、缺失和不可比性 |
| 湿实验瓶颈 | 生成候选容易，验证、优化和生产更难 |
| 监管不确定性 | FDA / EMA 正在明确 AI 在药物生命周期中的可信度、适用场景和验证要求 |
| 商业模式压力 | 平台型收入、合作型收入、管线型收入的风险结构不同 |
| 生物安全 | AI 设计蛋白、基因编辑器和病原相关序列需要治理 |

参考：

- [FDA: Artificial Intelligence in Drug Development](https://www.fda.gov/about-fda/center-drug-evaluation-and-research-cder/artificial-intelligence-drug-development)
- [FDA draft guidance: AI to support regulatory decision-making](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/considerations-use-artificial-intelligence-support-regulatory-decision-making-drug-and-biological)
- [EMA: AI in medicinal product lifecycle](https://www.ema.europa.eu/en/use-artificial-intelligence-ai-medicinal-product-lifecycle-scientific-guideline)
- [BenevolentAI BEN-2293 Phase 2a result](https://www.benevolent.com/news-and-media/press-releases-and-in-media/benevolentai-announces-top-line-phase-iia-results-its-topical-pan-trk-inhibitor-ben-2293-1-mild-moderate-atopic-dermatitis/)

---

## 6. 对 Science Agent Evolution Infrastructure 的启发

### 6.1 不要只做科研 Copilot

市场上已经出现大量科研 assistant、文献 RAG、chat with papers、protocol generator。它们有用，但壁垒有限。真正的长期壁垒在：

- 任务状态；
- 科学证据链；
- 专家判断；
- 实验结果；
- 失败轨迹；
- reward 设计；
- 可训练数据；
- 可复用 agent policy。

### 6.2 不要只做单点蛋白设计模型

蛋白 / 抗体设计公司的共同经验是：模型只是第一步，真正难的是多目标优化和闭环验证。

一个可训练的 Target-to-Binder 系统至少需要：

```text
Target Card
  → Evidence Review
  → Design Strategy
  → Candidate Generation
  → In-silico Filtering
  → Expert Review
  → Wet-lab Plan
  → Experiment Result
  → Reward Vector
  → Next-round Design
```

### 6.3 器官芯片更适合作为 reward factory

从 related work 看，自动化实验公司的价值在于提供 AI 可调用的物理反馈。器官芯片不应一开始被定义为独立湿实验平台，而更适合作为人体相关 phenotype reward 的来源：

- efficacy phenotype；
- toxicity phenotype；
- tissue-specific response；
- mechanism readout；
- dose response；
- safety / developability proxy。

这能把蛋白设计从 binding 优化推进到功能表型优化。

### 6.4 Scientific Memory 是护城河

AI4Sci 组织最值得沉淀的不是最终答案，而是过程：

- 为什么选这个 target？
- 哪些证据支持 / 反对？
- 哪些候选被淘汰？
- 淘汰原因是什么？
- 哪个 expert 提过什么 objection？
- 哪个实验失败了？
- 失败是 protocol、sample、assay、model 还是 hypothesis 问题？
- 下一轮设计吸收了什么反馈？

这些信息构成科研组织的长期记忆和训练数据。

### 6.5 Reward 需要分层

生命科学任务不能只有一个 reward。建议将 reward 拆成：

| Reward 类型 | 例子 |
|---|---|
| Evidence reward | 文献证据强度、遗传证据、疾病相关性 |
| Model reward | pLDDT、PAE、binding score、affinity、specificity |
| Developability reward | stability、expression、aggregation、immunogenicity、manufacturability |
| Experiment reward | binding assay、cell assay、organ-chip phenotype |
| Cost reward | 实验成本、时间、样本消耗 |
| Information gain reward | 实验是否减少关键不确定性 |
| Expert reward | PI / domain expert 的偏好、反驳和排序 |
| Safety reward | 生物安全、毒性、dual-use 风险 |

### 6.6 关键产品形态：Science Agent OS

related work 显示，领先公司都在从“工具”走向“系统”。因此本项目也应避免只做若干 AI 工具，而是设计 Science Agent OS：

```text
Scientific Resource Graph
  + Scientific Memory
  + Agent Workflow
  + Human Review Protocol
  + Experiment Interface
  + Reward Ledger
  + Training Data Compiler
```

---

## 7. 目标用户与中国国内 ICP

### 7.1 核心目标用户

本项目不应面向泛科研用户，也不应先做高校 PI 的通用科研助手。最优先目标用户是：

> **有明确 target / disease hypothesis，需要快速从 target 推进到 binder / antibody / protein candidate，并希望得到专家判断、wet validation 与更接近人体表型 reward 的 biotech / pharma discovery team。**

他们买的不是“AI 工具”，而是一个能帮助项目负责人判断是否继续投入的 **Candidate Decision Package**：

```text
Target Card
  + Evidence Review
  + Design Strategy
  + Binder / Antibody Candidate Set
  + Expert Objection & Ranking
  + Wet Validation Plan / Result
  + Organ-chip / Cell Phenotype Reward
  + Developability Risk
  + Next-round Design Plan
```

### 7.2 全球 ICP 分层

| ICP | 谁买单 | 谁使用 | 主要痛点 | 我们的切入方式 |
|---|---|---|---|---|
| 早中期 biologics biotech | CEO / CSO / VP Discovery | protein engineer、computational biologist、assay lead | 有靶点和机制假设，但缺完整 AI + expert + wet-loop 能力 | Target-to-Binder sprint + expert review + 小规模验证 |
| 药企 discovery / external innovation team | Head of Discovery、Modality lead、External Innovation | internal project team | 内部资源多但流程慢，特定项目需要外部速度和差异化证据 | 私有化 project room + candidate package + human-relevant reward |
| 新模态团队 | Program lead、Translational lead | 抗体、ADC、TCE、cell therapy、protein engineering 团队 | 候选物多目标优化复杂，binding 之外还要看功能、毒性和开发性 | 多目标 reward ledger + organ-chip / cell phenotype |
| CRO / organ-chip / model animal / wet-lab 平台 | BD、科学负责人 | 实验执行团队 | 有实验能力但缺 AI 设计和科研 trajectory 系统 | 作为 wet reward 和执行合作伙伴 |

### 7.3 为什么用户愿意外包

用户愿意把一部分任务外包，不是因为他们“不懂 AI”，而是因为要形成闭环需要跨越太多能力边界：

1. **完整能力栈难以自建**  
   一个可用的 target-to-binder 闭环需要结构生物学、蛋白 / 抗体设计、AI 模型、assay、organ-chip、专家 review、项目管理和数据系统。早中期 biotech 很难全栈自建。

2. **速度和资本效率更重要**  
   很多 biotech 的关键问题不是长期建设平台，而是 8-12 周内回答“这个 target 是否值得继续投钱”。外部闭环服务可以把固定成本变成项目成本。

3. **外部专家网络有独立价值**  
   内部团队容易被已有 hypothesis 锚定。外部 domain expert、结构专家、assay 专家、转化医学专家可以提供反驳、排序和 kill criteria。

4. **human-relevant phenotype reward 稀缺**  
   许多团队可以做 binding assay，但缺更接近人体机制的 organ-chip / organoid / cell phenotype readout。这个 reward 对候选优先级判断很重要。

5. **药企内部 AI 与外部平台并不互斥**  
   AstraZeneca 与 Absci、AbbVie 与 BigHat、Pfizer 与 Chai Discovery、Lilly TuneLab 等案例说明，大药企即使有内部 AI 团队，也会购买外部专业平台、模型或数据能力。

### 7.4 数据泄露顾虑与服务形态

生命科学客户尤其担心序列、靶点、未公开管线、实验结果、BD 计划和临床策略泄露。因此服务形态必须从第一天就围绕数据安全设计：

| 阶段 | 数据策略 | 适合客户 |
|---|---|---|
| Public Discovery Sprint | 只使用公开 target、文献、结构、数据库和客户给出的非机密约束 | 早期评估、BD 前快速判断 |
| Confidential Project Room | NDA、租户隔离、访问控制、审计日志，客户数据默认不进入通用训练 | 早中期 biotech、药企项目组 |
| Blinded Wet Loop | 样本、序列、项目代号脱敏；外部专家只看必要上下文 | 高敏感靶点、未公开管线 |
| Private / VPC Deployment | 在客户云、VPC 或本地环境部署，模型调用和数据留在客户环境 | 大药企、头部 biotech |
| Federated Learning / Opt-in Training | 跨客户训练默认关闭，只在客户明确授权时使用去标识化数据 | 长期战略合作 |

合同边界需要清晰：

- 客户 foreground IP 归客户；
- 我们的 background platform IP 归我们；
- 客户项目数据默认不用于训练跨客户模型；
- 专家 review 记录、实验轨迹、模型输出、失败结果都纳入项目数据治理；
- 对外展示只使用客户批准的案例或完全匿名统计。

### 7.5 中国国内目标用户

中国市场尤其适合该方向，但打法需要更谨慎。国内创新药已经从“快速跟随”进入“差异化、出海、BD 和临床兑现”阶段，ADC、双抗 / 多抗、TCE、细胞治疗、蛋白工程和新靶点竞争激烈。客户不缺研发团队，但缺的是 **更快的差异化证据、更强的专家判断、更可信的人体相关 reward，以及能支持 BD / IND / 立项决策的候选物证据包**。

#### 7.5.1 国内直接 ICP

| 国内用户类型 | 代表团队 / 公司类型 | 典型任务 | 购买动因 |
|---|---|---|---|
| 早中期创新药 biotech | 有新靶点、双抗、ADC、TCE、细胞治疗或蛋白药项目的公司 | 从 target 到 binder / antibody candidate，或对候选做二轮优化 | 内部团队小，外包可快速补齐 AI、专家和 wet validation |
| 头部 biologics / 创新药公司项目组 | 恒瑞、信达、复宏汉霖、康方、科伦博泰、和铂医药、百济神州、君实、荣昌、迈威等类型团队 | 特定高价值 target 的差异化设计、AI 辅助抗体 / ADC / 多抗优化、出海前数据包增强 | 内部有平台，但需要外部速度、专家反驳和 human-relevant phenotype reward |
| ADC / 双抗 / TCE 项目团队 | 国内 ADC、双抗、多抗、TCE 研发团队 | binder selection、epitope strategy、linker / payload / internalization、tumor microenvironment phenotype | 竞争拥挤，需要证明差异化和临床转化可能性 |
| 转化医学 / 临床前安全团队 | 药企 translational science、安全性评价、药效药理团队 | organ-chip / organoid / human cell readout 验证候选优先级 | 动物模型外推有限，需要更接近人体的早期证据 |
| BD / NewCo / 出海团队 | 准备 out-license、NewCo、海外 IND 或联合开发的团队 | 生成可被海外 partner / investor 理解的 evidence package | BD 竞争激烈，差异化证据和专家背书影响估值 |

#### 7.5.2 国内合作伙伴 / 渠道伙伴

| 伙伴类型 | 例子 | 合作价值 |
|---|---|---|
| AI for Science 平台公司 | 深势科技、晶泰科技、英矽智能、唯信计算等 | 模型、计算、分子 / 抗体设计工具，可能成为组件或联合解决方案 |
| 抗体 / 模型动物 / CRO 平台 | 百奥赛图、集萃药康、药明系、康龙化成、美迪西、昭衍等类型机构 | wet validation、动物模型、临床前执行、客户渠道 |
| 类器官 / 器官芯片平台 | 大橡科技、耀速科技、类器官 CRO / 转化医学平台 | 提供 human-relevant phenotype reward |
| 医院转化中心 / PI 孵化项目 | 肿瘤、自免、罕见病方向的转化医学中心 | 早期 disease biology、样本、机制验证和临床问题定义 |

### 7.6 中国市场公开信号

国内已经出现多条与本项目相关的公开信号：

- **复宏汉霖与深势科技** 达成 AI 辅助药物研发战略合作，覆盖癌症靶点、小分子、ADC linker 切割位点预测、生物药抗体发现与优化；复宏汉霖也公开强调 AI 驱动新药开发平台、蛋白药物发现、TCE 三特异性平台和 ADC 平台。
- **和铂医药与 Insilico Medicine** 合作推进 AI-driven antibody discovery，结合 Insilico 的 AI 能力与和铂医药湿实验能力，面向免疫、肿瘤和神经等疾病方向。
- **信达生物与唯信计算** 合作建设一站式 AI 药物研发平台，目标是降低 AI 落地和实验成本、缩短研发周期、提高成功率。
- **康方生物** 已形成双抗 / 多抗 / 双抗 ADC 等创新管线，公开披露多个候选药进入临床和商业化，说明国内 biologics 已进入高复杂度平台竞争。
- **科伦博泰** 以 ADC 平台和国际合作为代表，显示国内 ADC 公司已经进入全球竞争和 BD 验证阶段。
- **大橡科技、耀速科技等类器官 / 器官芯片公司** 说明国内 human-relevant preclinical model 正在产业化，适合作为本项目的 phenotype reward 伙伴。

### 7.7 中国市场推荐切入顺序

| 阶段 | 推荐客户 | 推荐产品形态 | 原因 |
|---|---|---|---|
| 0-6 个月 | 早中期 biotech、PI 孵化项目、BD 前项目 | Public / confidential Target-to-Binder sprint | 销售周期短，需求明确，容易形成案例 |
| 6-12 个月 | ADC / 双抗 / TCE 项目团队 | Candidate Decision Package + expert panel + wet validation | 国内竞争拥挤，差异化证据有直接商业价值 |
| 12-18 个月 | 头部药企项目组 | Private project room / VPC deployment + organ-chip reward | 数据敏感但付费能力强，需要安全部署 |
| 18 个月后 | CRO、器官芯片、医院转化中心 | 联合解决方案 / 渠道合作 | 扩大交付能力和客户来源 |

### 7.8 国内用户的独特销售主张

对中国客户，最有说服力的表述不是“我们有 AGI”，而是：

> **用 AI + 专家网络 + 湿实验 / 器官芯片 reward，在 8-12 周内帮你把一个 target 或候选物变成可立项、可停项、可 BD、可进入下一轮实验的证据包。**

具体价值：

1. **更快做 kill / continue 决策**：避免在低质量 target 或候选上继续烧钱。
2. **增强差异化证据**：不只给 binding，而是给 epitope、developability、functional phenotype 和专家反驳。
3. **支持出海 / BD 叙事**：形成海外 partner 能读懂的 evidence package。
4. **补齐跨学科能力**：把 AI、结构、抗体工程、assay、organ-chip、转化医学专家组织到同一项目流里。
5. **保护数据安全**：用分阶段披露、脱敏 wet loop、私有化部署和明确 IP 条款降低泄露顾虑。

---

## 8. 机会与竞争边界

### 8.1 近期可落地机会

1. **Target-to-Binder agent workflow**  
   结合文献、数据库、结构预测、蛋白设计、专家 review 和 wet-lab plan。

2. **Scientific Memory / Project State Graph**  
   做科研项目的 system of record，而不是聊天记录。

3. **Experiment Planning and Review Agent**  
   让 Agent 输出可执行实验计划，并由专家审批。

4. **Reward Ledger**  
   统一记录 computational score、expert score、wet-lab result 和 cost。

5. **Trajectory Compiler**  
   将每次科研任务编译为可训练样本，服务后续 SFT、preference learning、critique learning、offline RL。

### 8.2 不建议直接硬碰的区域

1. 从零训练通用生物基础模型；
2. 与 Isomorphic / EvolutionaryScale / Chai 正面竞争结构预测基础模型；
3. 自建大规模全栈湿实验平台；
4. 一开始就做完整药物管线公司；
5. 泛化科研聊天助手。

### 8.3 推荐 wedge

最适合本项目的 wedge 是：

> **Target-to-Binder Research & Design Loop with Organ-chip Phenotype Reward**

理由：

- 足够具体，可以验证；
- 覆盖科研 Agent 的关键能力；
- 能利用现有蛋白设计模型和结构工具；
- 能接入专家 review；
- 能产生实验 reward；
- 能自然沉淀 trajectory 和 training data；
- 与 Frontis 的 ME / WE / MA 组织智能框架一致。

---

## 9. 重点观察清单

### 9.1 需要持续跟踪的公司

| 优先级 | 公司 |
|---|---|
| 高 | Isomorphic Labs、Recursion、Insilico、Generate、Lila、FutureHouse、EvolutionaryScale、Absci、Cradle、Tempus、深势科技、晶泰科技、英矽智能 |
| 中高 | Xaira、insitro、Schrodinger、Iambic、Genesis、Terray、BigHat、LabGenius、Chai、Profluent、Owkin、复宏汉霖、和铂医药、信达生物、康方生物、科伦博泰、恒瑞医药 |
| 中 | Emerald Cloud Lab、Strateos、Ginkgo、Synthace、Automata、Culture Biosciences、Benchling、Veeva、Databricks、大橡科技、耀速科技、百奥赛图、集萃药康、美迪西 |

### 9.2 需要持续跟踪的信号

1. AI-designed / AI-discovered drug 是否进入 Phase 2b / Phase 3；
2. 是否出现 FDA / EMA 对 AI 支持药物开发的关键案例；
3. 大药企合作中的 upfront / milestone 比例；
4. 自动化实验室是否与 foundation model 形成真实闭环；
5. 生物基础模型是否从 benchmark 转向 wet-lab success rate；
6. 科研 Agent 是否能在真实项目中减少周期和成本；
7. 生物安全监管是否收紧；
8. TechBio 上市公司现金流、裁员、并购和管线停项情况。

---

## 10. 资源预算与 HC 对标

详细测算见：[AI4AI / AGI4Sci 头部创业公司资源预算与 HC 对标](./ai4ai_agi4sci_startup_budget_benchmark_2026-06-28.md)。

### 10.1 不应直接按大厂 AI 基建口径估算

字节、阿里、腾讯、京东等大厂 AI 基建投入是集团级、云基础设施级，适合判断 AI 竞争的资本强度，但不适合直接作为 Frontis 第一阶段部门预算。更合适的参照是：

- Lila Sciences、Periodic Labs：AI Scientist + 自主实验设施的重资产上限；
- FutureHouse / Edison Scientific：agent-first、相对轻资产的 AI Scientist 路线；
- EvolutionaryScale、Cradle、Generate、Xaira：生物基础模型、蛋白工程和 AI-native biotech 的不同资本强度；
- 深势科技、晶泰科技、百图生科、英矽智能、剂泰科技：国内 AI4Sci / AI drug discovery 的融资、HC 和干湿闭环样本。

### 10.2 衔远第一年预算建议

结合衔远当前阶段，建议先采用 5200 万元人民币 / 年验证版，而不是直接上头部创业公司的重资产标准档。这个版本的目标是用小而完整的核心团队，配常态 64 张 H200，跑通 1 条可收费项目闭环、1 个关键 ML benchmark 和必要的外部实验验证，不在第一年自训大型 foundation model 或自建 wet-lab。

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

### 10.3 判断

1. 如果只做科研 agent、项目工作区和少量 wet validation，保守档即可。
2. 如果要同时验证 Target-to-Binder 闭环和一个关键 ML benchmark，5200 万元 / 年版本更符合衔远当前阶段。
3. 如果付费项目、数据飞轮和实验回流都成立，再升级到 8000 万-1.5 亿元 / 年的标准档。
4. 如果要自训大型生命科学 foundation model、自建自动化实验平台或多项目 wet-lab 并行，应进入进取档。
5. 预算不能只看 GPU。头部公司共同特征是：专有数据、实验反馈、专家评审、自动化或半自动化 wet-lab 网络、BD / IP / 合规能力共同构成壁垒。

---

## 11. 结论

生命科学方向的 AGI 加速科学发现，短期不会表现为“一个通用 AGI 科学家独立发明新药”，而会表现为：

```text
科研 Agent 负责推理和编排；
生物基础模型负责生成和预测；
自动化实验室负责验证和造数据；
专家负责审查和偏好标注；
临床 / 真实世界数据负责外部验证；
Trajectory / Reward 系统负责持续训练。
```

因此，AI4Sci 基础设施的关键不是追逐某一个最强模型，而是建设一套可以让科研组织持续学习的系统：

- 科研状态可记录；
- 科学证据可审计；
- 任务轨迹可复盘；
- 实验反馈可结构化；
- 专家判断可训练；
- 失败经验可复用；
- Agent 能在真实科研闭环中持续进化。

这正是 Science Agent Evolution Infrastructure 的核心战略价值。

---

## 12. 参考来源

### AI 药物发现与生成式生物学

- [Isomorphic Labs partnerships](https://www.isomorphiclabs.com/partnerships)
- [Isomorphic Labs 与 Johnson & Johnson 合作](https://www.isomorphiclabs.com/articles/isomorphic-labs-enters-into-a-research-collaboration-with-johnson-johnson)
- [Google DeepMind: AlphaFold 3](https://blog.google/innovation-and-ai/products/google-deepmind-isomorphic-alphafold-3-ai-model/)
- [Recursion and Exscientia merger](https://ir.recursion.com/news-releases/news-release-details/recursion-and-exscientia-two-leaders-ai-drug-discovery-space/)
- [Recursion platform](https://www.recursion.com/platform)
- [Insilico Medicine](https://insilico.com/)
- [Nature Medicine: rentosertib Phase 2a](https://www.nature.com/articles/s41591-025-03743-2)
- [Generate:Biomedicines Phase 3 announcement](https://generatebiomedicines.com/media-center/generatebiomedicines-to-initiate-global-phase-3-studies-of-gb-0895-a-long-acting-anti-tslp-antibody-for-severe-asthma-engineered-with-ai)
- [Absci technology](https://www.absci.com/technology/)
- [Absci-AstraZeneca collaboration](https://investors.absci.com/news-releases/news-release-details/absci-announces-collaboration-astrazeneca-advance-ai-driven)
- [BigHat technology](https://www.bighatbio.com/technology)
- [Cradle Series B](https://www.cradle.bio/blog/series-b)
- [EvolutionaryScale: ESM3](https://www.evolutionaryscale.ai/blog/esm3-release)
- [Meta ESM Atlas](https://ai.meta.com/blog/protein-folding-esmfold-metagenomics/)
- [Profluent OpenCRISPR](https://www.profluent.bio/media/editing-the-human-genome-with-ai)

### AI Scientist 与自动化实验室

- [Lila Sciences](https://www.lila.ai/)
- [Lila Sciences therapeutics](https://www.lila.ai/industries/therapeutics)
- [FutureHouse](https://www.futurehouse.org/)
- [FutureHouse AI agents platform](https://www.futurehouse.org/research-announcements/launching-futurehouse-platform-ai-agents)
- [Edison Scientific announcement](https://www.futurehouse.org/research-announcements/announcing-edison-scientific)
- [Emerald Cloud Lab](https://www.emeraldcloudlab.com/)
- [Emerald Cloud Lab: how it works](https://www.emeraldcloudlab.com/how-it-works/run/)
- [Strateos](https://www.strateos.com/)
- [Ginkgo Bioworks](https://www.ginkgo.bio/)
- [Synthace](https://www.synthace.com/)
- [Automata](https://www.automata.tech/)

### 大厂与基础设施

- [NVIDIA BioNeMo Agent Toolkit](https://nvidianews.nvidia.com/news/nvidia-launches-bionemo-agent-toolkit-giving-ai-agents-the-tools-to-accelerate-scientific-discovery)
- [Microsoft Discovery](https://azure.microsoft.com/en-us/blog/transforming-rd-with-agentic-ai-introducing-microsoft-discovery/)
- [Microsoft BioEmu-1](https://www.microsoft.com/en-us/research/blog/exploring-the-structural-changes-driving-protein-function-with-bioemu-1/)
- [Anthropic Claude for Life Sciences](https://www.anthropic.com/news/claude-for-life-sciences)
- [AWS HealthOmics for Drug Discovery](https://aws.amazon.com/healthomics/drug-discovery/)
- [Oracle Life Sciences AI Data Platform](https://www.oracle.com/news/announcement/oracle-life-sciences-ai-data-platform-unites-data-and-agentic-intelligence-2026-01-29/)
- [Databricks Genesis Workbench](https://www.databricks.com/blog/genesis-workbench-blueprint-life-sciences-applications-databricks)
- [Veeva Vault AI](https://www.veeva.com/products/vault-ai/)

### 数据、临床与监管

- [Tempus S-1](https://www.sec.gov/Archives/edgar/data/1717115/000119312524142956/d221145ds1.htm)
- [Owkin-Sanofi collaboration](https://www.sanofi.com/en/media-room/press-releases/2021/2021-11-18-06-30-00-2336966)
- [FDA: Artificial Intelligence in Drug Development](https://www.fda.gov/about-fda/center-drug-evaluation-and-research-cder/artificial-intelligence-drug-development)
- [FDA draft guidance: AI to support regulatory decision-making](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/considerations-use-artificial-intelligence-support-regulatory-decision-making-drug-and-biological)
- [EMA: AI in medicinal product lifecycle](https://www.ema.europa.eu/en/use-artificial-intelligence-ai-medicinal-product-lifecycle-scientific-guideline)
- [BenevolentAI BEN-2293 Phase 2a result](https://www.benevolent.com/news-and-media/press-releases-and-in-media/benevolentai-announces-top-line-phase-iia-results-its-topical-pan-trk-inhibitor-ben-2293-1-mild-moderate-atopic-dermatitis/)

### 中国国内用户、合作与器官芯片相关来源

- [复宏汉霖与深势科技 AI 辅助药物研发战略合作](https://www.henlius.com/NewsDetails-4839-26.html)
- [复宏汉霖 2025 全球研发日：TCE、ADC、AI 新药开发平台](https://www.henlius.com/NewsDetails-4962-26.html)
- [复宏汉霖全产业平台与创新管线](https://www.henlius.com/comprehensive-platform.html)
- [和铂医药与 Insilico Medicine 推进 AI-driven antibody discovery](https://www.harbourbiomed.com/news/234.html)
- [和铂医药：抗体发现引擎与 AI 技术](https://www.harbourbiomed.com/)
- [信达生物与唯信计算推进 AI 药物研发平台建设](https://www.prnewswire.com/news-releases/innovent-and-wecomput-announce-strategic-partnership-to-advance-ai-driven-drug-discovery-and-development-302207255.html)
- [唯信计算 WeMol 平台](https://www.wecomput.com/af5fb0540d/)
- [迈威生物与 Insilico Medicine：AI 赋能 ADC 创新药研发](https://www.mabwell.com/news_info/id-202.html)
- [深势科技生命科学 AI 研发解决方案](https://www.dp.tech/services/solution)
- [乐普生物与深势科技 ADC drug collaboration](https://www.prnewswire.com/news-releases/dp-technology-and-lepu-biopharma-announce-milestone-collaboration-leveraging-advanced-computational-methods-to-accelerate-adc-drug-innovation-302312430.html)
- [康方生物 ACE Platform、AI 制药、双抗/多抗、ADC、TCE](https://www.akesobio.com/)
- [康方生物 2026 新闻：双抗/多抗、AI 新药研发、双抗 ADC、TCE](https://www.akesobio.com/cn/media/akeso-news/20260327-1/)
- [科伦博泰 ADC 平台 OptiDC](https://kelun-biotech.com/)
- [恒瑞医药 2025 研发日：ADC、双/多抗、小核酸、口服多肽等平台](https://www.hengrui.com/media/detail-889.html)
- [大橡科技：类器官芯片 / organ-on-a-chip](https://www.daxiangbio.cn/)
- [大橡科技与集萃药康：类器官与小鼠模型联合赋能新药研发](https://cn.gempharmatech.com/about/detail/4867393.html)
- [耀速科技与辉瑞：AI 深度学习病理图像自动识别系统](https://www.fengxian.gov.cn/gzms/20250624/91241.html)
- [耀速科技融资与 3D-Wet-AI 闭环体系](https://www.stcn.com/article/detail/1733756.html)
