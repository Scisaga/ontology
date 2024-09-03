## 事件本体定义
### 事件类型
基本原则：
1. 所有事件的父类型：Evt
2. 一个事件类型可以有0-n个子事件类型，一个子事件类型可以隶属于1-n个父节点（公司高管变动和人物职位变动是一个事件，但可以隶属于两个父节点：公司人事事件/人物事件），整个事件类型是一个多叉树
3. 子事件类型会继承父事件类型的论元定义，子事件类型的链式延申是对事件类型定义的层层细化
4. 为了更好的维护现实一致性，事件类型将尽量与Wikidata中的Q节点进行关联
5. 根据事件的出现上下文，可以分为：文本、表格
   - 本文将金融和财经指标的作为事件进行定义，大量财经指标数据以表格形态出现
6. 扩展子事件类型：
   - Α 起止事件簇：事件【开始/结束】，事件通常需维持较长时间，具有状态属性；
   - Ε 预期事件簇：当前值【强于/符合/弱于】预期
   - Δ 变化事件簇：当前值【同比/环比】【增长/下降/保持】

#### 事件类型定义
1. 宏观经济事件 / Macro Economics Event / macro_econ_evt
   - 政策发布 / Policy Event / plcy_evt
      - 财政政策 / Fiscal Policy / plcy_fiscal_evt
	     - 预算
		 - 税收
		 - 国债 / 地方债
		 - 财政补贴
	  - 货币政策 / Monetary Policy / plcy_monetary_evt
	     - 新增贷款
		 - 公开市场操作 逆回购 SLF TLF
		 - 存款准备金率
		 - 再贴现与再贷款
		 - 利率 存贷款基准利率 LPR
		 - 常备借贷便利 SLF
		 - 中期借贷便利 MLF
		 - 抵押补充贷款 PSL
	  - 贸易政策 / Trade Policy / plcy_trade_evt
	     - 关税措施
		 - 进口管制
		 - 出口信贷
		 - 出口补贴
		 - 出口管制
	  - 汇率政策 / Exchange Rate Policy / plcy_ex_event
	     - 外汇储备
		 - 资本外流
		 - 汇率变化
		 - 外汇存款准备金率
		 - 外汇风险准备金率
		 - 跨境融资宏观审慎调节参数
		 - 逆周期因子
	  - 资本账户政策 / Capital Account Policy / plcy_ca_evt
   - 市场监管事件 / Market Regulatory Event / mkt_reg_evt (医药反腐，相关行业和主管部门)
   - 经济指标事件 / Economic Indicator Event / econ_id_evt
      - CPI / PPI / PMI 等一系列经济指标事件 `${name}_evt`
	     - 强于预期 `${name}_se_evt`
		 - 符合预期 `${name}_me_evt`
		 - 弱于预期 `${name}_we_evt`
1. 微观经济事件（经济实体事件/公司事件） / Micro Economics Event / micro_econ_evt
   - 投融资事件 / Investment Event / invt_evt
   - 并购事件 / Merger and Acquisition Event / ma_event
   - 运营事件 / Operation Event / op_event
      - 创建
	  - 关闭
   - 商务事件 / Business Event / biz_evt
	  - 支付
      - 合作 / Deal Event / deal_evt
	  - 中标 / Bid Winning Event / bid_winning_evt
   - 财务事件 / Financial Event / fin_evt
      - 公司市值
	  - 营业收入
	     - 销售收入
	  - 支出
	     - 研发支持
	  - 利润
	     - 净利润
		 - 归母净利润
		 - 扣非净利润
	  - 现金流
	  - 资产收益率 ROE
	     - 加权平均净资产收益率
		 - 扣费加权平均净资产收益率
	  - 每股收益 EPS
	     - 基本每股收益
		 - 稀释每股收益
		 - 扣非每股收益
	  - 资产负债率
	  - 市盈率 PE
	  - 市净率 PB
	  - 市消率 PS
	  - 派息/分红
	  - 配股
   - 法务事件
      - 行政处罚
      - 诉讼
	  - 定罪 / 和解
	  - 无罪
	  - 上诉
   - 人事事件
      - 聘用 / Employment
	  - 薪酬变化
   - 产品事件 / Product Development Event / pd_event
      - 发布
	  - 定价
	  - 测试
	     - 测试成功
		 - 测试失败
	  - 终止/召回
	  - 热销
	  - 滞销
   - 品牌事件 / Brand Event / brand_event
