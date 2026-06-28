# 中国蛋白质设计与器官芯片企业调研报告

**调研日期**：2026-06-28  
**用途**：AI4Sci / Scientific MA 方向的 related work 与产业参照  
**调研对象**：中国国内及中国团队主导的蛋白质设计、AI 蛋白设计、器官芯片、类器官芯片、微生理系统相关企业  
**结论口径**：以下“龙头 / 准龙头”是基于公开资料、融资与合作、平台成熟度、产业落地和赛道纯度形成的判断，不等同于收入排名。

---

## 0. Executive Summary

蛋白质设计方向，国内已形成一批以 AI 大模型、结构预测、生成式蛋白设计、抗体/多肽/酶设计和干湿实验闭环为核心的公司。当前更值得重点跟踪的头部梯队包括：

- **分子之心 MoleculeMind**：更接近“纯 AI 蛋白设计平台”龙头候选。
- **百奥几何 BioGeometry**：生成式全原子蛋白设计和干湿闭环方向的准龙头。
- **华深智药 Helixon / Earendil Labs**：AI 抗体和蛋白疗法设计方向商业化验证较强。
- **百图生科 BioMap**：生命科学大模型平台型头部，蛋白设计是其中重要模块。
- **天鹜科技 Matwings**：工业蛋白、酶设计、生物制造落地较强。

器官芯片方向，国内仍处在早期商业化阶段，头部判断不能只看“类器官”或“微流控”标签，而要看是否有标准化芯片/设备/模型体系、药企付费项目、IND 或监管证据链。当前更值得重点跟踪的公司包括：

- **艾玮得 AVATARGET**：器官芯片数据进入药物临床申报证据链的公开案例较突出。
- **大橡科技 Daxiang Bio**：类器官芯片产品化和药筛服务能力较完整。
- **耀速科技 Xellar Biosystems**：高通量器官芯片 + AI + 国际药企合作路线。
- **丹望医疗 D1Med**：类器官模型库、药筛服务和类器官芯片融合路线。

对 Frontis / AI4Sci 的启发是：单点蛋白设计模型和单点器官芯片平台都已有专业玩家，Frontis 更适合切入 **Science Agent Evolution Infrastructure**，把蛋白质设计与器官芯片作为真实任务场和 reward source，而不是从零复制某一家模型公司或湿实验平台。

---

## 1. 判断标准

### 1.1 蛋白质设计企业判断标准

| 指标 | 含义 |
|---|---|
| 赛道纯度 | 核心产品是否直接输出新蛋白序列、结构、功能优化方案，还是只做广义 AI 制药 |
| 干湿闭环 | 是否具备计算设计、合成表达、实验筛选、模型迭代的闭环能力 |
| 技术壁垒 | 是否有结构预测、生成式模型、全原子建模、多目标优化、抗体/酶/多肽设计能力 |
| 产业验证 | 是否有药企/工业客户付费项目、BD、授权、共同开发或量产案例 |
| 通用性 | 是否能跨靶点、跨蛋白类型复用，而不是只完成单点项目 |
| 可核验证据 | 是否有官网、论文、融资公告、药企合作公告、监管或交易所文件支持 |

### 1.2 器官芯片企业判断标准

| 指标 | 含义 |
|---|---|
| 芯片属性 | 是否真的有微流控、芯片化、动态培养、多细胞分区、力学/流体控制等 OoC / MPS 特征 |
| 生物模型质量 | 是否能保持器官相关结构、功能、生理 readout 和疾病表型 |
| 标准化能力 | 是否有芯片、设备、试剂、SOP、数据分析和质量体系 |
| 药企应用 | 是否进入药效、毒理、DMPK、候选筛选或 IND 支撑链条 |
| 临床相关性 | 类器官药敏、患者来源模型、前瞻性验证或临床相关论文 |
| 商业化程度 | 是否有明确产品、服务、客户、融资、合作和复购线索 |

---

## 2. 赛道边界

### 2.1 蛋白质设计与相邻赛道

**蛋白质设计 / AI 蛋白设计** 的核心输出是新蛋白或优化蛋白的序列、结构和功能，常见对象包括抗体、纳米抗体、多肽、酶、小蛋白、疫苗抗原等。理想状态是计算生成后进入湿实验验证，并把实验结果反馈给模型。

