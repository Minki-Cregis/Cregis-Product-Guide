---
hidden: true
---

# Copy of 策略中心

## 什么是策略引擎？

策略引擎是Cregis于最新版本V.2.11.0推出的一款全面风险管理工具，专为用户提供灵活的出金管理方案。通过策略引擎，用户可以设置详细的规则和自动化执行动作，以规范和控制团队成员的出金请求。这项工具未来将支持自动签名和出款功能，还能显著提升工作效率和管理效能，减少人工操作中的风险。目前，策略引擎支持三种出金类型的策略定制，包括交易发送、付款申请以及API提币。用户可以根据具体的业务需求进行策略设计，例如限制特定币种的出金操作，或仅在指定的时间窗口内执行相关动作。这些灵活的配置选项，使得企业能够更加精确地控制资金流动，从而保障资产安全并优化操作流程。此外，策略引擎还提供了一个集中式的日志查看功能，用户可以直接在系统中查看和监控所有策略的执行情况。这一功能确保了所有出金活动的透明度，使得每一次操作都可以被完整追踪和审核，从而进一步提升了风险管理的严谨性与可控性。透过即时查看和分析策略日志，管理者能够迅速识别潜在问题，并做出相应的调整，确保企业资金的安全性和操作的合规性。<br>

## 操作手冊

1. ### 进入策略引擎页面

由「管理」>「策略」进入页面，按「建立决策」开始设置流程。

<figure><img src="../.gitbook/assets/image (399).png" alt=""><figcaption></figcaption></figure>

2. ### 建立决策

所有策略引擎必须先建立决策才可以建立规则，我们一共提供三种出款类型的配置，用户可根据业务需要进行设定并提交，提交后需要进行身份验证。

<figure><img src="../.gitbook/assets/image (400).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (401).png" alt=""><figcaption></figcaption></figure>

我们一共提供三种出款类型及执行动作的配置，以下是三种类型可供配置的执行动作：

| 出款类型   | 传送交易                                | 付款申请                                  | API提币                                 |
| ------ | ----------------------------------- | ------------------------------------- | ------------------------------------- |
| 设置出款钱包 | <ul><li>不需要</li></ul>               | <ul><li>需要</li></ul>                  | <ul><li>需要</li></ul>                  |
| 執行動作   | <ul><li>拒绝</li><li>发起审批流程</li></ul> | <ul><li>付款签名</li><li>发起审批流程</li></ul> | <ul><li>付款签名</li><li>发起审批流程</li></ul> |

* **执行动作：拒绝** 无须进行进阶设置，可直接提交。

<figure><img src="../.gitbook/assets/image (402).png" alt=""><figcaption></figcaption></figure>

* **执行动作：发起审批流程** 需要进行审批流设置，包括设定审批节点及签名人员。

<figure><img src="../.gitbook/assets/image (403).png" alt=""><figcaption></figcaption></figure>

* **执行动作：付款签名** 需要设定签名人员，由于直接签名只适用于付款申请及API提币，所以一般都必须设定出款钱包，完成后可提交。

<figure><img src="../.gitbook/assets/image (404).png" alt=""><figcaption></figcaption></figure>

\
成功创建后画面会直接跳到策略日志同时可看到你刚才建立决策的记录

<figure><img src="../.gitbook/assets/image (405).png" alt=""><figcaption></figcaption></figure>

你亦可以到执行决策页面查看自己已创建的执行决策。

<figure><img src="../.gitbook/assets/image (406).png" alt=""><figcaption></figcaption></figure>

3. ### 建立策略

到策略页面点击「+」开始建策略

*   **基本设置**\
    先为此策略设定名称、类型及相应的设置，同时亦要为此策略设定权重等级。当同时命中多条策略时，会执行权重等级最大的策略。举例：即策略A权重等级为10而策略B权重等级为5时，会优先执行策略A。

    <figure><img src="../.gitbook/assets/image (407).png" alt=""><figcaption></figcaption></figure>

    * 类型为传送交易时需要选择发起钱包
    * 类型为付款申请时则没有需要设置的地方
    * 类型为API提币时需要选择项目


*   **触发条件**

    完成基础设置后可以为策略设定规则，条件方面可根据金额大小或操作时间进行设置。用户可选择只是其中一个进行设置。<br>

    <figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=NWZjMzYwZmQ5ZDNkZjdkZWM2MDEzZjFiMzNhOTk3ZDBfaUR6WTVBUkNnTm9OUzFJRFRGVWdQaDFwblRuemZhbXdfVG9rZW46RFRNaWJvTVJtb1ZzdXF4NHJiS2xnMUtuZ09iXzE3Mjk3NjU2MDU6MTcyOTc2OTIwNV9WNA" alt=""><figcaption></figcaption></figure>
* **发起币种**\
  在此栏用户可先选择币种，如需指定币种则要为每个币都进行一次金额设定。用户可为单笔、单日或单月的金额进行限制。

<figure><img src="../.gitbook/assets/image (409).png" alt=""><figcaption></figcaption></figure>

* **操作时间** \
  操作时间则用完限制此策略类型的操作(传送交易、付款申请、API提币)，用户可选择全天或指定时间作为条件。如选择指定时间的话则需设定开始及结束时间，亦可增加多个时段。 \
  <mark style="color:green;">**请注意：此时间是以UTC+8作为标准**</mark><br>

<figure><img src="../.gitbook/assets/image (410).png" alt=""><figcaption></figcaption></figure>

* **命中方式** \
  用户可选择全部命中或部份命中，部份命中指只要命中了操作时间或发起币种的条件其中一项都会触发此策略。 此方式只在操作时间及发起币种的条件同时激活时适用，如只激活其中一个则不论全部命中或部份命中都是一样的决策逻辑。



