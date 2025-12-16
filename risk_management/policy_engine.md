# 策略中心

## 什么是策略引擎？

策略引擎是Cregis于最新版本V.2.11.0推出的一款全面风险管理工具，专为用户提供灵活的出金管理方案。通过策略引擎，用户可以设置详细的规则和自动化执行动作，以规范和控制团队成员的出金请求。这项工具未来将支持自动签名和出款功能，还能显著提升工作效率和管理效能，减少人工操作中的风险。目前，策略引擎支持三种出金类型的策略定制，包括交易发送、付款申请以及API提币。用户可以根据具体的业务需求进行策略设计，例如限制特定币种的出金操作，或仅在指定的时间窗口内执行相关动作。这些灵活的配置选项，使得企业能够更加精确地控制资金流动，从而保障资产安全并优化操作流程。此外，策略引擎还提供了一个集中式的日志查看功能，用户可以直接在系统中查看和监控所有策略的执行情况。这一功能确保了所有出金活动的透明度，使得每一次操作都可以被完整追踪和审核，从而进一步提升了风险管理的严谨性与可控性。透过即时查看和分析策略日志，管理者能够迅速识别潜在问题，并做出相应的调整，确保企业资金的安全性和操作的合规性。<br>

## 操作流程

### 创建策略

进入策略中心页面，点击"策略"。

<figure><img src="../.gitbook/assets/image (629).png" alt=""><figcaption></figcaption></figure>

点击"+"创建策略，先为策略命名然后选择相应的类型，类型分为人工转出以及API转出：

* 人工转出：通过客户端转出的交易，包括钱包手动转出，以及项目内地址的手动转出
* API转出：即通过API转出的交易，包括所有针对WaaS项目发出的钱包出款或是项目地址出款

<figure><img src="../.gitbook/assets/image (630).png" alt=""><figcaption></figcaption></figure>

选择好类型后可以新增规则，<mark style="color:green;">**请注意：用户可以为钱包设定多于一条的规则，每条规则的关系是「或者」。**</mark>你可以根据你实际的场景进行触发规则以及执行动作，最后提交并进行验证即可成功创建。

<figure><img src="../.gitbook/assets/image (650).png" alt=""><figcaption></figcaption></figure>

### 编辑及删除策略

你可以在以下地方找到编辑及删除的入口

<figure><img src="../.gitbook/assets/image (643).png" alt=""><figcaption></figcaption></figure>

### 查看日志

你可以從以下地方找到日志，可以看到每个操作的时间及操作人。

<figure><img src="../.gitbook/assets/image (644).png" alt=""><figcaption></figcaption></figure>

## 触发规则说明

**发起操作配置**

规则的触发条件会根据策略类型有所不同，人工转出需要配置成员及出款钱包，而API转出则要配置WaaS项目及出款的操作。

<figure><img src="../.gitbook/assets/image (654).png" alt=""><figcaption></figcaption></figure>

**操作时间**

操作时间是用于限制此策略类型的操作(人工转出、API转出)，用户可选择全天或指定时间作为条件。如选择指定时间的话则需设定开始及结束时间，支持设置多个时段。\
<mark style="color:green;">**请注意：此时间是以UTC+8作为标准**</mark>

**发起币种**

在此栏用户可选择发起的币种，可选择任意币种或指定币种。

* 金额条件说明：用户可为选择的发送币种设置单笔、单日或单月的金额进行限制。

## 执行动作说明

我们一共提供三种执行动作的配置，以下是三种类型可供配置的执行动作：

* **拒绝：**&#x7CFB;统自动拒绝出款

<figure><img src="../.gitbook/assets/image (651).png" alt=""><figcaption></figcaption></figure>

* **审批：**&#x9700;要进行审批流设置，包括设定审批节点及签名人员。

<figure><img src="../.gitbook/assets/image (652).png" alt=""><figcaption></figcaption></figure>

* **签名：**&#x9700;要设定签名人员

<figure><img src="../.gitbook/assets/image (641).png" alt=""><figcaption></figcaption></figure>

## 实际使用场景

实际的设置需根据用户自身需求进行，以下是一些场景的策略引擎设置\
**场景一：我想限制比特币的出款，所有比特币相关的出款必须经过审批，并没有使用API服务。** 两种类型的触发条件及执行动作内容如下：

*   触发条件设置

    * 选择指定币种Bitcoin，并把所有传送限额设成大于等于0时就触发条件。

    <figure><img src="../.gitbook/assets/image (645).png" alt="" width="299"><figcaption></figcaption></figure>
*   执行动作设定

    * 执行动作选择「发起审批流程」，设置相应的审批人员及签名人员。

    <figure><img src="../.gitbook/assets/image (646).png" alt="" width="326"><figcaption></figcaption></figure>

**场景二：于工作外的时间如晚上7点至明早7点不允许所有出款申请。**

* 触发条件设置
  * 这里要注意需分开两个时间做设置

<figure><img src="../.gitbook/assets/image (648).png" alt="" width="303"><figcaption></figcaption></figure>

*   执行动作设定

    * 直接选择拒绝即可

    <figure><img src="../.gitbook/assets/image (649).png" alt="" width="337"><figcaption></figcaption></figure>

\
<br>
