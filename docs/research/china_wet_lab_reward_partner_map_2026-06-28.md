# 中国湿实验 Reward Source 与合作伙伴地图

**调研日期**：2026-06-28  
**用途**：Frontis AI4Sci / Scientific MA 的 wet-lab partner map  
**核心问题**：寻找可作为工具供应商、实验数据/reward 来源、潜在客户或合作伙伴的公司与机构，而不是寻找 AI 叙事最强的公司。  
**结论口径**：本报告基于公开资料与 sub-agent 并行调研，重点评估“能否稳定产出高质量、可追溯、可训练的湿实验数据”。公开资料无法证明供应商愿意交付失败样本、原始曲线、完整元数据和模型训练权，因此这些条款必须通过试单和合同尽调确认。

---

## 0. Executive Summary

Frontis 当前真正需要的是 **wet-lab reward network**，而不是再找一批 AI 模型公司。合作对象应按实验闭环拆成四类：

1. **蛋白/抗体快速验证工厂**：把 AI 设计序列转成表达、纯化、binding、developability 和功能 readout。
2. **标准 reagent 与 QC 供应商**：提供 target protein、抗原、FcR、MHC/TCR、膜蛋白、SPR/BLI assay 等可重复基线。
3. **表型/毒理 reward source**：用类器官、器官芯片、PDX/PDO、高内涵成像、毒理/DMPK 输出 phenotype / toxicity / mechanism reward。
4. **高校医院/国家平台**：提供高密度、方法学先进、临床样本或结构生物学 readout，适合共建而不是简单外包。

建议第一批优先接触：

| 目的 | 第一批候选 | 用法 |
|---|---|---|
| 抗体/纳米抗体序列验证 | **百英生物 Biointron、金斯瑞 GenScript、药明生物 WuXi Biologics** | 50-300 条候选序列表达、binding、developability、小规模功能验证 |
| 困难靶点与标准 QC | **义翘神州、百普赛斯、近岸蛋白、KACTUS** | target reagent、cross-reactivity panel、SPR/BLI 交叉验证 |
| 体内抗体/纳米抗体资产与动物模型 | **百奥赛图 Biocytogen** | 难靶点、纳米抗体、双抗/ADC 的平台共研或数据授权 |
| 肿瘤类器官/PDX/PDO reward | **冠科生物 Crown Bioscience、科途医学 K2、丹望医疗 D1Med** | oncology benchmark、PDO 药敏、免疫共培养、药效机制 |
| 器官芯片/高维表型/毒理 | **耀速科技 Xellar、大橡科技、艾玮得** | 高内涵图像、MPS/器官芯片毒理、动态培养、DILI/心毒/肾毒 |
| IND/GLP 后期补强 | **美迪西、昭衍新药、康龙化成、药明康德 Biology** | DMPK、GLP 安评、体内药效、IND-enabling package |
| 共建型科研平台 | **国家蛋白质设施、iHuman、深圳湾实验室、东南大学器官芯片、复旦肿瘤、华西医院** | 结构、药筛、临床样本、类器官/OoC 方法学共建 |

最关键的合作条款不是价格，而是 **raw reward**：

- 每个样本的序列、构建设计、表达失败原因、产量、纯度、SEC monomer、浓度、Tm、内毒素；
- KD / kon / koff 原始曲线、表位分箱、竞争 binding、细胞功能读数；
- 类器官/器官芯片原始图像、孔级 metadata、剂量反应曲线、IC50/AUC、毒理 biomarker、组学数据；
- 阳性/阴性对照、失败样本、批次号、试剂/仪器/SOP 版本、复测规则；
- Frontis 对数据、负样本和衍生模型的训练使用权。

---

## 1. 筛选框架

### 1.1 评分维度

| 维度 | 权重 | 评估要点 |
|---|---:|---|
| 数据质量 / QC / 可复现 | 20 | SOP、批间一致性、阳性/阴性对照、复测率、原始数据可追溯 |
| 通量 / 自动化 / 周转 | 15 | 96/384/1536 孔、液体处理、高内涵成像、月产能、TAT |
| Reward vector 密度 | 15 | 连续表型、剂量曲线、动力学、组学、失败原因，而不是只给 yes/no |
| 失败样本 / 负数据可得性 | 12 | no-expression、低纯度、聚集、污染、建模失败、无响应样本是否结构化交付 |
| Assay 相关性 | 13 | 蛋白：表达-纯化-表征-功能；类器官：PDO/PDXO/芯片/共培养/毒理 |
| 数据治理 / Agent 接入 | 10 | LIMS/ELN、条码、API/SFTP、批量导出、元数据字典、审计日志 |
| 合规与质量体系 | 8 | GLP/ISO/CLIA、人遗/伦理/知情同意、临床样本链路 |
| 商务/IP/合作适配 | 7 | 共建 SOP、训练数据权利、排他限制、响应速度 |

