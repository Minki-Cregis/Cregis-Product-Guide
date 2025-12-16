# 简介

Cregis 加密收单支付工具为企业提供一站式加密支付解决方案，商户只需通过简单的 API 接口即可快速接入。我们提供已设计好的收银台供直接使用，商户也可根据需求自行设计界面。当商户发起付款请求时，系统将生成专属收款地址，资金会进入Cregis钱包并通过自动结算机制快速转入商户指定钱包。商户可通过Cregis 客户端随时查看订单状态、结算数据及其他交易详情，轻松管理支付流程。我们支持多链多币种支付，确保资金流转高效灵活，为客户提供安全便捷的加密货币支付体验。



## 支付规则

Cregis 支持多种币种及网络作为[订单币种](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-order-currency)、[支付币种及结算币种](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-pay-currency)，包括法定货币及加密货币。如订单币种与支付币种不同，Cregis 将实时获取最新汇率，并在订单有效期内进行换算及锁定该汇率不变。



## 结算规则

* **常规结算**：若待结算金额达到或超过 50 USDT 等值（测试阶段）／500 USDT 等值（正式阶段），将每 10 分钟结算一次。
* **兜底结算**：若待结算金额累计持续少于 50 USDT 等值（测试阶段）／500 USDT 等值（正式阶段），将触发兜底结算，24 小时内至少给商家结算一次。为了方便商家测试收单功能，对于商家接入后，首次收单，若收单金额少于 50 USDT 等值，都会在 10 分钟内自动触发兜底结算。
* **结算金额**：金额会在扣除交易手续费后入帐
* **结算地址**：商户可在建立支付引擎时选择 Cregis 钱包内部地址，结算后可结算到外部。
* **汇率结算**：按照 CoinMarketCap 的即时汇率计算，并以订单建立时的汇率为准

如有法币结算需求，可[联系我们](https://www.cregis.com/zh/appointment/)查询。



### 订单状态

| 订单状态 | 接受／设定上下限「超额支付」或「部分支付」 | 订单已支付 & 将结算 | 描述             |
| ---- | --------------------- | ----------- | -------------- |
| 待支付  | 不适用                   | ✗           | 订单已创建，但未过有效时间。 |
| 已过期  | 不适用                   | ✗           | 订单已创建及已过有效时间。  |
| 已支付  | ✗                     | ✓           | 应收金额 = 实付金额    |
| 超额支付 | ✓                     | ✓           | 应收金额 < 实付金额    |
| 部分支付 | ✓                     | ✓           | 应收金额 > 实付金额    |



## 补款规则

### 触法条件

如支付有以下的所有条件，订单将进入补款流程及返回[`paid_partial`](https://developer-cn.cregis.com/api-reference/callback/payment-engine)回调。

1. 订单不接受部分支付
2. 首笔支付
3. 实付金额 < 订单金额 或 实付金额 < 订单金额 - 部分支付限额（[`underpaid_tolerance`](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-engine-create)）
4. 支付币种为稳定币



### 补款流程

1. 系统会发送补款通知邮件至付款（邮箱会发至订单创建时提交的[`payer_email`](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-engine-create)）
2. 付款人可通过电邮提供的链结进入付款页
3. 支付币种和网络将与第一次支付相同
4. 补款金额会根据原订单的币种金额按汇率进行换算，再相减已支付的金额
5. 补款时效有 24 小时限制，超出时效，订单将自动进行全额退款
6. 成功补款后，将返回[`paid_remain`](https://developer-cn.cregis.com/api-reference/callback/payment-engine)回调



## 退款规则

### 部分退款

#### 触发条件

如订单有以下的所有条件，订单将进入部分退款流程及返回[`paid_over`](https://developer-cn.cregis.com/api-reference/callback/payment-engine)回调。

1. 订单不接受超额支付
2. 实付金额 > 订单金额 或 实付金额 > 订单金额 + 超额支付限额（[`overpaid_tolerance`](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-engine-create)）
3. 支付币种为稳定币



#### 部分退款流程

1. 系统会发送部分退款通知邮件至付款人（邮箱会发至订单创建时提交的[`payer_email`](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-engine-create)）
2. 付款人可通过电邮提供的链结进入部分退款页
3. 退款币种和网络将与第一次支付相同
4. 部分退款金额会根据实付金额，再相减按汇率进行换算原订单的币种金额
5. 部分退款时效有 24 小时限制，超出时效，订单将自动进行全额退款
6. 成功部分退款后，订单将进行结算。



### 全额退款

#### 触发条件

如订单有以下的其一条件，订单将进入全额退款流程

1. 订单不接受部分支付、以非稳定币支付及部分支付
2. 补款没有在 24 小时内完成
3. 部分退款没有在 24 小时内完成
4. 补款在第二次支付后，仍然 实付金额 < 订单金额 或 实付金额 < 订单金额 - 部分支付限额（[`underpaid_tolerance`](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-engine-create)）

#### 全额退款流程

* 系统会发送全额退款通知邮件至付款人（邮箱会发至订单创建时提交的的[`payer_email`](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-engine-create)）
* 付款人可通过电邮提供的链结进入全额退款页
* 退款币种和网络将与第一次支付相同
* 全额退款金额会根据已支付的所有实付金额
* 全额退款时效有 24 小时限制
* 如超出 24 小时时效，需联络客服处理后续情况。
* 完成退款后，系统将返回[`refunded`](https://developer-cn.cregis.com/api-reference/callback/payment-engine)回调。



### 其他退款事项



* 每笔退款将收取相应手续费，手续费金额将在退款申请页面明确显示并将直接从退款金额中扣除。









<br>