* **命中后执行决策** \
  完成触发条件的设置后用户可选择命中条件，只决策可从用户过去建立的同类型中选择。

| 出款类型   | 传送交易                                | 付款申请                                  | API提币                                 |
| ------ | ----------------------------------- | ------------------------------------- | ------------------------------------- |
| 设置出款钱包 | <ul><li>不需要</li></ul>               | <ul><li>需要</li></ul>                  | <ul><li>需要</li></ul>                  |
| 執行動作   | <ul><li>拒绝</li><li>发起审批流程</li></ul> | <ul><li>付款签名</li><li>发起审批流程</li></ul> | <ul><li>付款签名</li><li>发起审批流程</li></ul> |

<mark style="color:green;">**请注意：用户可以为钱包设定多于一条的规则，每条规则的关系是「或者」**</mark>

*   设定完成后需进行身份认证。

    <figure><img src="../.gitbook/assets/image (411).png" alt=""><figcaption></figcaption></figure>
*   完成后会跳到策略页面，用户需要激活策略，在成功激活前需要进身份及Google双重验证。<br>

    <figure><img src="../.gitbook/assets/image (412).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../.gitbook/assets/image (413).png" alt=""><figcaption></figcaption></figure>



* **完成双重验证后整个策略引擎正式建立完成。**

4. ### 编辑及删除策略

* 编辑策略\
  已建立的策略可以在策略页面进行编辑，进行编辑前必须先禁用策略，禁用时亦需要进行身份验证。

<figure><img src="../.gitbook/assets/image (414).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (415).png" alt=""><figcaption></figcaption></figure>

* 删除策略 \
  删除已建立的策略可以在策略页面中进行，删除前必须先禁用策略，禁用时亦需要进行身份验证。

<figure><img src="../.gitbook/assets/image (416).png" alt=""><figcaption></figcaption></figure>

5. ### 查看策略日志

进入策略日志可以看到每一个策略的动作，包括日期时间、操作人员及动作。

<figure><img src="../.gitbook/assets/image (417).png" alt=""><figcaption></figcaption></figure>

在此页面用户亦可根据操作日期、操作人或策略类型进行筛选

<figure><img src="../.gitbook/assets/image (418).png" alt=""><figcaption></figcaption></figure>

同时搜寻栏亦支持使用决策／策略名称及编号去搜寻相关记录。

<figure><img src="../.gitbook/assets/image (419).png" alt=""><figcaption></figcaption></figure>

另外在日志中如有触发动作亦可以检视命中日志，按下后会可查看命中详情包括命中策略清单等。

<figure><img src="../.gitbook/assets/image (420).png" alt=""><figcaption></figcaption></figure>

## 触发策略的动作

目前可以触发的动作一共有三种，以下为每个动作执行时的画面。

* 拒绝 \
  如触发拒绝，画面会弹出视窗表示操作失败并通知用户所触发的策略。

<figure><img src="../.gitbook/assets/image (421).png" alt=""><figcaption></figcaption></figure>

* 发起审批流程

如触发审批流程就会弹出温馨提示并通知用户所触发的策略。

<figure><img src="../.gitbook/assets/image (422).png" alt=""><figcaption></figcaption></figure>

* 付款签名 \
  如进行付款签名动作则不会有视窗弹出，但查看发起需求详情时可查看到命中策略

<figure><img src="../.gitbook/assets/image (423).png" alt=""><figcaption></figcaption></figure>

## 实际使用场景

实际的设置需根据用户自身需求进行，以下是一些场景的策略引擎设置\
**场景一：我想限制比特币的出款，所有比特币相关的出款必须经过审批，并没有使用API服务。** 这种情况下用户需要同时设定两种类型的策略，分别是传送交易及付款申请，两种类型的触发条件及执行动作内容如下：

* 触发条件设置
  * 选择指定币种Bitcoin，并把所有传送限额设成大于等于0时就触发条件。

<figure><img src="../.gitbook/assets/image (424).png" alt=""><figcaption></figcaption></figure>

* 执行动作设定
  * 执行动作选择「发起审批流程」，设置相应的审批人员及签名人员。

<figure><img src="../.gitbook/assets/image (425).png" alt="" width="375"><figcaption></figcaption></figure>

**场景二：低于USD $50 的小额付款申请都无需审批直接进入签名流程**

* 触发条件设置

<figure><img src="../.gitbook/assets/image (426).png" alt="" width="375"><figcaption></figcaption></figure>

* 执行动作设定
  * 由于只是套用于付款申请，所以只需要开设一个策略并设定签名人员及出款钱包。

<figure><img src="../.gitbook/assets/image (427).png" alt="" width="375"><figcaption></figcaption></figure>

\
<br>

## 升级策略数目

目前基础版只允许创建两个策略及两个执行决策，而每个策略亦只可以套用于一个钱包。如需升级策略数目，用户可到帐户权益页面进行升级或扩容服务。

<figure><img src="../.gitbook/assets/image (428).png" alt=""><figcaption></figcaption></figure>

1. ### 升级团队套餐

用户可根据自身业务选择升级到商业版或企业版。

<figure><img src="../.gitbook/assets/image (429).png" alt=""><figcaption></figcaption></figure>

2. ### 扩容策略

除升级团队套餐外，用户亦可选择只升级可创建的策略数目，点击「扩容」进入画面，然后选择所需的策略数量，每个策略数量需支付$19美元。

<figure><img src="../.gitbook/assets/image (431).png" alt=""><figcaption></figcaption></figure>