### 1.2 一票否决问题

以下任一项不能满足，应降级为普通供应商，而不是 reward source：

1. 只交 PDF 报告，不交原始数据、处理后数据和 QC；
2. 不交失败样本和阴性样本；
3. 不记录 SOP 版本、批次号、试剂批号、仪器参数；
4. 不允许 Frontis 将实验数据用于内部模型训练和评估；
5. 人源样本没有清晰 IRB、知情同意、人遗和数据合规边界；
6. 无法做盲测 pilot、跨批复测和固定对照。

---

## 2. 蛋白/抗体湿实验 Partner Map

### 2.1 第一梯队：抗体/纳米抗体闭环验证

| 候选 | 适合定位 | 核心湿实验能力 | 可产出 reward vector | 合作接口 | 风险 |
|---|---|---|---|---|---|
| **百英生物 Biointron** | 抗体/纳米抗体变体快速验证工厂 | 高通量抗体表达、AbDrop 单 B、纳米抗体、人源化、亲和力成熟、ADC 高通量偶联、developability | 表达成功率、表达量、binding/cell binding、affinity、epitope binning、热稳定性、聚集、developability | 50-300 条 AI 设计抗体/纳米抗体的快速表达 + binding + developability pilot | 非 GLP/IND 主力；需确认 raw curve、阴性数据、QC failure 是否交付 |
| **金斯瑞 GenScript / ProBio** | 序列到蛋白/抗体的标准化外包循环 | 基因合成、蛋白/抗体表达、cell-free protein synthesis、hybridoma/phage/yeast display、SPR/BLI | 序列可合成性、表达成功率、产量、可溶性、BLI/SPR binding、hit rate | 大规模探索批次；“设计序列 -> 下单 -> 表达 -> 初筛” | 标准服务强，深度共研需定制 SOW；数据权利要提前写清 |
| **药明生物 WuXi Biologics** | 高可信 design-to-IND 验证 | Hybridoma、single B、phage/yeast display、VHH、蛋白工程、SPR/BLI、体外 bioassay、CMC/IND | 表达量、纯度/聚集、KD/kon/koff、表位分箱、dual binding、FcR、细胞 potency、CMC developability | 少量高价值候选物的标准化确认与后续 IND 路线 | 成本高、周期长；数据/IP 和地缘风险需合同处理 |
| **百奥赛图 Biocytogen** | 体内抗体/纳米抗体平台共研 | RenMab/RenLite/RenNano/RenTCR 全人抗体和纳米抗体小鼠、靶点人源化动物、药效模型 | 体内免疫产生的序列-表位-亲和力、交叉反应、体内药效、安全性初筛 | 难靶点、纳米抗体、双抗/ADC 早期资产共研或数据授权 | 更像资产合作，不是便宜外包；靶点排他和里程碑复杂 |

参考来源：