1. 交易品/证券事件
   - 价格变动
   - 研究报告评级
      - 购买
	  - 卖出
	  - 持有
	  - 评级
	  - 预测目标价格
1. 科学/技术事件
   - 新理论/技术/发现/发明的发布（领域/机构/人/名称/简称/时间）
1. 地缘事件
   - 自然灾害
   - 环境污染
   - 突发事故
   - 农业事件
1. 政治事件
   - 军事冲突
1. 生命事件
   - 出生
   - 死亡
   - 受伤
   - 生病
   - 住院

## 事件触发词 Trigger
事件的触发词是最简明地表达事件发生的文本跨度（一个单词或小短语）。通常，它是描述动作或状态的主要动词。一般来说，我们认为触发词是最明确指代事件的单词。

## 事件论元 Arguments
事件描述了世界中的状态变化，涵盖了行为、关系、事件等。这些事件涉及多个参与实体，以不同方式参与其中：作为主体（发起者/引发者）、受事者（目标/承受者、主题）、限定词、数量词、特定描述修饰语以及其他描述性修饰语。例如，执行动作的人或公司、涉及的股份数量或其他信息，比如事件发生的地点等。我们将事件中这些参与实体和参数称之为论元，每个事件都有若干对应的论元，对于特定的一种事件类型，其论元的角色数量是固定的。不同的事件类型的论元角色有所差异，子事件类型会继承父事件类型的论元角色。论元角色可以分为以下两种：

### 参与方 Participant ###
在事件提及范围中出现，可以是代词

代词提及共指：
1. 标注代词最近可明确表明指代实体的**专有名词/名词组合**
2. 本质上是关系标注

### 通用参数 Filler
   - 可在上下文距离较远的位置出现，必须是名词
   - 时间 TIME
   - 地点 PLACE
   - 数量 AMOUNT

## 事件事实性 Factuality
1. 极性 / Polarity
   - 肯定 / Positive
   - 否定 / Negative
1. 时态 / Tense
   - 过去 / Past
   - 现在 / Present
   - 未来 / Future
   - 未确定 / Unspecified
1. 一般/特例 / Genericity
   - 一般 / Generic
   - 特例 / Specific
1. 模态 / Modality
   - 确信 / Believed
   - 假设 / Hypothetical
   - 命令和请求 / Commanded
   - 威胁、提议和讨论 / Proposed
   - 期望 / Desired
   - 许诺 / Promised
   - 其他 / Other
1. 强度
   - 强化 / Intensified
   - 中性 / Neutral
   - 缓和 / Eased

参考：
1. [zotpress items="{12427172:59KHJZ6H}" style="apa"]

## 事件模板

## 事件关系

### 事件之间时序关系
1. i is before j (<)
1. i meets j (m)
1. i overlaps j (o)
1. i starts j (s)
1. i is during j (d)
1. i finishes j (f)
1. i is overlapped by j (oi)
1. i is met by j (mi)
1. i is after j (>)
1. i equals j (=)
1. i is finished by j (fi)
1. i has j during it (di)
1. i is started by j (si)

参考：
- [zotpress items="{12427172:TBLXLTQV}" style="apa"]

### 事件的共指
1. 相同类型和子类型，描述的同一事件，在触发词上标注；链指标注：A --> B, B --> C
2. Event Hopper: 指向同一事件的一堆事件

## 事件提取处理逻辑
1. 分段，段落分割：长度最大512，按句子切分。
2. 文本多标签预测（multi label）：提取超过一定阈值事件类型预测结果
3. 整理该类型下的提示文本，结合已微调的UIE模型进行预测
4. 记录推理结果

## 参考
1. [SENTiVENT Event Annotation Guidelines v1.1](https://biblio.ugent.be/publication/8644921)
