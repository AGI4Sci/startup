# Frontis AI4Sci 目标用户清单与市场规模调研报告

**调研日期**：2026-06-28  
**主题**：Frontis AI4Sci / Target-to-Binder Sprint / Candidate Decision Package 的目标用户、科研机构生态与市场规模  
**用途**：补充 `site/index.html` 中“目标用户”“资源请求”“市场机会”相关判断

---

## 0. Executive Summary

Frontis AI4Sci 的第一批目标用户不应定义为泛科研人群，也不应从大药企总部级平台采购切入。更准确的 ICP 是：

> **已有明确 target / disease hypothesis / biologics candidate，需要在 8-12 周内完成 continue / kill / BD / next experiment 决策，但缺完整 AI + expert review + wet validation 闭环的 discovery team。**

第一阶段应卖项目结果，而不是抽象平台：

```text
Target-to-Binder Sprint
  + Confidential Project Room
  + Candidate Decision Package
  + Expert Review
  + Wet Validation / Reward Coordination
```

核心结论：

1. **第一批直接客户**：ADC / 双抗 / TCE / biologics 项目型 biotech，尤其是有 BD、融资、IND 前或下一轮实验时间窗口的团队。
2. **大药企和头部 biotech**：适合 lighthouse pilot，不适合作为最早期收入主线。
3. **科研机构、医院、国家平台**：不应作为泛科研助手客户；主要角色是 clinical context、疾病机制、样本、结构生物学、类器官 / 器官芯片 reward、科学背书和 PI 孵化项目来源。
4. **CRO、器官芯片、类器官、模型动物和 wet-lab 平台**：优先作为 reward source、执行伙伴和渠道伙伴，不要混入第一批直接客户。
5. **市场规模**：Frontis 当前可切入的是全球约 **$1-3B** 的 AI-native discovery execution market，中国约 **$0.1-0.4B**；到 2031 年全球可达 **$5-14B**，中国 **$0.8-2.5B**；到 2036 年全球可达 **$14-40B**，中国 **$2.5-7.5B**。

---

## 1. ICP 定义

### 1.1 不要用人数定义用户

HTML 里当前表述是：

> 20-200 人 biotech / discovery group，有 target 和 wet-loop 需求，但缺完整 AI platform team。

这个方向正确，但人数不是最关键的判断标准。更好的定义方式是按 **项目状态 + 购买事件 + 闭环能力缺口**。

推荐 ICP：

> 第一批客户是有明确 target / disease hypothesis / biologics candidate、需要在 8-12 周内完成 continue / kill / BD / next experiment 决策的早中期 discovery team。典型规模 20-200 人，已有 wet-lab 或 CRO 合作，但缺完整 AI platform、专家 review 和可训练 wet reward 闭环。

### 1.2 购买触发事件

最强购买事件不是“想用 AI”，而是项目窗口逼近：

1. 融资前需要可信 research dossier。
2. BD / out-license 前需要差异化证据包。
3. Target 立项前需要快速 kill / continue。
4. Candidate 进入下一轮实验前需要排序和 developability 风险判断。
5. IND-enabling 前需要补强候选物证据链。
6. 内部 AI / wet-lab / 专家资源不足，但项目窗口只有 8-12 周。

### 1.3 谁买、谁用、谁影响

| 角色 | 典型头衔 | 关心什么 |
|---|---|---|
| 经济买方 | CEO、CSO、VP Discovery、BD Head、Program Lead | 项目进度、证据质量、融资/BD 叙事、是否继续投入 |
| 日常使用者 | Protein engineer、computational biologist、assay lead、translational scientist | 候选排序、实验计划、证据追踪、复盘效率 |
| 影响者 | 外部 domain expert、结构专家、assay 专家、转化医学专家 | 科学判断、反驳、rubric、kill criteria |
| 数据 / 合规把关 | IT、法务、数据治理、IP 负责人 | 数据不出域、no-training-by-default、权限审计、IP 边界 |

---

## 2. 中国直接客户清单

### 2.1 A 档：第一批优先约谈

这些公司最接近第一批直接付费客户：有 biologics / ADC / 双抗 / TCE / 细胞治疗项目压力，同时销售链条相对大药企更短。