**AI 制药** 范围更大，包含靶点发现、小分子生成、ADMET、晶型预测、临床试验设计等。晶泰科技、英矽智能等是 AI 制药或 AI4S 重要公司，但不能因为有 AI 药物发现能力就直接归为“蛋白质设计龙头”。

**合成生物 / 酶设计** 是蛋白设计的重要应用分支，但商业落点常在工业酶、菌株、细胞工厂和生物制造。天鹜科技、百奥几何的酶设计能力与蛋白设计本体高度相关；恩和科技、凯赛生物、蓝晶微生物等则更适合作为合成生物公司评估。

**抗体发现 / 抗体 CRO** 与蛋白设计有交集，但并不天然等于 AI 蛋白设计。百奥赛图、三优生物、百英生物、义翘神州等更应按抗体发现、抗体工程、试剂和 CRO 服务来评估。

### 2.2 器官芯片与相邻赛道

**类器官** 是体外 3D 自组织结构，强调组织来源、分化状态和疾病表型。

**器官芯片 / Organ-on-a-Chip / MPS** 强调芯片化微环境控制，通常包含微流控、动态培养、机械力、营养/代谢交换、多细胞分区等工程属性。

**类器官芯片** 是类器官和器官芯片的融合形态，既有类器官模型，又有芯片或微流控工程调控。

**微流控工具商** 可能是器官芯片上游供应商，但如果主要业务是微流控打印、控制模组或通用芯片制造，不能直接算器官芯片药筛平台龙头。

**CRO 药筛公司** 可以使用类器官或器官芯片模型，但“会做药筛”不代表拥有器官芯片底层平台。

---

## 3. 蛋白质设计企业图谱

### 3.1 核心梯队

| 企业 | 定位 | 头部判断 | 关键证据 | 主要风险 |
|---|---|---|---|---|
| 分子之心 MoleculeMind | AI 蛋白设计平台 | 龙头候选 | 2026 年 A 轮系列融资累计逾 1 亿美元；平台包括 MoleculeOS、NewOrigin、MMDesign；披露纳米抗体从头设计命中率表现 | 公开客户、收入和临床资产细节有限；命中率多来自公司或媒体披露 |
| 百奥几何 BioGeometry | 生成式蛋白设计 | 龙头 / 准龙头 | GeoFlow、GeoBiologics、GeoEnzyme；2026 年完成数亿元战略融资；披露 20+ BD 合作 | 部分性能来自预印本或公司口径；临床和收入兑现仍待观察 |
| 华深智药 Helixon | AI 大分子 / 抗体药物设计 | 龙头候选 | 清华智能产业研究院孵化背景；AI + 高通量实验；海外关联 Earendil Labs 与 Sanofi 有大额合作 | 海外主体与国内主体边界需进一步核验；里程碑金额高度依赖后续临床 |
| 百图生科 BioMap | 生命科学大模型平台 | 平台型头部 | xTrimo、AIGP、BioMap OS；与 Sanofi 共建生物治疗药物 AI 模块，潜在总额超 10 亿美元 | 业务范围很宽，蛋白设计只是模块之一；真实收入和管线兑现未充分透明 |
| 天鹜科技 Matwings | 蛋白质设计大模型 + 自动化实验 | 准龙头 | MatwingsVenus / AccelProtein；A+ 轮超 2 亿元；披露工业蛋白和 5000L 放大生产案例 | 更偏工业蛋白和生物制造，创新药管线证据较少 |

### 3.2 重点公司笔记

#### 分子之心 MoleculeMind

分子之心是国内 AI 蛋白设计中赛道纯度较高的公司之一。公开资料显示，公司围绕 MoleculeOS、NewOrigin、MMDesign 等平台，覆盖蛋白结构预测、复合物预测、蛋白优化、从头设计和动态结合设计，应用场景包括抗体、纳米抗体、酶、小蛋白和疫苗。

值得关注的地方在于，它不是单纯做文献或结构预测工具，而是明确把 AI 设计结果推进到湿实验验证。公开报道中，MMDesign 在多个真实疾病靶点上进行纳米抗体从头设计并披露较高命中率。公司 2026 年 A 轮系列融资累计逾 1 亿美元，产业资本参与度较高。

主要风险是：公开信息仍以公司披露和媒体转述为主，真实客户结构、收入、药物管线、失败样本和可重复验证情况仍不透明。

参考来源：