- [Biointron 官网](https://www.biointron.com.cn/)、[Biointron developability](https://www.biointron.com/antibody-developability/antibody-developability-assessment.html)
- [GenScript 2025 业绩](https://www.genscript.com/genscript-biotech-announces-2025-results.html)、[GenScript BLI/SPR](https://www.genscript.com/bli-spr-real-time-affinity-measurement-services.html)、[GenScript hit generation](https://www.genscript.com/hit-generation-screening.html)
- [WuXi Biologics 抗体发现](https://www.wuxibiologics.com/antibody-discovery-services/)、[WuXi Biologics SPR/BLI](https://www.wuxibiologics.com/cro-services/spr-bli-binding-assays-services/)
- [Biocytogen 官网](https://biocytogen.com.cn/about-us/about-the-company)、[RenNano 授权](https://biocytogen.com/news/Biocytogen-Grants-Taisho-Pharmaceutical-a-License-to-its-RenNano-Fully-Human-Heavy-Chain-Only-Antibody-Discovery-Platform)

### 2.2 第二梯队：标准 target、reagent、binding assay 与 QC

| 候选 | 适合定位 | 核心湿实验能力 | 可产出 reward vector | 合作接口 | 风险 |
|---|---|---|---|---|---|
| **义翘神州 Sino Biological** | 标准 target protein / reagent / assay feasibility | 重组蛋白、抗体、基因、培养基、蛋白/抗体开发、生物分析检测 | 抗原表达成功率、蛋白活性、KD/kinetics、批间一致性、ELISA/SPR/BLI assay feasibility | 标准 target panel、FcR/细胞因子/受体 reagent、交叉验证 | Catalog 与技术服务强，深度功能筛选不是核心 |
| **百普赛斯 ACROBiosystems** | 药物开发关键试剂与 binding assay | 重组蛋白、GMP 级关键试剂、SPR/BLI、抗独特型抗体、假病毒中和、FACS/SEC-MALS | binding kinetics、Fc/FcR、C1q、细胞染色、蛋白聚集/纯度、病毒中和 | Cross-reactivity panel、QC assay 包、标准化 reagent | 大规模负样本和训练权需商务谈判 |
| **近岸蛋白 Novoprotein** | 本土蛋白/酶/抗原快速验证 | 蛋白表达纯化、SPR/BLI、抗体/重组抗体、酶和试剂、RNA/疫苗/CGT 原料 | 表达量、纯度、活性、binding、抗体筛选、抗原/抗体应用验证 | 蛋白/酶/抗原工程的本土快速验证 | 抗体 discovery 深度不如百英/百奥赛图 |
| **KACTUS 恺佧生物** | 难表达 target 与膜蛋白 reagent | VLP/nanodisc 膜蛋白、MHC 复合物、TCR、GMP gene-editing enzymes、SPR | 难表达靶点成功率、膜蛋白构象/活性、SPR KD、MHC/TCR binding、酶活 | GPCR、多跨膜蛋白、MHC/TCR 等困难 antigen 与 assay reagent | 私营信息透明度有限，项目级失败数据不一定可得 |
| **维亚生物 Viva Biotech** | 结构生物学与难靶点机制反馈 | 蛋白生产、结构生物学、cryo-EM、膜蛋白/复合物、SBDD | 结构模型、复合物界面、biophysical binding、构象状态 | 难靶点、结构反馈、cryo-EM / X-ray 机制验证 | 更偏结构和小分子 CRO，蛋白疗法闭环需配套 |

参考来源：

- [Sino Biological 技术平台](https://www.sinobiological.com/services/platform)、[Sino Biological SPR/BLI](https://www.sinobiological.com/services/spr-bli-assay-services)
- [ACROBiosystems SPR](https://www.acrobiosystems.cn/services/spr)、[ACROBiosystems BLI](https://www.acrobiosystems.cn/services/bli)
- [Novoprotein 官网](https://www.novoprotein.com.cn/)、[Novoprotein 服务](https://www.novoprotein.com/service-list)
- [KACTUS 官网](https://kactusbio.com/)、[KACTUS SPR](https://kactusbio.com/pages/surface-plasmon-resonance-spr-services)
- [Viva Biotech 结构生物学服务](https://www.vivabiotech.com/cro/structuralbiologyservices)

### 2.3 下游功能、DMPK、毒理与 IND/GLP 补强

| 候选 | 适合定位 | 核心能力 | 可产出 reward vector | 合作接口 | 风险 |
|---|---|---|---|---|---|
| **药明康德 Biology / WuXi Biology** | 综合 discovery 与方法学开发 | 蛋白科学、SPR/nanoDSF/DSF/ITC、结构生物学、HTS、ASMS、DEL、细胞/体内药理 | 热稳定性、binding、结构、biochemical/cell potency、target tractability | 方法学开发、结构/生物物理验证、细胞功能 assay | 小分子和综合 discovery 更强，蛋白 therapeutic 连续闭环需配套 |
| **美迪西 Medicilon** | IND-enabling 验证 | 药效、DMPK、毒理、安全性评价、CMC、IND package、GLP 实验室 | PK/PD、毒理、免疫原性、药效模型、NOAEL、IND acceptability | Lead 确认后的 IND-enabling 验证 | 不适合早期大规模序列迭代 |
| **昭衍新药 JOINN** | GLP 安评和法规毒理 | 非临床安全评价、药效、药代、免疫毒性/免疫原性、DART、安全药理 | 安全窗、免疫毒性、PK/PD、体内药效、监管可接受性 | 候选蛋白/抗体临床前安全性验证 | 下游验证为主，不产生高频设计 reward |
| **康龙化成 Pharmaron** | DMPK/ADMET 与临床前补强 | DMPK、体外/体内药效、ADMET、PDX organoid / ADC testing 等 | PK/PD、ADMET、药效、ADC/biologics 功能验证 | 与器官芯片或类器官伙伴搭配，补 IND/GLP 路线 | 大型 CRO，数据开放和训练权需强合同 |
| **冠科生物 Crown Bioscience** | 肿瘤生物药/ADC/TCE 功能验证 | PDX/PDO/PDXO、肿瘤/IO、off-target binding cell microarray、ADC/biologics lead selection | 类器官 response、off-tumor binding、ADC efficacy、biomarker、PD/efficacy correlation | 肿瘤抗体、ADC、TCE、细胞因子类候选物功能验证 | 不是表达/纯化供应商；适用范围偏肿瘤转化 |

参考来源：

- [WuXi Biology biophysics](https://discoverybiology.wuxiapptec.com/solution-biophysics)、[WuXi Biology target-to-hit](https://wuxibiology.com/solutions/phase/hit-finding/)
- [Medicilon 官网](https://medicilon.com/)、[Medicilon 2025 回顾](https://medicilon.com/medicilon-2025-year-end-review/)
- [JOINN 昭衍官网](https://www.joinnlabs.com/)
- [Pharmaron DMPK](https://www.pharmaron.cn/services/biosciences/dmpk-for-discovery-preclinical-development)
- [CrownBio 官网](https://www.crownbio.com/zh-cn/)、[CrownBio ADC/biologics lead selection](https://www.crownbio.com/target/to-lead-selection-for-adcs-and-biologics)

### 2.4 酶设计与工业蛋白 reward

| 候选 | 适合定位 | 核心能力 | 可产出 reward vector | 风险 |
|---|---|---|---|---|
| **恩和生物 Bota Bio** | 工业酶和生物制造闭环 | Biofoundry、蛋白/酶迭代筛选、菌株工程、发酵放大 | enzyme activity、selectivity、titer、yield、COGS、发酵稳定性 | 平台封闭，医药 GLP 相关性弱 |
| **弈柯莱 Abiochem** | 酶库与高通量酶筛选 | ProRD、实体酶库、自动化高通量筛选、底盘细胞与发酵筛选 | 酶活、选择性、稳定性、底物转化率、发酵产量 | 偏产业化合成生物学，客户/项目集中度需审计 |
| **中科院天津工业生物技术所** | 共建型酶工程平台 | 自动化基因编辑、蛋白纯化表征、代谢物检测、液滴微流控筛选 | 突变体适应度、酶活、表达量、代谢产物、发酵 readout | 偏工业生物和合成生物，临床药物弱一些 |

参考来源：

- [Bota Bio 官网](https://bota.bio/)、[Bota Bio 酶工程](https://bota.bio/cn/%E9%85%B6%E5%B7%A5%E7%A8%8B%E5%BF%AB%E9%80%9F%E8%BF%AD%E4%BB%A3%E4%BC%98%E5%8C%96/)
- [Abiochem 官网](https://www.abiochem.com/9.html)
- [中科院天津工业生物技术所高通量平台](https://tib.cas.cn/kjpt/gtlsxybjpt/)

---

## 3. 类器官 / 器官芯片 / 表型毒理 Partner Map

### 3.1 第一梯队：高维 phenotype reward

| 候选 | 适合定位 | 核心湿实验能力 | 可产出 reward vector | 合作接口 | 风险 |
|---|---|---|---|---|---|
| **耀速科技 Xellar Biosystems** | 高通量器官芯片 + 3D HCI reward source | 高通量器官芯片、自动化灌流培养、3D 高内涵成像；肿瘤芯片、PDO+免疫共培养、血管化模型、DILI 肝芯片、肾/血管毒性模型 | 3D 形态学 HCI、多染色、活细胞响应、免疫浸润、毒性/药效表型、多组学 | 共建 Agent 自动提出实验、湿实验执行、图像/组学回流 pilot | AI 叙事强，需锁定 raw image、QC、重复数、批次效应；中美双地合规需确认 |
| **冠科生物 Crown Bioscience** | 肿瘤 PDO/PDXO/PDX benchmark | PDO/PDXO/PDX/CDX、3D ex vivo patient tissue、免疫共培养、高内涵成像、DMPK/PKPD/生物标志物 | IC50、AUC、CTG 活力、HCI 形态、WES/RNA-seq、IHC/IF/mIF、流式、ELISA/MSD/Luminex、空间组学 | Oncology benchmark 数据集、肿瘤生物药/ADC/TCE 功能验证 | 强项偏肿瘤药效，器官芯片和动态生理毒理不如 Xellar/大橡/丹望 |
| **大橡科技 Daxiang Bio** | 国产类器官芯片闭环 | 类器官芯片、单器官/多器官/屏障模型、类器官建系、DMPK、早期毒性、肿瘤药敏、靶免联合药敏 | 明场跟踪、细胞活力、肝毒/肾毒、CYP/转运体、代谢稳定性、临床药敏、免疫微环境响应 | 类器官芯片 + 药筛 + 毒理的国内共建平台 | 商业材料较强，需实测模型 CV、临床一致性、免疫共培养稳定性 |
| **丹望医疗 D1Med** | 临床相关 PDO + 类器官芯片 | 类器官疾病模型库、类器官芯片、药筛、毒理、免疫共培养；血管、肺、肾/肠屏障芯片 | 类器官计数/面积、实时成像、活力、ELISA 细胞因子、WES/RNA-seq、IHC/IF、免疫细胞杀伤/迁移/浸润 | PDO 模型库、模型定制、药筛和毒评 | 需核验 GLP/IND 级质量体系、样本授权链和历史客户 |
| **科途医学 K2 Oncology** | 肿瘤类器官药敏与临床样本 | 肿瘤类器官建模、鉴定、HTS、药效评价、精准药敏；覆盖多癌种 | CellTiter-Glo 3D ATP、IC50/EC50、最大抑制率、协同效应、FISH/WES/RNA-seq、明场图像 | 患者来源药敏、临床样本和新药客户网络 | 偏肿瘤药效/药敏，毒理和器官芯片需外部补强 |

参考来源：

- [Xellar efficacy/toxicity models](https://xellarbio.com/drug-efficacy-and-disease-modeling/)、[Xellar E-P-IC platform](https://xellarbio.com/e-p-ic-platform/)
- [CrownBio drug efficacy testing](https://www.crownbio.com/zh-cn/drug-efficacy-testing)、[CrownBio organoids](https://www.crownbio.com/zh-cn/model-systems/in-vitro/organoids)、[OrganoidXplore](https://www.crownbio.cn/press/crown-bioscience-introduces-organoidxplore/)
- [大橡科技模型与服务](https://www.daxiangbio.cn/research/116.html)、[大橡临床前药效](https://www.daxiangbio.cn/preclinical/40.html)、[大橡 DMPK/毒理](https://www.daxiangbio.cn/preclinical/41.html)
- [D1Med 毒理模型](https://www.d1med.com/list-105-1.html)、[D1Med 药筛服务](https://www.d1med.com/list-103-1.html)
- [K2 Oncology 类器官建模](https://k2oncology.cn/k2item/technology-services-organoid-modeling-and-identification/)、[K2 高通量药筛](https://k2oncology.cn/k2item/technology-services-organoid-based-high-throughput-drug-screening/)

### 3.2 第二梯队：专项器官芯片、区域样本库与精准医疗

| 候选 | 适合定位 | 核心能力 | 可产出 reward vector | 风险 |
|---|---|---|---|---|
| **艾玮得 AVATARGET** | 标准化芯片 + 设备 + 专病毒理 | 心脏器官芯片、肝毒理、皮肤模型、药物功效/安全性评价、高内涵分析系统与灌流设备 | 心毒、肝毒、皮肤刺激/光毒/功效、动态培养 readout | 需确认是否按 CRO 项目交付原始实验数据，而不是只卖产品 |
| **骆华生物 Luohua Bio** | 类器官 + 器官芯片模型库 | 肿瘤、肠、肝、肺、肾、神经、血管等芯片模型；肿瘤药敏和病理 | 药敏、病理、荧光成像、疾病模型 readout | 公开资料多来自案例/新闻，需补官网、客户和 QC 尽调 |
| **华医再生** | 区域类器官样本库与精准医疗 | 类器官样本库、精准医疗、药物筛选、科研模型 | 肿瘤类器官药敏、高通量药筛、药物毒性筛查 | 公开技术参数和药企客户较少 |
| **希格生科 Signet** | 特定肿瘤机制 reward | 类器官疾病模型、药效评价、新靶点发现和内部管线 | 特定靶点机制、药效和 biomarker readout | 主业是自研药，不是中立 CRO，需确认外部服务边界 |
| **粤港澳大湾区精准医学研究院类器官与细胞治疗平台** | 非公司化共建平台 | 肿瘤类器官个性化用药、样本库高通量药筛、人源高仿真类器官用于细胞治疗药物评价 | 药敏、细胞治疗评价、临床样本关联 readout | 合作周期、样本合规和 IP 边界需提前设计 |

参考来源：

- [AVATARGET 官网](https://www.avatarget.com.cn/)、[新华网恒瑞案例](https://www.news.cn/health/20230710/898b756726754c54b2be1bc92beef682/c.html)
- [骆华生物案例](https://www.keyence.com.cn/ss/products/microscope/bz-casestudy/interview-organoid-research.jsp)、[武汉政府报道](https://www.wuhan.gov.cn/sy/whyw/202406/t20240619_2417810.shtml)
- [华医再生](https://www.huayizaisheng.com/list/7.html)
- [Signet 希格生科](https://www.signettx.com/about/)
- [粤港澳大湾区精准医学研究院类器官平台](https://www.ipm-gba.org.cn/Index/customize_details/model_id/16/cid/24/id/171.html)

---

## 4. 高校、医院与国家平台

这些机构不一定适合做标准外包供应商，但适合共建高价值 reward 方法学、标准数据集或样本/结构平台。

| 机构/团队 | 平台能力 | 可产出 readout | 适合 Frontis 的合作方式 | 潜在限制 |
|---|---|---|---|---|
| **国家蛋白质科学研究（上海）设施** | 蛋白制备、晶体学、冷冻电镜、NMR、SAXS、质谱、动态结构、结构药筛 | 结构、结合模式、亲和力、MS/蛋白组、抗体-靶点机制 | 高质量结构和机制 reward；困难靶点结构解析 | 机时排队，样品质量要求高 |
| **国家蛋白质科学中心（北京）/清华蛋白质研究技术中心** | 冷冻电镜、X-ray、蛋白制备、NMR、组学、计算、细胞功能 | cryo-EM map、结构模型、蛋白表达纯化、互作/功能数据 | 结构生物学方法学共建 | 更偏基础平台，转化药筛需另配团队 |
| **上海科技大学 iHuman** | GPCR 结构生物学、分子药理、HTS、质谱、NMR、AI/计算 | GPCR 配体活性、信号偏向性、结构、药理曲线 | GPCR/膜蛋白方向的深度闭环 | 靶点集中在 GPCR 等方向 |
| **中科院上海药物所国家新药筛选中心** | 国家级化合物库、分子/细胞 HTS、筛选模型 | hit rate、IC50/EC50、SAR、细胞表型 | 药筛 reward 和 assay 方法学 | 化合物/IP 边界需前置约定 |
| **中国医学科学院药物研究所国家药物筛选中心** | 靶点发现、分子/细胞高通量药筛、药物发现模型 | 靶点验证、细胞活性、筛选命中、药效初筛 | 医科院体系药理药效共建 | 开放合作节奏可能偏项目制 |
| **深圳湾实验室转化医学中心** | 1536 孔超高通量筛选、百万级化合物库、抗体/多肽/蛋白治疗平台 | 超高通量 hit、剂量反应、早研候选物验证 | 成熟 assay 的大规模 reward factory | 早期靶点需共建 assay |
| **上海交通大学转化医学国家重大科技基础设施新药发现技术中心** | HTS、结构药理、类器官药效评价、AI 药物发现 | 药筛、类器官药效、临床前药理毒理 | 联通临床转化和瑞金等资源 | 跨系统合作流程较重 |
| **上海交通大学细胞工程与抗体药物教育部工程研究中心** | 抗体药物、细胞工程、中试/产业化、质控与制剂 | 抗体亲和力、表达量、稳定性、工艺/质控数据 | 抗体工程和 CMC 转化 | 偏工程化/产业化 |
| **上海抗体药物国家工程研究中心** | 新型抗体筛选、抗体工程、中试工艺、检测平台 | 抗体候选、亲和力/活性、工艺放大 readout | 抗体工程产业接口 | 商务/IP 条款关键 |
| **东南大学器官芯片和类器官研究中心** | 肿瘤、皮肤、心脏、血管、脑等器官芯片，高内涵成像 | 收缩频率/钙瞬变、毒性、药效、图像表型 | 器官芯片标准化和产业合作 | OoC 标准仍在形成 |
| **清华大学医学院刘鹏团队** | 微流控、高通量类器官培养/药筛、Grouped-seq | PDO 药敏、图像表型、转录组、单孔溯源数据 | 多模态 readout 密度高，适合 AI 训练 | 更像课题组技术，规模化需确认 |
| **复旦大学附属肿瘤医院/复旦类器官方向团队** | 肿瘤类器官、药敏、样本库、精准医疗 | PDO 建库率、药敏、病理/基因组一致性、临床响应 | 临床样本和真实世界转化 | 伦理、隐私、随访和授权成本高 |
| **四川大学华西医院精准药物/精准转化平台** | PDO/PDX、CRISPR、多组学、HTS、器官芯片 | 药敏、PDX 验证、多组学、靶点验证 | 大体量临床样本和转化医学链条 | 跨团队协调复杂 |
| **西湖大学/西湖实验室** | 冷冻电镜、质谱、流式、基因组、高通量、智能蛋白质组 | 结构、蛋白组、成像/流式、候选分子验证 | AI + 湿实验闭环原型 | 临床样本资源不如大型医院 |

参考来源：

- [国家蛋白质科学研究（上海）设施](https://sari.cas.cn/sylb/202507/t20250727_7897108.html)
- [清华蛋白质研究技术中心](https://phoenix.tsinghua.edu.cn/zxgk/zxjj.htm)
- [上海科技大学 iHuman](https://ihuman.shanghaitech.edu.cn/yjsjj/list.htm)
- [上海药物所化合物资源及筛选技术服务部](https://simm.cas.cn/web/ggjsfwzx/zxjj/hhw/)
- [中国医学科学院药物研究所国家药物筛选中心](https://www.imm.ac.cn/jgsz/yjjg/hcywhxyjs_d9ab6bf7809948a0ab49bbf3a650e8ae/index.htm)
- [深圳湾实验室转化医学中心报道](https://www.szbl.ac.cn/info/1015/3819.htm)
- [上海交大转化医学设施新药发现技术中心](https://transmed.sjtu.edu.cn/service0?cat=zx&id=1836996635922608129)
- [东南大学器官芯片和类器官研究中心](https://kjc.seu.edu.cn/jbyjy/31008/list.htm)
- [清华刘鹏团队](https://www.med.tsinghua.edu.cn/info/1144/2113.htm)、[Grouped-seq](https://www.tsinghua.edu.cn/info/1175/89965.htm)
- [华西精准药物研究室](https://www.wchscu.cn/public/notice/recruit/82216.html)
- [西湖大学冷冻电镜平台](https://brcf.westlake.edu.cn/ejpt/lddj1/ptgk.htm)

---

## 5. 建议的 Frontis 合作架构

### 5.1 不找单一全能供应商

Wet-lab reward network 应拆成多层：

```text
Layer 1: Sequence-to-material
  gene synthesis / expression / purification / QC

Layer 2: Binding and biophysics
  SPR / BLI / ITC / DSF / SEC / epitope binning

Layer 3: Functional assay
  cell potency / receptor activation / neutralization / immune killing

Layer 4: Phenotype and safety
  organoid / organ-chip / HCI / DMPK / toxicity

Layer 5: IND/GLP confirmation
  GLP tox / PK-PD / immunogenicity / regulatory package

Layer 6: Scientific Memory and training data
  raw data + negative data + metadata + SOP + decision trace
```

### 5.2 第一批 pilot 设计

#### Pilot A: Target-to-Binder wet validation

目标：验证 Frontis 能否把 AI 设计候选转为可训练的 protein reward。

建议配置：

- 设计输入：1 个靶点，50-300 条抗体或纳米抗体候选序列；
- 快速表达：百英生物或金斯瑞；
- 标准 target/QC：义翘神州、百普赛斯、近岸蛋白或 KACTUS；
- Binding：SPR/BLI，至少包含 KD、kon、koff、raw curve、阴性样本；
- Developability：表达量、纯度、SEC monomer、Tm、聚集、内毒素；
- 交叉验证：Top 10-20 条在第二家供应商复测；
- 可选功能：药明康德 Biology 或冠科补细胞功能 assay。

成功标准：

- 至少 90% 样本有完整 metadata；
- 失败样本有结构化原因；
- Top candidate 与 negative candidate 都可进入训练集；
- 两家供应商复测结果可校准到统一 reward schema；
- 能形成 `design -> experiment -> reward -> next design` 的闭环日志。

#### Pilot B: Phenotype / toxicity reward

目标：验证 Frontis 能否把类器官/器官芯片结果编译成 phenotype reward。

建议配置：

- 模型：肿瘤 PDO 或 DILI/心毒/肾毒器官芯片；
- 供应商：Xellar / 冠科 / 大橡 / 丹望 / K2 中选 2 家；
- Readout：IC50/AUC、HCI 图像、形态 embedding、细胞死亡、免疫浸润、毒理 biomarker、可选 RNA-seq；
- 对照：标准阳性药、阴性药、vehicle control、重复孔；
- 数据：原始图像、孔级 metadata、dose-response、QC flags、失败孔原因。

成功标准：

- 每个样本有孔级、批次级、模型级 metadata；
- 可把 HCI 图像和剂量曲线转成 reward vector；
- 可追踪 donor / model / passage / matrix / medium / SOP version；
- 能识别边缘孔效应、污染、建模失败等负数据；
- 能用于下一轮候选排序，而不是只做结论展示。

---

## 6. Reward Vector Schema 草案

### 6.1 蛋白 / 抗体 reward vector

| 字段 | 示例 |
|---|---|
| Sequence metadata | protein type、length、CDR、mutation、construct、tag、signal peptide |
| Expression | host、expression success、yield、solubility、culture scale、TAT |
| Purification/QC | purity、SEC monomer、aggregation、concentration、endotoxin、MS confirmation |
| Stability | Tm、DSF shift、freeze-thaw stability、storage stability |
| Binding | KD、kon、koff、Rmax、raw sensorgram、epitope bin、competition、cross-reactivity |
| Function | cell potency、EC50/IC50、neutralization、receptor activation/blocking、immune killing |
| Developability | pI、hydrophobicity、polyreactivity、viscosity、liability motifs、PTM risk |
| Failure labels | no expression、low yield、insoluble、degraded、aggregated、non-binding、assay interference |
| Provenance | supplier、SOP version、operator、instrument、reagent lot、batch id、replicate id |

### 6.2 类器官 / 器官芯片 reward vector

| 字段 | 示例 |
|---|---|
| Model metadata | cancer type / organ type、donor、passage、matrix、medium、chip type、co-culture cells |
| Treatment | compound/protein id、dose、schedule、exposure time、vehicle、control |
| Viability | CTG、cell count、live/dead、IC50、AUC、max inhibition |
| Imaging | raw HCI image、segmentation mask、morphology embedding、organoid size/roundness/texture |
| Toxicity | DILI biomarker、cardiac contraction、Ca2+ transient、TEER、kidney injury marker、cytokines |
| Mechanism | RNA-seq、proteomics、phospho-signaling、IHC/IF/mIF、flow cytometry |
| QC/failure | model establishment failure、contamination、edge effect、low viability、batch drift |
| Provenance | donor consent class、IRB id、sample chain、SOP version、reagent lot、instrument config |

---

## 7. 尽调问题清单

### 7.1 数据交付

1. 能否交付原始数据、处理后数据、QC、失败原因、批次/试剂/仪器/SOP 版本，而不是只交 PDF？
2. 是否默认保留失败样本并结构化标注？
3. 是否支持 SFTP/API/LIMS/ELN 批量导出？
4. 是否有数据字典、审计日志、条码追踪和孔级 metadata？
5. 原始图像、SPR/BLI 曲线、flow cytometry FCS、RNA-seq FASTQ/count matrix 是否可交付？

### 7.2 实验设计

1. 是否支持盲测 pilot？
2. 是否支持阳性/阴性对照、重复孔、跨批复测和固定重跑规则？
3. 模型间 CV、批间 CV、操作员差异如何记录？
4. Assay 干扰、边缘孔效应、污染、低活性、低表达是否结构化标记？
5. 是否可以共同设计 reward vector，而不是用供应商默认报告模板？

### 7.3 合规和 IP

1. 人源样本的 IRB、知情同意、人遗合规、PIPL、数据出境和二次研究授权是否覆盖 AI 训练？
2. Frontis 是否拥有内部模型训练权、负数据使用权、衍生 embedding 和 reward model 的权利？
3. 供应商是否会横向使用 Frontis 的序列、候选物、实验数据或训练样本？
4. 是否有靶点排他、用途限制、药物资产权属或里程碑条款？
5. 是否支持 Agent 介入边界：Agent 生成实验建议，人类审批 SOP，湿实验过程全程记录。

---

## 8. 合作优先级

### 8.1 第一批试单

建议先做两个 6-8 周 pilot：

| Pilot | 首选伙伴 | 目标 |
|---|---|---|
| Antibody/Nanobody validation | 百英生物 + 金斯瑞 + 义翘/百普赛斯/KACTUS | 验证 AI 设计候选能否形成表达、binding、developability reward |
| Organoid/OoC phenotype reward | 冠科 + Xellar / 大橡 / 丹望 | 验证 HCI 图像、药敏、毒理、组学能否进入 reward ledger |

### 8.2 第二批拓展

| 方向 | 候选 |
|---|---|
| 难靶点结构和机制 | 国家蛋白质设施、iHuman、维亚生物、西湖大学 |
| 体内抗体/纳米抗体平台 | 百奥赛图 |
| GLP/IND 补强 | 美迪西、昭衍、康龙、药明康德 Biology |
| 临床样本和 PDO | 复旦肿瘤、华西、K2、丹望、粤港澳大湾区精准医学研究院 |
| 酶设计/工业蛋白 | 恩和生物、弈柯莱、天津工生所 |

### 8.3 最推荐先聊的 10 个对象

1. **百英生物 Biointron**：抗体/纳米抗体变体快速表达和 developability。
2. **金斯瑞 GenScript**：低摩擦、标准化、规模化 gene-to-protein 循环。
3. **百普赛斯 ACROBiosystems**：高质量 reagent、SPR/BLI、Fc/FcR/C1q/QC。
4. **KACTUS 恺佧生物**：困难膜蛋白、MHC/TCR、VLP/nanodisc target。
5. **百奥赛图 Biocytogen**：RenMab/RenNano 和体内抗体数据资产。
6. **冠科生物 Crown Bioscience**：肿瘤 PDO/PDXO/PDX benchmark 和 biologics 功能验证。
7. **耀速科技 Xellar**：高通量器官芯片、高内涵图像和毒理表型。
8. **大橡科技 Daxiang Bio**：国产类器官芯片、DMPK/毒理/药敏。
9. **丹望医疗 D1Med**：PDO 样本库、类器官芯片、免疫共培养。
10. **东南大学器官芯片和类器官研究中心 / 国家蛋白质设施**：方法学共建和高可信 readout。

---

## 9. 与前一份产业图谱的关系

前一份报告 `china_protein_design_and_organ_chip_landscape_2026-06-28.md` 关注的是“哪些公司在蛋白质设计或器官芯片赛道做得好”。本报告关注的是另一件事：

> 谁能稳定、可审计、可复现地为 Frontis 产出实验数据和 reward。

因此，很多 AI 能力强的公司在本报告中不是第一优先；很多传统 CRO、reagent 公司、高校医院平台反而更重要。对 Frontis 来说，它们的价值不是讲 AI，而是把真实湿实验世界变成可训练、可记录、可迭代的 Scientific Memory。

