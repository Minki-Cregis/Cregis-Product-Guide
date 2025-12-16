# 支付链结（收银台）

Cregis 在 API 接口返回行业标准的收银台，供商户给付款人进行支付。商户可在网站付款页，跳转到收银台，支付完成后自动返回网页。减少商户对支付系统所需的开发和人力成本。

### 收银台支付流程



1.  在收银台，付款人可选择其一加密支付进行支付。如订单币种与支付币种不同，系统按实时汇率自动进行换算。（商户也可在 API 的 [`tokens`](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-engine-create) 进行限制支付币种）

    <div align="left"><figure><img src="../.gitbook/assets/螢幕截圖 2025-11-07 下午5.13.58.png" alt="" width="375"><figcaption></figcaption></figure></div>



2.  付款人也可在收银台查看订单信息，包括订单金额、订单号、商品内容等

    <div align="left"><figure><img src="../.gitbook/assets/螢幕截圖 2025-11-07 下午5.14.18.png" alt="" width="375"><figcaption></figcaption></figure></div>



3.  当选择支付币种后，付款人将需选举支付网路。

    <div align="left"><figure><img src="../.gitbook/assets/螢幕截圖 2025-11-07 下午5.14.30.png" alt="" width="375"><figcaption></figcaption></figure></div>



4.  选择完成后，系统将生成支付地址和二维码，付款人可复制地址或扫码完成支付。

    <div align="left"><figure><img src="../.gitbook/assets/螢幕截圖 2025-11-07 下午5.14.45.png" alt="" width="375"><figcaption></figcaption></figure></div>



5.  付款人也可选择第三方钱包进行扫码付款。扫码后，第三方钱包将自动录入币种、网络和金额，方便付款人直接确认。

    <div align="left"><figure><img src="../.gitbook/assets/螢幕截圖 2025-11-07 下午5.14.57.png" alt="" width="375"><figcaption></figcaption></figure></div>



6.  付款成功后，页面将跳到完成支付页面，5 秒后将自动返回到商家网站（在 API 提供的 [`success_url`](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-engine-create)字段）。如订单在付款后为[其他状态](https://support.cregis.com/cregis-wallet-guide/zh-tw/payment_engine/introduction)，完成支付页面也会提示原因及系统自动进入相对的流程如发送补款、部分退款或全额退款电邮等。

    <div align="left"><figure><img src="../.gitbook/assets/螢幕截圖 2025-11-07 下午5.02.11.png" alt="" width="375"><figcaption></figcaption></figure></div>



7.  若用户未在订单有效期内完成支付，订单将自动失效。付款人按「返回」，将回到在 API 提交的[`cancel_url`](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-engine-create)。

    <div align="left"><figure><img src="../.gitbook/assets/螢幕截圖 2025-11-07 下午5.21.35 (1).png" alt="" width="375"><figcaption></figcaption></figure></div>