- [经济参考网：分子之心完成 A 轮系列融资](https://www.jjckb.cn/20260617/705a6e11da4d4c9ea84156a60cb77349/c.html)
- [科技日报：MoleculeOS 相关报道](https://www.stdaily.com/web/gdxw/2025-07/28/content_376661.html)
- [凯赛生物：投资合作公告](https://m.cathaybiotech.com/newsxq.aspx?ID=67)

#### 百奥几何 BioGeometry

百奥几何主打生成式 AI 蛋白设计，技术关键词包括全原子扩散模型、序列-结构-功能联合建模、抗体从头设计、酶和功能蛋白设计。公司官网展示了 GeoFlow、GeoBiologics 和 GeoEnzyme 等平台，并强调高通量湿实验闭环。

从产业信号看，公司在 2026 年完成数亿元战略融资，并披露已与国内外药企达成 20 多项 BD 合作。其优势是模型方向前沿、叙事清晰、融资和合作增长快。

主要风险是：技术指标仍有一部分来自预印本和公司口径，是否能持续转化为付费收入、临床前资产或工业规模化案例，需要继续观察。

参考来源：

- [百奥几何官网：关于我们](https://www.biogeom.com/zh/%E5%85%B3%E4%BA%8E%E6%88%91%E4%BB%AC/)
- [36氪：百奥几何数亿元战略融资](https://m.36kr.com/p/3839626642344454)
- [BioRxiv：GeoFlow-V2 预印本](https://www.biorxiv.org/content/10.1101/2025.05.06.652551.full)
- [义翘神州：与百奥几何合作](https://cn.sinobiological.com/news/sinobiological-biogeometry)

#### 华深智药 Helixon / Earendil Labs

华深智药由清华相关团队孵化，定位为 AI 驱动的大分子和抗体药物设计公司。它的优势不只是模型，而是 AI 与高通量实验的组合。若从“AI 蛋白疗法设计”的角度看，华深智药及其相关海外主体 Earendil Labs 的商业化验证较强。

公开资料显示，华深智药在 2022 年完成近 5 亿元 A 轮融资。Earendil Labs 与 Sanofi 在 2025 年和 2026 年分别披露大额合作，涉及双抗和 AI 蛋白疗法平台合作。

主要风险是：Earendil Labs 是海外主体，其与华深智药之间的股权和业务边界公开信息有限；同时，大额 BD 中很大比例通常是未来或有里程碑，并不等同于已确认收入。

参考来源：

- [华深智药官网](https://www.huashen.bio/)
- [医药魔方：华深智药近 5 亿元 A 轮融资](https://bydrug.pharmcube.com/news/detail/d130fb2d1295119641714bc50c01116b)
- [PR Newswire：Earendil Labs 与 Sanofi 授权合作](https://www.prnewswire.com/news-releases/earendil-labs-announces-worldwide-exclusive-license-agreement-with-sanofi-for-next-generation-bispecific-antibodies-for-autoimmune-and-inflammatory-bowel-diseases-302431020.html)
- [BioPharma Dive：Earendil Labs 融资报道](https://www.biopharmadive.com/news/earendil-labs-financing-ai-biologics-china-sanofi/815336/)

#### 百图生科 BioMap

百图生科是生命科学大模型平台公司，技术体系包括 xTrimo、AIGP、BioMap OS 等，覆盖蛋白、细胞、多组学和生物制剂设计。它是国内生命科学大模型最有国际认知度的公司之一。

与 Sanofi 的合作是重要产业背书。公开公告显示，双方合作开发用于生物治疗药物发现的 AI 模块，潜在交易总额超过 10 亿美元。

主要风险是：BioMap 不是只做蛋白设计，其平台跨度大，蛋白设计只是生命科学大模型的一部分。若评估“纯蛋白设计龙头”，应把它放在平台型头部，而不是单点蛋白设计公司。

参考来源：

- [BioMap 官网：Technology](https://www.biomap.com/technology)
- [BusinessWire：BioMap 与 Sanofi 合作](https://www.businesswire.com/news/home/20231010485897/en/BioMap-Establishes-a-Strategic-Collaboration-with-Sanofi-to-Co-Develop-AI-Modules-to-Accelerate-Drug-Discovery-for-Biotherapeutics)
- [Sanofi：Technology Platforms](https://www.sanofi.com/en/partnering/partnering-focus-areas/technology-platforms)
- [PubMed：xTrimoPGLM 相关论文](https://pubmed.ncbi.nlm.nih.gov/40181110/)

#### 天鹜科技 Matwings

天鹜科技由上海交通大学相关团队创建，聚焦蛋白质设计大模型、AI 定向进化、AI 挖酶、de novo 设计和自动化实验平台。它更偏工业蛋白、酶设计和生物制造落地，而不是传统创新药管线公司。

公开资料显示，公司在 2024 年完成数千万美元 A 轮，2026 年 A+ 轮超过 2 亿元人民币。产业案例中，天鹜科技与金赛药业合作的耐碱蛋白改造和放大生产案例值得关注。

主要风险是：公开命名客户仍有限，且商业落点更偏工业蛋白和生物制造。如果研究重点是抗体药物或创新药管线，需要与分子之心、华深智药、百图生科区别看待。

参考来源：

- [天鹜科技官网](https://www.matwings.com/)
- [36氪：天鹜科技 A+ 轮融资](https://m.36kr.com/newsflashes/3724873893640576)
- [PR Newswire：Matwings Series A](https://www.prnewswire.com/news-releases/matwings-technology-raised-series-a-funding-of-tens-of-millions-usd-to-redefine-protein-design-302339150.html)

### 3.3 观察名单

| 企业 | 说明 |
|---|---|
| 元思生肽 Syneron Bio | 大环肽药物发现平台，融资和阿斯利康合作强，但严格说是多肽 / 环肽细分，不是通用蛋白设计平台 |
| 深势科技 DP Technology | AI4S 基础设施和科学计算平台强，蛋白结构预测、药靶结合和抗体/ADC/TCE 方向有布局，但蛋白设计不是唯一主线 |
| 晶泰科技 XtalPi | 港股上市的 AI + 机器人自动化药物研发平台，蛋白和多肽相关能力值得跟踪，但市场认知更多来自小分子、晶型、自动化等方向 |
| 佰翱得 Biortus | 结构生物学、复杂蛋白制备和蛋白工程服务积累深，AI/ML 蛋白设计是新增能力 |
| 力文所 Levinthal Biotech | 早期潜力公司，围绕共进化机器学习和全原子模型做蛋白设计，客户和融资证据弱于核心梯队 |

---

## 4. 器官芯片企业图谱

### 4.1 核心梯队

| 企业 | 定位 | 头部判断 | 关键证据 | 主要风险 |
|---|---|---|---|---|
| 艾玮得 AVATARGET | 器官芯片、生命科学设备、药效/毒理评价 | 龙头候选 | 恒瑞 HRS-1893 体外筛选中使用心脏器官芯片数据并获批临床；Pre-A 与 Pre-A+ 融资；产品在药企、医院和科研机构应用 | 公司仍年轻，收入和复购未充分披露；监管采信仍在早期 |
| 大橡科技 Daxiang Bio | 类器官芯片产品与药筛服务 | 龙头候选 | IBAC 类器官芯片系列；50+ 试剂盒、100+ 模型；近亿元融资；药明康德等投资背景 | 很多 IND / 头部药企信息来自公司口径；临床药敏一致性需更大规模验证 |
| 耀速科技 Xellar Biosystems | 高通量器官芯片 + AI | 龙头 / 准龙头 | HTS Organ-on-Chip + 3D imaging + AI；辉瑞、赛诺菲等合作线索；晶泰科技战略投资 | 中美双布局，不是纯本土起步；AI/标准制定等表述需要进一步第三方验证 |
| 丹望医疗 D1Med | 类器官模型库 + 类器官芯片 | 龙头 / 准龙头 | 血管芯片、肺芯片、屏障芯片；直肠癌类器官 Cell Stem Cell 研究；服务药企和 IND 支撑线索 | 更偏类器官平台，不是纯器官芯片公司；患者药敏商业化受监管和支付影响 |

### 4.2 重点公司笔记

#### 艾玮得 AVATARGET

艾玮得成立于 2021 年，源自东南大学苏州医疗器械研究院和相关生物电子学团队。公司方向包括人体器官芯片、生命科学设备、生物试剂，以及药物功效和安全性评价。

它最值得关注的公开证据，是心脏器官芯片数据进入药物临床申报支撑链条。新华网报道中，恒瑞医药 HRS-1893 项目在体外筛选中使用了心脏器官芯片数据并获批临床。这类案例对器官芯片赛道很关键，因为它把模型从科研工具推进到药物研发决策和监管证据链。

主要风险是：器官芯片在国内新药申报中多数仍属于补充证据，离广泛替代动物实验还有距离。公司收入、客户复购和批量化交付能力也需要持续跟踪。

参考来源：

- [艾玮得官网](https://www.avatarget.com.cn/)
- [新华网：器官芯片支撑恒瑞项目筛选](https://www.news.cn/health/20230710/898b756726754c54b2be1bc92beef682/c.html)
- [丁香通：艾玮得 Pre-A+ 融资](https://www.biomart.cn/news/16/3210548.htm)
- [东南大学苏州医疗器械研究院：公司孵化背景](https://ibmd.seu.edu.cn/2022/0802/c19023a415015/pagem.htm)

#### 大橡科技 Daxiang Bio

大橡科技成立较早，是国内类器官芯片产品化代表。公司产品包括 IBAC S1、M1、O1、O2 等类器官芯片，覆盖 3D 高通量培养、屏障功能、多器官共培养和动态培养等场景。

公司公开资料显示，它已开发 50 多种类器官培养试剂盒和 100 多种人源化模型，并将服务延伸到药效、DMPK、早期毒性评价和精准医疗。大橡还获得过药明康德等产业方投资，说明其商业化路线获得过药企生态认可。

主要风险是：公司披露的药企管线和 IND 申报应用需要逐项核验。类器官药敏与临床疗效的一致性，也需要更大规模前瞻性研究支撑。

参考来源：

- [大橡科技官网：器官芯片产品](https://www.daxiangbio.cn/organs-on-chips.html)
- [大橡科技官网：药物研发服务](https://www.daxiangbio.cn/preclinical.html)
- [大橡科技新闻：模型与试剂盒能力](https://www.daxiangbio.cn/news/199.html)
- [36氪项目库：大橡科技](https://pitchhub.36kr.com/project/1678369341731840)

#### 耀速科技 Xellar Biosystems

耀速科技定位为高通量器官芯片和 AI 公司，技术组合包括 3D 生物模型、器官芯片、高内涵成像、计算机视觉和 AI 分析。它的路线更像“下一代临床前数据基础设施”，而不是单纯销售芯片耗材。

公开资料显示，耀速科技曾完成千万美元天使轮、亿元级天使+轮，并在 2025 年获得晶泰科技领投的战略融资。公开报道还提到其与辉瑞、赛诺菲等国际药企在毒理、血管毒性模型等方向的合作。

主要风险是：耀速科技中美双布局，严格来说不完全是纯本土起步公司；另外，AI 毒理预测和高通量器官芯片的真实交付、同行评议论文和监管项目仍需继续验证。

参考来源：

- [耀速科技官网](https://xellarbio.com/)
- [耀速科技技术页](https://xellarbio.com/technology/)
- [鼎泰集团：耀速科技融资与合作](https://zh.tri-apex.com/info/news/headlines/655.html)
- [证券时报：晶泰科技领投战略融资](https://www.stcn.com/article/detail/1733756.html)
- [上海奉贤政府：耀速科技相关报道](https://www.fengxian.gov.cn/gzms/20250624/91241.html)

#### 丹望医疗 D1Med

丹望医疗更偏类器官模型库和类器官芯片融合平台。公司官网列出血管芯片、肺芯片、屏障芯片、类器官库、药筛和毒理评价服务。

丹望医疗的优势是类器官临床验证和模型库能力。公开资料显示，公司在 2021 年完成 1.2 亿元 A 轮融资；其直肠癌类器官研究发表于 Cell Stem Cell，并披露了较高的疗效预测准确度。公司也有服务药企和辅助 IND 的公开线索。

主要风险是：丹望医疗的核心更像类器官平台，而不是纯器官芯片平台。若项目重点是微流控器官芯片，需将其与艾玮得、大橡、耀速区分。

参考来源：

- [丹望医疗官网](https://www.d1med.com/)
- [丹望医疗：A 轮融资](https://d1med.com/show-23-7-1.html)
- [丹望医疗：学术成果](https://www.d1med.com/show-24-11-1.html)
- [医药魔方：国家重点研发计划与药企服务](https://bydrug.pharmcube.com/news/detail/f90a4c3e711d07a87cfd9fdfc7fa76d9)

### 4.3 观察名单

| 企业 | 说明 |
|---|---|
| 创芯国际 | 类器官全产业链和样本/模型库能力较强，但公开资料显示“类器官”属性强于“器官芯片”属性 |
| 黑玉科学 | 类器官智能设备、自动化、芯片和 AI 制造方向，偏底层设备和标准化供给 |
| 骆华生物 | 类器官芯片模型库型公司，模型覆盖面较广，但药企客户、论文和监管采信证据相对有限 |
| 逸芯生命科学 | AI + 器官芯片 / MPS 早期玩家，方向正但公司阶段较早 |
| 诺善科技 | 肺癌药敏微流控类器官芯片方向，已有协和前瞻性队列线索，但仍是早期专项型公司 |

---

## 5. 不宜误判为细分赛道龙头的公司类型

| 类型 | 代表 | 为什么要谨慎 |
|---|---|---|
| 广义 AI 制药公司 | 晶泰科技、英矽智能 | 它们很强，但核心证据更多在小分子、靶点发现、晶型、自动化或药物发现全流程 |
| 抗体发现 / CRO 公司 | 百奥赛图、三优生物、百英生物、义翘神州 | 抗体是蛋白药物，但抗体发现平台不等同于 AI 从头蛋白设计平台 |
| 合成生物公司 | 恩和科技、凯赛生物、华恒生物、蓝晶微生物 | 酶工程与蛋白设计相关，但商业主线通常是生物制造、菌株和细胞工厂 |
| 微流控工具商 | 傲睿科技、顶旭微控、泰初科技等 | 是器官芯片上游工具，但不一定拥有器官模型和药筛验证平台 |
| 大型 CRO | 药明康德、康龙化成、美迪西、鼎泰、皇冠生物 | 可能具备药筛或类器官服务，但 CRO 能力不等于器官芯片底层平台 |

---

## 6. 对 Frontis AI4Sci 的启发

### 6.1 不建议直接复制的方向

不建议把 Frontis 的 AI4Sci 第一阶段定义为：

1. 再做一个纯蛋白生成模型公司；
2. 再做一个器官芯片湿实验平台；
3. 再做一个类器官药筛 CRO；
4. 再做一个广义 AI 制药平台；
5. 再做一个 ELN / LIMS / 文献 RAG 工具。

这些方向都有专业玩家，且需要大量实验、BD、监管、平台和行业积累。

### 6.2 更适合 Frontis 的切入点

Frontis 更适合切入 **Science Agent Evolution Infrastructure**：

```text
蛋白质设计公司
  提供候选生成、结构预测、亲和力优化、抗体/酶/多肽设计能力

器官芯片 / 类器官芯片公司
  提供人体相关 phenotype、toxicity、mechanism、safety reward

Frontis AI4Sci
  连接目标调研、候选设计、专家 review、实验计划、结果解析、失败复盘和 Agent 训练
```

也就是说，Frontis 可以把这些公司视为：

- **潜在工具供应商**：调用其设计、筛选、模型或实验能力；
- **潜在数据和 reward 来源**：把 wet-lab / organ-chip readout 编译成 reward vector；
- **潜在客户或合作伙伴**：为其提供科研 Agent、项目记忆、实验决策和训练数据基础设施；
- **竞品参照**：避免把自身定位落到单点模型或单点实验平台。

### 6.3 推荐的第一个 wedge

建议继续采用当前主方案中的 **Target-to-Binder Research & Design Loop**：

1. target / disease / pathway 调研；
2. 证据图谱和 Target Card；
3. 调用外部或内部蛋白设计工具生成候选；
4. 计算筛选和专家 review；
5. 小规模 wet validation；
6. 器官芯片或类器官芯片提供 phenotype / toxicity / mechanism reward；
7. 将失败、专家判断和实验结果沉淀为 Scientific Memory 与训练样本。

这个切入点可以绕开“和蛋白设计公司正面拼模型”以及“重资产自建器官芯片平台”的问题，把 Frontis 的核心壁垒落在科研任务编排、专家协作、轨迹数据、reward ledger 和 Agent 进化上。

---

## 7. 后续跟踪清单

### 7.1 蛋白质设计方向

- 分子之心：是否披露更多客户、付费项目、论文、失败样本和临床前资产。
- 百奥几何：GeoFlow / GeoBiologics 是否有同行评议论文和更多真实 BD 兑现。
- 华深智药 / Earendil Labs：Sanofi 合作资产是否进入临床，国内外主体边界是否更清晰。
- 百图生科：Sanofi 合作的阶段性成果和 xTrimo 生态的真实使用情况。
- 天鹜科技：工业蛋白项目是否形成规模化收入，是否扩展到创新药和治疗性蛋白。

### 7.2 器官芯片方向

- 艾玮得：是否有更多 IND 支撑案例和监管采信案例。
- 大橡科技：类器官芯片是否形成标准化产品销售和药企复购。
- 耀速科技：辉瑞、赛诺菲等合作是否有论文、产品或真实药物研发决策输出。
- 丹望医疗：类器官临床预测能力是否有更大规模前瞻性验证。
- 行业整体：CDE / NMPA 对类器官、器官芯片和 MPS 数据的指导原则变化。

---

## 8. 关键来源索引

### 蛋白质设计

- 分子之心融资与平台：[经济参考网](https://www.jjckb.cn/20260617/705a6e11da4d4c9ea84156a60cb77349/c.html)、[科技日报](https://www.stdaily.com/web/gdxw/2025-07/28/content_376661.html)、[凯赛生物](https://m.cathaybiotech.com/newsxq.aspx?ID=67)
- 百奥几何：[官网](https://www.biogeom.com/zh/%E5%85%B3%E4%BA%8E%E6%88%91%E4%BB%AC/)、[36氪](https://m.36kr.com/p/3839626642344454)、[GeoFlow-V2](https://www.biorxiv.org/content/10.1101/2025.05.06.652551.full)
- 华深智药：[官网](https://www.huashen.bio/)、[医药魔方](https://bydrug.pharmcube.com/news/detail/d130fb2d1295119641714bc50c01116b)、[PR Newswire](https://www.prnewswire.com/news-releases/earendil-labs-announces-worldwide-exclusive-license-agreement-with-sanofi-for-next-generation-bispecific-antibodies-for-autoimmune-and-inflammatory-bowel-diseases-302431020.html)
- 百图生科：[官网](https://www.biomap.com/technology)、[BusinessWire](https://www.businesswire.com/news/home/20231010485897/en/BioMap-Establishes-a-Strategic-Collaboration-with-Sanofi-to-Co-Develop-AI-Modules-to-Accelerate-Drug-Discovery-for-Biotherapeutics)、[Sanofi](https://www.sanofi.com/en/partnering/partnering-focus-areas/technology-platforms)
- 天鹜科技：[官网](https://www.matwings.com/)、[36氪](https://m.36kr.com/newsflashes/3724873893640576)、[PR Newswire](https://www.prnewswire.com/news-releases/matwings-technology-raised-series-a-funding-of-tens-of-millions-usd-to-redefine-protein-design-302339150.html)

### 器官芯片

- 艾玮得：[官网](https://www.avatarget.com.cn/)、[新华网](https://www.news.cn/health/20230710/898b756726754c54b2be1bc92beef682/c.html)、[丁香通](https://www.biomart.cn/news/16/3210548.htm)、[东南大学苏州医疗器械研究院](https://ibmd.seu.edu.cn/2022/0802/c19023a415015/pagem.htm)
- 大橡科技：[器官芯片产品](https://www.daxiangbio.cn/organs-on-chips.html)、[药物研发服务](https://www.daxiangbio.cn/preclinical.html)、[公司新闻](https://www.daxiangbio.cn/news/199.html)、[36氪项目库](https://pitchhub.36kr.com/project/1678369341731840)
- 耀速科技：[官网](https://xellarbio.com/)、[技术页](https://xellarbio.com/technology/)、[鼎泰集团](https://zh.tri-apex.com/info/news/headlines/655.html)、[证券时报](https://www.stcn.com/article/detail/1733756.html)、[奉贤政府](https://www.fengxian.gov.cn/gzms/20250624/91241.html)
- 丹望医疗：[官网](https://www.d1med.com/)、[A 轮融资](https://d1med.com/show-23-7-1.html)、[学术成果](https://www.d1med.com/show-24-11-1.html)、[医药魔方](https://bydrug.pharmcube.com/news/detail/f90a4c3e711d07a87cfd9fdfc7fa76d9)