| 公司 | 为什么适合 | 可能买方 / 切入项目 | 难度 | 来源 |
|---|---|---|---|---|
| 映恩生物 DualityBio | ADC 管线密集，BD 叙事强 | CSO / BD；ADC target / candidate 排序 | 中 | [官网](https://www.dualitybiologics.com/) |
| 礼新医药 LaNova | ADC / 双抗资产，适合 BD 前证据包 | BD / 研发负责人；候选物差异化 | 中 | [官网](https://www.lanovamedicines.com/) |
| 宜联生物 MediLink | ADC 平台型 biotech，项目决策频繁 | 研发 / BD；linker-payload / 靶点优先级 | 中 | [官网](https://www.medilinkthera.com/) |
| 迈威生物 Mabwell | 抗体 / ADC / 融合蛋白，多项目管线 | 早研 / 转化；candidate package | 中 | [官网](https://www.mabwell.com/) |
| 乐普生物 Lepu Biopharma | ADC / IO 管线，上市公司有 BD 压力 | 研发 / BD；适应症与组合证据 | 中 | [官网](https://www.lepubiopharma.com/) |
| 天演药业 Adagene | 抗体工程 / 条件激活抗体，AI 叙事兼容 | CSO / BD；抗体工程优化 | 中 | [官网](https://www.adagene.com/) |
| 岸迈生物 EpimAb | 双抗平台公司，正中 target-to-binder | 创始人 / CSO；双抗组合设计 | 中 | [官网](https://www.epimab.com/) |
| 和铂医药 Harbour BioMed | 抗体平台 + 自研管线 | 平台 / 研发；新靶点立项 | 中 | [官网](https://www.harbourbiomed.com/) |
| 康诺亚 Keymed | 自免 / 肿瘤抗体管线，转化需求强 | 研发 / BD；适应症扩展证据 | 中 | [官网](https://www.keymedbio.com/) |
| 宜明昂科 ImmuneOnco | CD47 / IO 抗体与组合治疗 | CSO / 临床前；kill / continue | 中 | [官网](https://www.immuneonco.com/) |
| 礼进生物 Elpiscience | 肿瘤免疫抗体管线 | 创始人 / CSO；靶点与组合策略 | 中 | [官网](https://www.elpiscience.com/) |
| 康宁杰瑞 Alphamab | 双抗 / 多抗工程能力强 | 研发 / BD；双抗候选物排序 | 中高 | [官网](https://www.alphamabonc.com/) |
| OnCusp Therapeutics | 中美双站点、肿瘤创新资产 | CEO / BD；BD 前 decision package | 中 | [官网](https://www.oncusptx.com/) |
| Eucure / 百奥赛图创新管线 | 抗体发现资源强，但需区分平台服务与自研 | 自研管线负责人；抗体候选物 | 中 | [Eucure](https://www.eucure.com/)、[Biocytogen](https://www.biocytogen.com/) |
| 驯鹿生物 IASO Bio | 细胞治疗，BCMA 等方向 | 新靶点 / 下一代 construct | 中 | [官网](https://www.iasobio.com/) |
| 原启生物 OriCell | 细胞治疗 / 实体瘤方向 | 抗原选择与组合证据 | 中 | [官网](https://www.oricell.com/) |

第一批最建议约谈的 10-15 个：

> DualityBio、LaNova、MediLink、Mabwell、Lepu Biopharma、Adagene、EpimAb、Harbour BioMed、Keymed、ImmuneOnco、Elpiscience、Alphamab、OnCusp、IASO Bio、OriCell。

理由：这些团队都有明确 biologics / ADC / 双抗 / 细胞治疗项目压力，既需要科学证据，也需要 BD 或下一轮实验决策；相比大药企，销售链条短一些；相比 CRO / 实验平台，它们更像真正的直接付费客户。

### 2.2 B 档：项目化切入，销售更重

| 公司 | 为什么适合 | 可能切入 | 难度 | 来源 |
|---|---|---|---|---|
| 百利天恒 / SystImmune | ADC / 双抗资产强，BD 价值高 | 单项目 BD 证据包 | 高 | [SystImmune](https://www.systimmune.com/) |
| 科伦博泰 Kelun-Biotech | ADC 管线和海外交易活跃 | ADC 立项 / BD package | 高 | [官网](https://www.kelun-biotech.com/) |
| 荣昌生物 RemeGen | ADC + 抗体商业化经验 | 下一代 ADC / 适应症扩展 | 高 | [官网](https://www.remegen.com/) |
| 复宏汉霖 Henlius | 抗体 / 双抗 / ADC 管线 | 早研项目 room | 高 | [官网](https://www.henlius.com/) |
| 天境生物 I-Mab | 免疫抗体资产，BD 导向明显 | 海外 BD 前证据整理 | 中高 | [官网](https://www.i-mabbiopharma.com/) |
| 基石药业 CStone | 肿瘤管线，偏 BD / 组合策略 | in / out-license 科学评估 | 中高 | [官网](https://www.cstonepharma.com/) |
| 神州细胞 Sinocelltech | 生物药平台和抗体管线 | 新靶点 / 候选物评估 | 中高 | [官网](https://www.sinocelltech.com/) |
| 创胜集团 Transcenta | 抗体 / 肿瘤管线，状态需复核 | 存量资产再评估 | 中高 | [官网](https://www.transcenta.com/) |
| 药明巨诺 JW Therapeutics | 细胞治疗，适合抗原 / 构建设计 | CAR target / construct decision | 中高 | [官网](https://www.jwtherapeutics.com/) |
| 普瑞金 Pregene | 细胞治疗平台型公司 | 靶点 / construct 优先级 | 中 | [官网](https://www.pregene.com/) |

### 2.3 C 档：lighthouse 客户

这些客户价值高，但采购周期长、内部平台强、合规门槛高。建议作为 lighthouse pilot，而不是第一批收入主线。

| 公司 | 价值 | 问题 | 来源 |
|---|---|---|---|
| 信达生物 Innovent | 中国创新药标杆，抗体 / ADC / IO 管线 | 采购周期长，内部能力强 | [官网](https://www.innoventbio.com/) |
| 康方生物 Akeso | 双抗标杆，科学背书强 | 更适合单项目 lighthouse | [官网](https://www.akesobio.com/) |
| 百济神州 BeiGene | 全球化研发体系，背书极强 | 销售复杂，平台门槛高 | [官网](https://www.beigene.com/) |
| 恒瑞医药 Hengrui | ADC / 抗体 / 小分子全覆盖 | 大药企流程长 | [官网](https://www.hrs.com.cn/) |
| 石药集团 CSPC | 创新药和 ADC 布局 | 集团采购复杂 | [官网](https://www.cspc.com.hk/) |
| 君实生物 Junshi | IO 抗体经验深 | 早研预算与优先级需验证 | [官网](https://www.junshipharma.com/) |
| 再鼎医药 Zai Lab | BD / 引进能力强 | 更像 BD decision customer，不是 target-to-binder 主线 | [官网](https://www.zailaboratory.com/) |
| 传奇生物 Legend Biotech | 细胞治疗标杆 | 全球化大客户，销售长 | [官网](https://www.legendbiotech.com/) |

---

## 3. 科研机构、医院与国家平台

### 3.1 基本判断

科研机构要纳入，但不能作为泛科研工具客户。它们更适合作为：

1. 疾病机制和 target source；
2. 临床样本和 patient-derived model source；
3. 类器官 / 器官芯片 / 表型 readout source；
4. 蛋白制备、结构生物学、组学和方法学平台；
5. 科学背书和共同论文来源；
6. PI 孵化项目 / NewCo 前项目入口。

只有当科研项目具备融资、BD、立项或临床转化时间窗口时，才适合作为项目制付费客户。

### 3.2 中国优先清单

| 层级 | 机构 / 平台 | 适合角色 | 付费判断 | 来源 |
|---|---|---|---|---|
| A | 转化医学国家重大科技基础设施上海 / 瑞金-交大 | 临床样本、生物标志物、新药验证 | 共研 + 少数付费 | [来源](https://transmed.sjtu.edu.cn/about3) |
| A | 中科院上海药物所 SIMM | 靶点、筛选、药理、转化 | 潜在付费 / 共研 | [来源](https://simm.cas.cn/) |
| A | 上海科技大学免疫化学研究所 SIAIS | 抗体、ADC、蛋白药物 | 潜在付费 / 共研 / NewCo | [来源](https://siais.shanghaitech.edu.cn/1843/list.htm) |
| A | 国家蛋白质科学设施上海 NFPS | 蛋白制备、结构、组学 | Reward source | [来源](https://lssf.cas.cn/en/facilities/biology/nfps/) |
| A | 北京协和转化医学国家设施 | 罕见病、老龄化、临床验证 | 共研 / reward | [来源](https://www.pumch.cn/linsyansuo_zhuanhuajichusheshi.html) |
| A | 北京生命科学研究所 / 清华生医交叉 | 原创靶点、PI 孵化 NewCo | NewCo 源 / 共研 | [来源](https://www.timbr.tsinghua.edu.cn/yjyjs1/gkjs.htm) |
| A | 清华北京生物结构前沿研究中心 | 结构生物学、AI 结构药物 | Methodology / reward | [来源](https://www.frcbs.tsinghua.edu.cn/) |
| A | 北京大学未来技术学院 / 分子医学 | 疾病机制、类器官、RNA / GPCR | 共研 / 项目付费 | [来源](https://future.pku.edu.cn/xygkn/xszx/index.htm) |
| A | 深圳湾实验室 / 深圳医学科学院 | IT + BT、重大疾病、创新药 | 战略共研 | [来源](https://www.szbl.ac.cn/about-us.htm) |
| A | 西湖大学 WeCIP / 蛋白组中心 | 蛋白组基础模型、靶点发现 | 共研 / 项目付费 | [来源](https://sls.westlake.edu.cn/Research/CoreLab/WestlakeIntelligentBiomarkerDiscoveryLab/) |
| A | 四川大学华西医院生物治疗平台 | 肿瘤免疫、细胞 / 蛋白治疗 | 付费 / 共研 / 临床 reward | [来源](https://www.wchscu.cn/details/51626.html) |
| A | 中山大学肿瘤防治中心 SYSUCC | 肿瘤样本、临床试验、转化 | 共研 / reward / 项目付费 | [来源](https://research.sysu.edu.cn/platform/gjj) |
| B | 复旦大学附属肿瘤医院 | 肿瘤类器官、样本、精准治疗 | 共研 / reward | [来源](https://www.shca.org.cn/) |
| B | 中国医学科学院肿瘤医院 / 国家癌症中心 | 国家级肿瘤临床转化 | 背书 / reward | [来源](https://www.cams.ac.cn/rcjs/szdw/zpcpjs/js/js_zlyy/6445f3339d8a470f890339c709a8365b.htm) |
| B | 浙江大学转化医学研究院 / 良渚实验室 | 转化医学、再生、精准诊治 | 共研 / 项目付费 | [来源](https://itm.zju.edu.cn/) |
| B | 中科院广州生物医药与健康研究院 | 干细胞、感染免疫、化学生物学 | 共研 / NewCo 源 | [来源](https://gibh.cas.cn/) |
| B | 中科院深圳先进院 / 合成生物学所 | 合成生物学、自动化平台 | Methodology / reward | [来源](https://isynbio.siat.ac.cn/) |
| B | 中科院生物物理所 | 蛋白结构、感染免疫、核酸 | Reward / methodology | [来源](https://www.ibp.cas.cn/) |
| B | 国家蛋白质科学中心北京 | 蛋白组、结构设施 | Reward source | [来源](https://www.ncpsb.org.cn/genee/) |
| B | 复旦中山医院 | 肝癌、心血管、临床研究 | Clinical reward | [来源](https://gs-shmc.fudan.edu.cn/zsyy/list.htm) |
| B | 中科院上海营养与健康所 | 衰老、代谢、慢病、生物数据 | 机制 / 靶点共研 | [来源](https://sinh.cas.cn/) |
| B | 中山大学附属一院转化医学中心 | 临床转化、样本、疾病机制 | 共研 / reward | [来源](https://www.fahsysu.org.cn/node/552) |
| B | 华中科技大学协和医院转化医学中心 | 临床-药物转化 | Clinical reward | [来源](https://www.whuh.com/info/1446/8268.htm) |
| B | 华中科技大学同济医院 | 科创转化、细胞治疗 | NewCo / 临床共研 | [来源](https://www.tjh.com.cn/contents/1537/55229.html) |
| B | 同济大学东方医院 / 再生医学 | 干细胞、再生医学 | Methodology / reward | [来源](https://life.tongji.edu.cn/03/30/c12684a131888/page.htm) |
| B | 南方科技大学冷冻电镜中心 | 结构解析、蛋白验证 | Reward source | [来源](https://cryoem.sustech.edu.cn/about/about.html) |
| C | 广医一院 / 呼吸疾病全国重点实验室 | 呼吸疾病、肺癌、感染 | Clinical reward | [来源](https://www.sklrd.cn/show_list.php?id=1) |
| C | 上海市肺科医院 | 肺癌、结核、肺部疑难病 | Clinical / sample source | [来源](https://www.shsfkyy.com/) |
| C | 武汉大学人民医院肿瘤中心 | 肿瘤免疫、精准治疗 | Clinical reward | [来源](https://www.rmhospital.com/dept/zl) |
| C | 厦门大学细胞应激生物学实验室 | 肿瘤 / 炎症机制 | 机制共研 | [来源](https://sklcsb.xmu.edu.cn/) |
| C | 中科院上海有机所 SIOC | 化学生物学、linker / PROTAC | Methodology partner | [来源](https://www.sioc.ac.cn/) |
| C | 中科院分子细胞卓越中心 | 免疫、发育、细胞机制 | PI / 机制源 | [来源](https://cemcs.cas.cn/) |

### 3.3 角色归类

潜在付费优先看：

- 上海药物所；
- SIAIS；
- 西湖 WeCIP；
- 北大 / 清华部分产业合作项目；
- 华西 / 中山肿瘤 / 复旦肿瘤的具体病种项目；
- 北生所孵化 NewCo。

主要共研 / 背书看：

- 瑞金-交大转化设施；
- 北京协和；
- 深圳湾实验室；
- 浙大 / 良渚；
- 中科院广州生物医药与健康研究院；
- 中国医学科学院肿瘤医院 / 国家癌症中心。

主要 reward source 看：

- 国家蛋白质科学设施上海；
- 国家蛋白质科学中心北京；
- 中科院生物物理所；
- 清华 FRCBS；
- 南科大冷冻电镜；
- 医院样本、类器官和临床 readout 平台。

### 3.4 建议写入 HTML 的表述

> 科研机构不是我们的泛科研助手客户。我们优先绑定有明确转化项目、疾病机制、样本 / 类器官 / 器官芯片 / 蛋白结构 / 抗体平台和 NewCo / BD 可能性的医院转化中心、国家平台和 PI 孵化项目。它们主要提供 clinical context、wet reward、科学背书和高质量项目源；只有当项目具备融资、BD、立项或临床转化时间窗口时，才作为项目制付费客户切入。

---

## 4. 海外参照

### 4.1 A 类：中小 biologics / antibody / protein biotech

这些公司最像海外可比直接客户。共同特征是：围绕 antibody、ADC、TCE、multispecific、protein engineering 或新型 scaffold 做项目推进，需要外部 expert + wet-loop decision package。

| 公司 | 为什么相关 | 切入点 | 来源 |
|---|---|---|---|
| Zymeworks | Multispecific / oncology pipeline | 新 target / backup candidate package | [Pipeline](https://www.zymeworks.com/pipeline/) |
| Xencor | XmAb Fc、多特异抗体工程 | Developability + differentiation | [Pipeline](https://xencor.com/pipeline/) |
| Sutro Biopharma | ADC、cell-free protein engineering | ADC candidate optimization | [官网](https://www.sutrobio.com/) |
| MacroGenics | DART / TRIDENT bispecific | TCE / bispecific 风险评估 | [Platforms](https://macrogenics.com/platforms/dart-and-trident-platforms/) |
| Janux Therapeutics | Tumor-activated TCE | 安全窗、target 选择 | [Pipeline](https://www.januxrx.com/development-pipeline/) |
| CytomX | Masked biologics、ADC、TCE | Masked modality 外部验证 | [Technology](https://cytomx.com/probody-therapeutics/) |
| Werewolf Therapeutics | Conditionally activated proteins / TCE | Cytokine / TCE 机制验证 | [Pipeline](https://werewolftx.com/our-pipeline/) |
| Bicara Therapeutics | Bifunctional EGFR / TGF-beta antibody | Solid tumor translational package | [官网](https://www.bicara.com/) |
| Cullinan Therapeutics | T cell engager in oncology / autoimmune | TCE indication expansion | [Pipeline](https://cullinantherapeutics.com/science/pipeline/) |
| Numab Therapeutics | Multispecific antibody | Format / biology review | [官网](https://www.numab.com/) |
| Molecular Partners | DARPin / Radio-DARPin | Non-Ig scaffold 评估 | [官网](https://www.molecularpartners.com/) |
| Affimed | Innate cell engagers | Combination / response biology | [官网](https://www.affimed.com/) |
| Innate Pharma | NK / innate immunotherapy | Biomarker + target package | [官网](https://www.innate-pharma.com/) |
| Orum Therapeutics | Degrader-antibody conjugate | DAC target / payload package | [Platforms](https://www.orumrx.com/platforms) |
| Pyxis Oncology | ADC / mAb clinical portfolio | ADC differentiation package | [官网](https://pyxisoncology.com/) |

### 4.2 B 类：大药企 lighthouse

大药企不是第一收入主线，而是 credibility 和 lighthouse。适合通过单个 discovery program、China / Asia asset review、ADC / biologics validation 进入。

| 公司 | 角色 | 切入点 | 来源 |
|---|---|---|---|
| Roche / Genentech | Biologics 与外部创新强 | China / Asia asset review、antibody optimization lighthouse | [Partnering](https://www.roche.com/stories/beyond-the-deal-in-partnering) |
| Novartis | AI / protein therapeutic 合作活跃 | 多 target pilot | [Generate 合作](https://generatebiomedicines.com/media-center/generatebiomedicines-announces-multi-target-collaboration-with-novartis) |
| AstraZeneca | ADC、AI biologics、open innovation | Biologics discovery / ADC validation | [Open Innovation](https://openinnovation.astrazeneca.com/) |
| Pfizer / Seagen | ADC 大玩家 | Next-gen ADC evidence package | [Pfizer](https://www.pfizer.com/) |
| Merck & Co. | Oncology / external innovation | Target / asset diligence | [BD&L](https://www.merck.com/research/business-development-and-licensing/) |
| Eli Lilly | AI antibody 合作活跃 | Bispecific / AI biologics pilot | [XtalPi-Ailux 合作](https://en.xtalpi.com/xtalpi-subsidiary-ailux-seals-345m-ai-powered-bispecific-antibody-partnership-with-eli-lilly/) |
| J&J | ADC / oncology M&A | ADC target / candidate review | [官网](https://www.jnj.com/) |
| AbbVie | ADC / ImmunoGen 后续管线 | ADC / oncology biologics validation | [官网](https://www.abbvie.com/) |
| Gilead | ADC external innovation | ADC / TCE 项目评估 | [官网](https://www.gilead.com/) |
| BMS / Takeda / Sanofi | Immunology、oncology biologics | TCE / antibody / protein design pilot | [BMS](https://www.bms.com/)、[Takeda](https://www.takeda.com/)、[Sanofi](https://www.sanofi.com/) |

### 4.3 C 类：AI-native / TechBio 标杆或合作方

这类大多不是客户，而是竞品、合作方或估值参照物。Frontis 如果切入，最好卖“human disease biology + China wet validation + expert decision package”，而不是和它们正面拼模型。

| 公司 | 判断 | 来源 |
|---|---|---|
| Generate:Biomedicines | 强竞品 / 标杆，可比交易对象 | [官网](https://generatebiomedicines.com/) |
| Absci | AI + wet biologics flywheel，直接竞品 | [Technology](https://www.absci.com/technology/) |
| BigHat Biosciences | AI antibody + wet lab，直接竞品 / 合作方 | [Technology](https://www.bighatbio.com/technology) |
| Xaira Therapeutics | AI drug discovery 超级标杆 | [官网](https://www.xaira.com/) |
| Nabla Bio | AI protein / biologics design 竞品 | [融资与合作新闻](https://www.businesswire.com/news/home/20240514763517/en/Nabla-Bio-Secures-%2426M-Series-A-Financing-and-Collaborations-with-AstraZeneca-Bristol-Myers-Squibb-and-Takeda-for-Generative-Protein-Design) |
| AbCellera | Antibody discovery 平台标杆 / 潜在合作 | [Lilly 合作](https://investors.abcellera.com/news/news-releases/2020/AbCellera-Announces-Multi-Year-Antibody-Discovery-Collaboration-with-Lilly/default.aspx) |
| Isomorphic Labs | AI drug discovery 标杆 | [Lilly / Novartis 合作](https://www.isomorphiclabs.com/articles/isomorphic-labs-kicks-off-2024-with-two-pharmaceutical-collaborations) |
| Recursion / Exscientia | AI discovery 平台标杆 | [Recursion](https://www.recursion.com/) |
| Cradle Bio | Protein engineering 工具 / 合作方 | [官网](https://www.cradle.bio/) |
| LabGenius | ML antibody discovery 竞品 | [官网](https://labgeniustx.com/) |
| Adaptyv Bio | Wet-loop / protein validation 合作方 | [官网](https://www.adaptyvbio.com/) |
| Dyno Therapeutics / Profluent | Protein / sequence design 合作方 | [Dyno](https://www.dynotx.com/)、[Profluent](https://www.profluent.bio/) |

---

## 5. 市场规模模型

### 5.1 建议使用的市场口径

不要直接引用整个 AI drug discovery 市场作为 Frontis 的市场规模。AI drug discovery 报告通常混合：

- target identification；
- small molecule generation；
- clinical trial design；
- repurposing；
- data analytics；
- imaging；
- enterprise software；
- service revenue。

Frontis 第一阶段切的是更窄但更高价值的交叉市场：

```text
AI discovery
  x biologics / antibody / protein discovery
  x preclinical / discovery outsourcing
  x expert review
  x wet reward network
  x project room / scientific memory / reward ledger
```

推荐命名：

> **AI-native early discovery execution market**

或：

> **AI-native discovery decision and validation market**

### 5.2 TAM / SAM / SOM 工作版

以下为工作版估算，不是审计级精算。核心假设见 5.4。

| 市场 | 2026 TAM | 2031 TAM | 2036 TAM | 2026 SAM | 2031 SAM | 2036 SAM | 2026 SOM | 2031 SOM | 2036 SOM |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 全球 | $1.1-3.3B | $5-14B | $14-40B | $0.25-0.9B | $1.7-5B | $5-14B | $1-5M | $40-150M | $250-900M |
| 中国 | $0.10-0.40B | $0.8-2.5B | $2.5-7.5B | $0.03-0.14B | $0.25-0.9B | $0.8-2.8B | $0.2-1.5M | $8-35M | $50-180M |

### 5.3 TAM 拆分

| 全球 TAM | 2026 | 2031 | 2036 |
|---|---:|---:|---:|
| Direct service: Target-to-Binder / Candidate Package | $0.8-2.4B | $3.7-10B | $10-28B |
| Platform software: Project Room / Memory / Workflow | $0.15-0.5B | $0.8-2.5B | $2.5-7B |
| Reward network coordination / validation layer | $0.1-0.4B | $0.5-1.8B | $1.5-5B |

| 中国 TAM | 2026 | 2031 | 2036 |
|---|---:|---:|---:|
| Direct service | $70-280M | $550M-1.7B | $1.8-5.2B |
| Platform software | $15-70M | $150-550M | $450M-1.6B |
| Reward network | $10-50M | $80-250M | $250-750M |

人民币口径：

| 中国市场 | 2026 | 2031 | 2036 |
|---|---:|---:|---:|
| 项目制 direct service 收入池 | 3-10 亿元 | 12-35 亿元 | 40-120 亿元 |
| 科研机构 / 医院 / 国家平台可捕获收入池 | 0.5-2 亿元 | 2-8 亿元 | 5-20 亿元 |

### 5.4 关键假设

| 假设 | 2026 | 2031 | 2036 |
|---|---:|---:|---:|
| 全球可服务 discovery org / project team | 1,500-2,500 | 4,000-6,000 | 7,000-10,000 |
| 中国可服务 discovery org / project team | 250-450 | 800-1,200 | 1,500-2,200 |
| 年项目数 / 客户 | 1-2 | 2-4 | 3-6 |
| Direct service ASP，全球 | $250k-750k | $350k-1M | $500k-1.5M |
| Direct service ASP，中国 | 全球 50-70% | 全球 50-70% | 全球 50-70% |
| Platform ARR / account | $50k-150k | $120k-400k | $250k-1M |
| Reward network take-rate | 10-25% | 10-25% | 10-25% |

### 5.5 市场报告锚点

这些公开报告口径不完全一致，只适合做交叉校验：

- [Grand View Research: AI in Drug Discovery](https://www.grandviewresearch.com/industry-analysis/artificial-intelligence-drug-discovery-market)：2026E 约 $2.9B，2033E 约 $13.8B。
- [Mordor Intelligence: AI in Drug Discovery](https://www.mordorintelligence.com/industry-reports/artificial-intelligence-in-drug-discovery-market)：2026E 约 $3.25B，2031E 约 $10.29B。
- [MarketsandMarkets: AI in Life Sciences](https://www.marketsandmarkets.com/Market-Reports/ai-in-life-science-market-45756262.html)：2026E 约 $21.58B，2031E 约 $69.34B；定义明显更宽。
- [Grand View Research: Drug Discovery Outsourcing](https://www.grandviewresearch.com/industry-analysis/drug-discovery-outsourcing-market)：2026E 约 $8.8B，2033E 约 $17.1B。
- [MarketsandMarkets: Antibody Discovery Services](https://www.marketsandmarkets.com/Market-Reports/antibody-discovery-market-182887795.html)：2025E 约 $1.90B，2030E 约 $3.54B。
- [Mordor Intelligence: Antibody Discovery](https://www.mordorintelligence.com/industry-reports/antibody-discovery-market)：2025E 约 $9.09B，2030E 约 $15.45B；口径比 antibody discovery services 更宽。
- [Grand View Research: Organoids & Spheroids](https://www.grandviewresearch.com/industry-analysis/organoids-spheroids-market)：2024 年约 $1.86B，2030E 约 $6.27B。
- [Grand View Research: Organ-on-a-Chip](https://www.grandviewresearch.com/industry-analysis/organ-on-a-chip-market-report)：2024 年约 $157M，2030E 约 $952M。
- [Grand View Research: China AI Drug Discovery](https://www.grandviewresearch.com/horizon/outlook/artificial-intelligence-in-drug-discovery-market/china)：2025 年约 $133.6M，2033E 约 $917.1M。
- [Grand View Research: China Preclinical CRO](https://www.grandviewresearch.com/horizon/outlook/preclinical-cro-market/china)：2025 年约 $346.2M，2033E 约 $759.2M。

### 5.6 投资人材料建议口径

> Frontis 当前可切入的是全球约 **$1-3B** 的 AI-native discovery execution market，中国约 **$0.1-0.4B**。到 2031 年，随着 AI discovery、抗体 / 新模态和 wet validation network 成熟，全球 TAM 可达 **$5-14B**，中国 **$0.8-2.5B**。到 2036 年，若 Science Agent OS 成为 discovery team 的工作层，全球 TAM 可扩到 **$14-40B**，中国 **$2.5-7.5B**。

---

## 6. 销售与产品建议

### 6.1 第一单怎么卖

不要卖：

- “AI 科研平台”；
- “通用科研助手”；
- “大模型 for science”；
- “企业级 Science Agent OS 订阅”。

建议卖：

> **8-12 周 Target-to-Binder / Candidate Decision Sprint：用 AI + 专家网络 + wet validation / reward，在一个 target 或候选物上形成可立项、可停项、可 BD、可进入下一轮实验的证据包。**

### 6.2 第一批客户筛选标准

| 标准 | 理想状态 |
|---|---|
| Target / candidate | 已有明确 target、disease hypothesis 或 biologics candidate |
| 时间窗口 | 8-12 周内有立项、停项、BD、融资或下一轮实验决策 |
| 数据 | 愿意提供必要的非敏感项目约束，或可先从 public / low-sensitive sprint 开始 |
| Wet-loop | 有内部实验能力或稳定 CRO / wet-lab partner |
| 买方 | CEO / CSO / VP Discovery / BD Head 有直接项目压力 |
| 数据边界 | 接受 no-training-by-default、项目级隔离、审计和可选 opt-in |
| 成功标准 | 能明确 continue / kill / next experiment / BD narrative |

### 6.3 中国市场独特卖点

对中国客户，最强表述不是“我们有 AGI”，而是：

> **用 AI + expert review + China-speed wet validation，在 8-12 周内帮你把一个 target 或候选物变成可立项、可停项、可 BD、可进入下一轮实验的证据包。**

中国优势：

1. ADC / 双抗 / TCE / biologics 项目密度高。
2. 国内 CRO、抗体表达、reagent、类器官、器官芯片和 wet-lab network 速度快、成本相对可控。
3. 国内创新药进入“差异化、出海、BD 和临床兑现”阶段，对 evidence package 的需求更强。
4. 大药企和头部 biotech 内部有平台，但仍需要外部速度、专家反驳和 human-relevant phenotype reward。

---

## 7. 风险与待验证问题

### 7.1 商业风险

1. 客户是否愿意把 early discovery 决策的一部分外包。
2. 项目制 ASP 是否能稳定站住 80-500 万人民币。
3. 客户是否接受 Frontis 作为项目空间和 evidence package 的组织者，而不是单纯 CRO 或模型供应商。
4. 大客户是否坚持私有化 / VPC，导致早期交付成本过高。

### 7.2 数据与 IP 风险

1. 客户数据必须 no-training-by-default。
2. Cross-customer training 只能 opt-in + 脱敏。
3. Foreground IP、background platform IP、专家 review、wet-lab raw data、negative data、衍生 reward model 的权属需要合同前置。
4. 外部 wet-lab partner 是否愿意交付 raw curve、raw image、negative data、SOP version、QC flags，不能只交 PDF 报告。

### 7.3 科学风险

1. 8-12 周内是否能产生足够有判断力的 wet reward。
2. Organ-chip / organoid phenotype reward 与真实临床转化之间的相关性仍需项目验证。
3. Expert review 能否结构化为 preference / critique / rubric，而不是一次性顾问意见。
4. Candidate Decision Package 是否真的改变客户的 continue / kill / BD 决策。

---

## 8. 建议更新 HTML 的方向

### 8.1 目标用户段落

建议把当前“20-200 人 biotech / discovery group”扩展成：

> 第一批客户是有明确 target / disease hypothesis / biologics candidate、需要在 8-12 周内完成 continue / kill / BD / next experiment 决策的早中期 discovery team。典型规模 20-200 人，已有 wet-lab 或 CRO 合作，但缺完整 AI platform、专家 review 和可训练 wet reward 闭环。

### 8.2 新增用户分层

建议在目标用户 section 里补一张四类用户 / 伙伴表：

| 类型 | 第一阶段角色 | 优先级 |
|---|---|---|
| ADC / 双抗 / TCE / biologics 项目型 biotech | 直接付费客户 | 最高 |
| 大药企 / 头部 biotech 单项目组 | Lighthouse pilot | 中高 |
| 科研机构 / 医院转化中心 / 国家平台 | 共研、clinical context、reward、科学背书、PI 孵化项目源 | 高，但不是收入主线 |
| CRO / 类器官 / 器官芯片 / wet-lab 平台 | Reward source、执行伙伴、渠道 | 高，但不是直接 ICP |

### 8.3 市场规模段落

建议新增一句：

> 我们不把市场定义为整个 AI drug discovery，而是更窄、更可交付的 AI-native discovery execution market：项目制 target-to-binder / candidate package、confidential project room、expert review、wet reward coordination 和长期 Science Agent OS。
