## 概述
实体类型的定义非常重要，是整个事件本体定义的基石，我们需要关注三种类型的实体：
- **命名实体（Named Entity）**：文中的实体提及通常指特定的一个事物；
- **名义实体（Nominal Entity）**：一类事物的统称、非可数名词如时间；
- **代词（Pronominal Entity）**：指代上下文的其他命名实体。

实体类型的定义主要参考了传统ACE/ERE中的实体类型、KBP RUFES 2022中第一层级实体类型和COfEE中的实体类型。

### 命名方式
- **大写简称**：ACE/ERE等较老的事件本体定义中出现过的实体类型；
- **首字母大写拼接**：KBP2022-RUFES中出现的扩展实体类型、新的不断扩充的实体类型。

### Wikidata 引用
- 维基数据（Wikidata）是一个由维基媒体基金会托管的开放式、协作性的包含事实主题的知识库；
- Wikidata的结构是一个图形数据库，由实体、属性和关系组成。Wikidata已经有超过1亿条记录和5w活跃编辑者；
- 在实体类型定义中，会同时记录Wikidata中的Q/P节点，作为实体类型的事实依据和扩展基础。

## 实体类型列表

### Animal
- 描述：动物，例如羊驼
- WD：[Q729 animal](https://www.wikidata.org/wiki/Q729)

### APP
- 描述：PC/主机/收集应用程序，例如Google Earth，YouTube，BiliBili
- WD：[Q166142 application](https://www.wikidata.org/wiki/Q166142)

### ConsumerGoods
- 描述：消费产品，包括日用品、食物、家具、3C产品、机械设备零件等
- WD：[Q868404 final good](https://www.wikidata.org/wiki/Q868404)

### ContactInfo
- 描述：联系方式，如URL，Email，电话号码
- WD：[Q2996679 contact information](https://www.wikidata.org/wiki/Q2996679)

### Document
- 描述：法律文档、证书、一般文档如书信、消息等
- WD：[Q49848 document](https://www.wikidata.org/wiki/Q49848)

### FAC
- 描述：设施机构，人工建造物，如办公楼、桥梁、机场、地铁站、高速公路等
- WD：[Q13226383 facility](https://www.wikidata.org/wiki/Q13226383)

### GPE
- 描述：Geo-Political Entity，地缘政治实体，国家、地区、城市等
- WD：[Q1048835 political territorial entity](https://www.wikidata.org/wiki/Q1048835)

### IllHealth
- 描述：疾病症状如盲肠炎、下腹痛等
- WD：[Q2057971 health problem](https://www.wikidata.org/wiki/Q2057971)

### LAW
- 描述：法案，包括行政法规如：《关于促进汽车消费的若干措施》
- WD：[Q7748 law](https://www.wikidata.org/wiki/Q7748)

### LOC
- 描述：地理地点，自然地点，如山、岳、江、河、湖、海、沙漠、沼泽和具体的地址
- WD：[Q27096213 geographic entity](https://www.wikidata.org/wiki/Q27096213)

### MED
- 描述：疫苗、药物、抗生素等
- WD：[Q12140 medication](https://www.wikidata.org/wiki/Q12140)

### NUM
- 描述：数字，数值，包含对应的度量单位（如美元、米、特斯拉等）
- WD：[P1181 numeric value](https://www.wikidata.org/wiki/P1181)

### Occupation
- 描述：职业，职位
- WD：[Q12737077 occupation](https://www.wikidata.org/wiki/Q12737077)

### ORG
- 描述：组织机构、包括社团、公司、法院、教育机构、犯罪组织、政府和政治团体（如联合国）
- WD：[Q43229 organization](https://www.wikidata.org/wiki/Q43229)

### Pathogen
- 描述：病原体、细菌病毒等
- WD：[Q170065 pathogen](https://www.wikidata.org/wiki/Q170065)

### PER
- 描述：人物
- WD：[Q215627 person](https://www.wikidata.org/wiki/Q215627)

### PN
- 描述：代词
- WD：[Q36224 pronoun](https://www.wikidata.org/wiki/Q36224)

### Publication
- 描述：出版物、文章、书籍、算法、软件、模型等
- WD：[Q732577 publication](https://www.wikidata.org/wiki/Q732577)

### Time
- 描述：时间，关于事务先后顺序、过去与未来的物理量
- WD：[Q11471 time](https://www.wikidata.org/wiki/Q11471)

### VEH
- 描述：通用载具，飞机、火箭、航空器、舰艇、汽车、摩托车、火车等
- WD：[Q42889 vehicle](https://www.wikidata.org/wiki/Q42889)

### WEA
- 描述：武器装备，近战武器（刀枪剑戟）、爆炸物、枪械、导弹、非致命性武器、武器系统、大规模杀伤性武器
- WD：[Q728 weapon](https://www.wikidata.org/wiki/Q728)

## TODO
1. [ ] 增加子层级的实体类型定义
2. [ ] 增加财经金融类型的实体类型定义

## Ref
1. Linguistic Data Consortium. (2016). Rich ERE Annotation Guidelines Overview V4.2. https://tac.nist.gov/2016/KBP/guidelines/summary_rich_ere_v4.2.pdf
2. Balali, A., Asadpour, M., & Jafari, S. H. (2022). Cofee: A Comprehensive Ontology for Event Extraction from Text. SSRN Electronic Journal. https://doi.org/10.2139/ssrn.4117538
3. RUFES 2022 Annotation Guidelines (V1.0). (2022). https://tac.nist.gov/2023/KBP/RUFES/guidelines/TAC-KBP2022-RUFES-AnnotationGuidelinesV1.0.pdf
