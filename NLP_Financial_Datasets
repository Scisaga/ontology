## 天池实验室数据集

0. [CCKS学术评测数据集汇总](https://tianchi.aliyun.com/dataset/136829)
1. [Daily Financial News for 6000+ Stocks](https://tianchi.aliyun.com/dataset/94123)
   - 2021年，英文，来源：benzinga.com
   - 超过6000只股票的每日财经新闻
   - 价值不高
2. [金融领域事件因果关系抽取数据集](https://tianchi.aliyun.com/dataset/110437)
   - 2021年，1.02MB
   - 该任务旨在从文本中抽取具有因果关系两个事件：原因事件和结果事件，并通过事件的四个要素来表示原因事件和结果事件。即给定文本T，抽取T中所有的原因事件M和结果事件N。
   - 格式较为奇怪，通用性差，价值不高
3. [Financial NER Dataset](https://tianchi.aliyun.com/dataset/145092)
   - Based on the four NE types provided in the CoNLL-2003 dataset: LOCATION (LOC), ORGANISATION (ORG), PERSON (PER), and MISCELLANEOUS (MISC).
   - 数据量小（112KB），只有实体类型标注，价值不高
4. [**面向金融领域的主体事件检测 ccks2023_task2**](https://tianchi.aliyun.com/dataset/159007)
   - 金融领域的公开新闻、报道
   - 同一实体可能包含多个事件
   - 103类风向事件类型
   - 可并入统一事件分析框架
5. [A股上市公司季度营收预测数据集](https://tianchi.aliyun.com/dataset/1074)
   - 包括历史财务数据、宏观数据、行情数据、行业数据。各数据包含的主要字段的名词解析以及财务数据的中英文对照
   - 财务数据包括三张表，分别为资产负债表 Balance Sheet、利润表 Income Statement、现金流量表 Cash Flow Statement。其中，由于非金融上市公司、证券、银行、保险四大行业的财务报表在结构上存在差异，所以每个类别又分为4个相对应的文档（csv格式）。这三张表代表了一个公司全部的财务信息，三大财务报表分析是投资的基础。
      - 资产负债表：代表一个公司的资产与负债及股东权益，资产负债表是所有表格的基础。
	  - 利润表：代表一个公司的利润来源，而净利润则直接影响资产负债表中股东权益的变化。
	  - 现金流量表：代表一个公司的现金流量，更代表资产负债表的变化。现金流量表是对资产负债表变化的解释。现金的变化最终反映到资产负债表的现金及等价物一项。而现金的变化源泉则是净利润。净利润经过“经营”、“投资”、“筹资”三项重要的现金变动转变为最终的现金变化。
   - 宏观数据 Macro Industry 是指一系列宏观经济学的统计指标， 包括生产总值(GDP)、国民总收入（GNI）、劳动者报酬、消费水平等。宏观经济周期是影响周期性行业的关键因素之一，对上市公司的经营情况也有直接的影响。
   - 行业数据 Industry Data 行业数据可以指示某个行业的发展态势，上市公司都会有自己所在的行业，分析行业的发展趋势、所处阶段等可对上市公司经营情况做出大体的判断（如从汽车行业每月的销量数据中，可以看到行业的景气程度）。
   - 公司经营数据 Company Operation Data 一般为月度数据，代表特定公司主营业务月度的统计值，与公司营收密切相关，每个公司指标不一样。
   - 行情数据 Market Data 行情数据代表上市公司股票月度交易行情，主要包括价格、成交量、成交额、换手率等。
   - 用途：数据对比补全
6. [A股上市公司公告信息抽取数据集](https://tianchi.aliyun.com/dataset/1075)
   - 可从公告中抽取以下几类事件：股东增减持、定向增发、重大合同等
   - 可以并入事件统一分析框架
7. [**CCKS2022金融领域FEW-SHOT事件抽取数据集 ccks2022**](https://tianchi.aliyun.com/dataset/136800)
   - 数据给的不全，100+事件类型中只给了16个类型，且每个类型只给了十条数据
   - train_data_final.txt：包含59,143条标注数据
   - 但还是很有价值，转化格式导入LabelStudio
   - 需并入事件统一分析框架
8. [CCKS2019金融领域篇章级事件主体抽取数据集](https://tianchi.aliyun.com/dataset/111237)
   - 相当于抽实体
   - [CCKS 2019 知识图谱评测技术报告：实体、关系、事件及问答](https://arxiv.org/ftp/arxiv/papers/2003/2003.03875.pdf)
   - 一般
9. [CCKS2020金融领域篇章级事件主体抽取数据集 ccks2020_subtask1](https://tianchi.aliyun.com/dataset/111209)
   - 包括互联网上的新闻文本，上市公司发布的公告文本（PDF文档已转成无结构化的文本内容）。
   - 事件类型包括：财务造假、偿付能力不足、高层失联/去世、企业破产、重大资损、重大赔付、重大事故、股权冻结、股权质押、增持、减持等。
   - 把发生特定事件类型的主体称为事件主体，如 “公司A向公司B赔付”对于事件类型“重大赔付”的事件主体是“公司A”。
   - event_entity_train_data_label.csv：包含72,515条标注数据
   - 只标注了类型和主体，一般，可尝试训练分类器
10. [**CCKS2020金融领域篇章级事件要素抽取数据集 ccks2020_subtask2**](https://tianchi.aliyun.com/dataset/111211)
   - 事件类型包括：财务造假、偿付能力不足、高层失联/去世、企业破产、重大资损、重大赔付、重大事故、股权冻结、股权质押、增持、减持等。
   - 事件要素为该事件类型的所有属性信息，如事件类型“破产清算”的事件要素包括“发布公告时间”、“破产清算的公司”、“受理法院”、 “公司所属行业”、 “裁定时间”。
   - 明确定义了要素的事件类型好像只有9种
   - 需并入事件统一分析框架
11. [CCKS2021金融领域篇章级事件元素抽取数据集](https://tianchi.aliyun.com/dataset/110904)
   - 数据集好像只有金融诈骗事件的数据
   - 即给定文本T抽取T中的13个事件要素
   - 通用性不高
12. [CCKS2021金融领域事件因果关系抽取数据集](https://tianchi.aliyun.com/dataset/110901)
   - 给定一段描述因果或影响关系的文本，从文本中抽取原因事件的表示和结果事件的表示。
   - 训练集是json格式，包含"text_id"、"text"、"reason_type"、"reason_region"、"reason_product"、 "reason_industry", "result_type"、"result_region"、"result_product"、"result_industry"字段，表示原因事件和结果事件的事件类型和三个事件要素。
   - 通用性不高
13. [AntSQL大规模金融语义解析数据集](https://tianchi.aliyun.com/dataset/139273)
   - AntSQL1.0数据集采用金融领域的表格作为数据源，涵盖了基金的产品和属性，主要聚焦单表查询问题，提供在此基础上的标注的Query-SQL对，希望选手们能在此基础上训练深度学习模型，将自然语言准确的转换为可查询的SQL语句。
   - 分析实体间关系
   - 可参考基金的特定事件类型
14. [AntCritic](https://tianchi.aliyun.com/dataset/142920)
   - 蚂蚁集团PGC/NEWS的论点论据结构数据集
   - https://github.com/ContentTech/AntCritic.git
