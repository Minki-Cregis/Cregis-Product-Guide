---
description: 本章会逐步说明如何创建项目、设定权限、提币外部验证、API 对接及通知设定。
---

# 开始使用

* 创建项目（建议由业务负责人或指定代表完成项目创建）<br>
  1.  创建项目：若您尚无任何项目，可从 WaaS 落地页直接创建；若已拥有 WaaS 项目，可在项目下拉清单中点击「创建项目」。

      <figure><img src="../../.gitbook/assets/image (1232).png" alt=""><figcaption></figcaption></figure>

      <figure><img src="../../.gitbook/assets/image (1233).png" alt=""><figcaption></figcaption></figure>


  2.  输入项目名称

      <figure><img src="../../.gitbook/assets/image (1235).png" alt=""><figcaption></figcaption></figure>


  3.  开启「收款方式」开关，并选择「订单模式」

      <figure><img src="../../.gitbook/assets/image (1236).png" alt=""><figcaption></figcaption></figure>


  4.  若您想使用 Cregis 内建收银台页面，强烈建议填写商户名称及商户标志，让您的客户进入收银台时能认出您的品牌。若留空，收银台页面仍可使用，但不会显示任何名称或标志。您亦可稍后在「设定」的「商户资料」页面更改。

      <figure><img src="../../.gitbook/assets/image (1237).png" alt=""><figcaption></figcaption></figure>


  5.  若您期望不只收款，还需要提币，可一并开启「提币」开关并选择提币钱包。请注意：一旦启用，该项目即可提交 API 提币请求。此 API 请求是钱包签名前的提币流程步骤。

      <figure><img src="../../.gitbook/assets/image (1238).png" alt=""><figcaption></figcaption></figure>


  6.  点击「创建」，并继续前往「收款及转账」页面。

      <figure><img src="../../.gitbook/assets/image (1239).png" alt=""><figcaption></figcaption></figure>


  7.  最后一步是设定收款的转账地址：针对每个想收款的支付币种，选择其中一个转账钱包及其钱包地址。完成此处的币种设定后，该支付币种才可开始收款。您之后可随时回到「设定」中的「收款及转账」页面更改。

      <figure><img src="../../.gitbook/assets/image (1240).png" alt=""><figcaption></figcaption></figure>


  8.  您可以为不同团队成员指派不同角色及权限。下表为 WaaS 订单模式专属的权限\
      \
      \- 允许退款及异常支付单转账：允许处理退款及异常支付单的转账\
      \
      \- 编辑转账设定：允许设定转账钱包及钱包地址\
      \
      适用于 WaaS 订单模式及 WaaS 子地址模式的通用权限，请参阅[团队角色页面](https://support.cregis.com/team/role)。<br>

      <figure><img src="../../.gitbook/assets/image (1241).png" alt=""><figcaption></figcaption></figure>


  9.  提币外部验证：您可启用外部验证以加强安全性。请参阅[详细资讯](https://support.cregis.com/api/api-manual/payout-external-verification)。

      <figure><img src="../../.gitbook/assets/image (1242).png" alt=""><figcaption></figcaption></figure>


* 对接指引（适用于指定开发团队）<br>
  1.  取得对接密匙 - 前往「设定」下的「开发者」页面，找出对接所需的项目 ID、API Key 及 Base URL。以项目 ID 作为 API 请求中的 pid 参数；依照[签名指南](https://developers.cregis.com/zh/waas-authentication/)，使用 API Key 生成 sign 参数；并以 Base URL + Path（例如 https://t-abcdefgh.cregis.dev + /api/v1/create\_order）作为 API 请求端点。请注意：切勿轻易向他人透露项目的 API Key，以免造成资产损失。

      <figure><img src="../../.gitbook/assets/image (1244).png" alt=""><figcaption></figcaption></figure>


  2.  将请求 IP 加入白名单：请求 API 前，您必须先将请求 API 装置的 IP 地址加入 IP 白名单以确保安全；否则 API 会回传错误。您可在「IP 白名单」中点击「创建群组」、输入 IP 地址、点击「储存」，然后完成授权验证。

      <figure><img src="../../.gitbook/assets/image (1245).png" alt=""><figcaption></figcaption></figure>


  3.  开始对接：设定完成后，开发团队即可使用「创建订单」请求创建订单、取得相关资料并展示给付款方完成付款。详情请参阅第 3 部分「付款方介面」，了解如何向付款方展示资料。开发团队亦可使用「查询订单」查阅历史订单及该订单的最新状态。此外，Cregis 系统会透过回调讯息，就订单、退款及异常支付的不同状态作即时更新。

      <figure><img src="../../.gitbook/assets/image (1246).png" alt=""><figcaption></figcaption></figure>



3. 通知设置<br>
   1.  「通知」页面：您可在「设定」下的「通知」页面设定项目的通知规则。共有 4 种类型的通知：\
       \
       i. 回调异常（客户端内通知）: 当回调无法送达回调网址时\
       \
       ii. 启用／停用项目（客户端内通知＋电邮）: 当商户在「设定」下的「开发者」页面启用或停用项目时\
       \
       iii. 重设 API Key（客户端内通知＋电邮）：当商户在「设定」下的「开发者」页面点击并确认重设 API Key 时\
       \
       iv. 团队余额不足以扣除服务费（客户端内通知＋电邮）：当服务费总额大于团队余额时\
       \
       v. 异常支付通知（电邮）：当收到异常支付时

       <figure><img src="../../.gitbook/assets/image (1247).png" alt=""><figcaption></figcaption></figure>


   2.  启用或停用：您可透过开关启用或停用每项通知。

       <figure><img src="../../.gitbook/assets/image (1248).png" alt=""><figcaption></figcaption></figure>


   3.  选择接收人：您可点击「编辑」，勾选需接收通知的指定团队成员。

       <figure><img src="../../.gitbook/assets/image (1249).png" alt=""><figcaption></figcaption></figure>

       \
       \
       <br>
