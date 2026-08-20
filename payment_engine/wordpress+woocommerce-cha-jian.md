---
hidden: true
---

# WordPress+WooCommerce 插件

## 简介



**什么是 WordPress 及 WooCommerce?**

WordPress 是全球最受欢迎的网站管理系统之一。它是一个开源平台，让任何人都可以在不需要大量技术知识的情况下创建和管理网站。 WooCommerce 是一个免费的 WordPress 电商插件，可以将您的 WordPress 网站转变为功能完整的网上商店。关键区别在于 WordPress 是通用的网站创建平台，而 WooCommerce 专门为电商设计，运行在 WordPress 之上。



**什么是 Cregis Payment** 于 **WooCommerce?**

Cregis Payment 于 WooCommerce 是一个将 Cregis 加密货币的支付网关整合到您的 WooCommerce 商店的插件。此整合可以让您的客户使用加密货币（包括 USDT、USDC、BTC、SOL、ETH、TRX 和 BNB）支付产品费用。

安装和配置完成后，插件会自动处理加密货币收款，将其转换为您偏好的结算货币，实时管理订单状态，并为您的客户提供无缝的结帐体验。该插件还包括处理加密货币支付场景常见的问题，例如超额支付和部分付款。

无需编写代码 – 只需安装插件，输入您的 Cregis 帐号信息，您的商店即可接受加密货币支付。



## 启用要求



设置 Cregis Payment 之前，请确保您已准备好以下项目：

* 运行 5.0 或更高版本的 WordPress 网站，并已安装和启用 WooCommerce 插件（3.0 或更高版本）。
* 您应该在 WooCommerce 商店中至少创建了一个产品。
* 您的网站已安装 SSL 证书以启用 HTTPS，这是加密货币交易必需的安全要求。
* Cregis 商户帐号，您可以按照下一部分的商家设置指南创建。



## 商家设置指南



1. 从[新手入门](https://support.cregis.com/cregis-wallet-guide/zh-cn/gettingstarted/download)下载 Cregis 客户端并创建您的商户帐号。成功创建后，请按照[创建支付引擎](https://support.cregis.com/cregis-wallet-guide/zh-cn/payment_engine/creation)部分提供的每一步指南完成完整的帐号设置。这包括结算钱包配置、API 生成以及选择您接收的加密货币币种。<br>
2.  一个关键步骤是将您的电商平台的伺服器 IP 地址添加到 Cregis 入口网站的 IP 白名单中。然后在 Cregis 客户端导航到 设置 > IP白名单，添加您的伺服器 IP 地址，并保存更改。如果没有正确的 IP 白名单设置，来自您商店的 API 请求将被拒绝。

    <figure><img src="../.gitbook/assets/image (1054).png" alt=""><figcaption></figcaption></figure>



## 安装和配置插件



1.  登录您的 WordPress 管理后台，导航到 Plugins > Add New。搜索「Cregis Payment for WooCommerce」并查找由 cregisproduct 创建的插件。点击 Install Now，然后点击 Activate 完成安装。

    <figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>



2.  安装后，您将在左侧菜单中看到 Cregis Payment。点击 Cregis Payment > Settings 访问配置页面。您需要从 Cregis 客户端复制 3 个信息：Base URL、Project ID 和 API Key。这些都可以在 Cregis 客户端的设置中找到。在插件 Settings 中贴上这些值，然后点击 Save Changes。

    <figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../.gitbook/assets/image (1055).png" alt=""><figcaption></figcaption></figure>



3. 设置所需信息后，您的电商平台上销售的产品将可自动接受加密货币支付。<br>
   1.  订单金额基于您的 WooCommerce 商店货币设置，您可以在 WooCommerce > Settings > Currency options > Currency 找到。（请确保您的货币是我们支持的货币，您可以在[此處](https://developers.cregis.com/zh/payment-engine-supported-currencies/)查阅）

       <figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>


   2.  产品价格是每个产品单独设置，置于 Products > All Products > \[选择产品] > Sale price。

       <figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>


   3. 如果您的商店货币是 USD 且列出的货币是与 USD 挂钩的稳定币，汇率将为 1:1。否则，您的产品标价与付款人选择的加密货币汇率将基于 CoinMarketCap 的实时汇率。<br>
   4. 付款人的电邮会在结帐时自动提交，并将用于处理超额支付和少额支付的情况。<br>
   5.  付款人可用的支付货币取决于您在 Cregis 客户端配置了哪些加密货币。

       <figure><img src="../.gitbook/assets/image (1056).png" alt=""><figcaption></figcaption></figure>


   6.  在 Web3 支付中，经常会遇到超额支付或部分支付的情况。您可以在插件设置中使用百分比配置容忍差，以控制您接受的上限和下限。例如，如果您在 100 美元的订单上设置 2% 的少额支付容差和 5% 的超额支付容差，您将接受 98 美元到 105 美元之间的支付。

       <figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>


   7.  每个支付默认有 60 分钟的有效时间。您可以根据需要调整此设置，最短为 10 分钟，最长为 1440 分钟（24 小时）。&#x20;

       <figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>



## 结帐流程与库存影响



1.  在您电商平台的结帐页面中，支付选项中将提供一个名为「Cregis Payment」的选项。付款人可以选择此选项并点击 Place Order。请注意，如果在库存中配置了产品数量（Products > All Products > 选择一个产品 > Product data section > Inventory > Quantity），当付款人点击「Place Order」按钮时，它将根据购物车中的数量自动扣除。

    <figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>



2. 支付链结是支付的行业标准界面。付款人可以选择他们偏好的加密货币，并按照介面完成支付。有关结帐的详细流程，可参考[支付链结（收银台）](https://support.cregis.com/cregis-wallet-guide/zh-cn/payment_engine/checkout_page?fallback=true)部分。\
   ![](<../.gitbook/assets/image (1057).png>)<br>
3. 在支付链结完成支付后，将重定向到您的订单状态页面。请注意，根据不同的支付状态，订单状态也会有所不同，可参下下表。

<table><thead><tr><th width="153.4140625">支付状态</th><th width="130.03125">订单状态</th><th>后续操作</th></tr></thead><tbody><tr><td>全额支付</td><td>已完成</td><td>无需操作。</td></tr><tr><td>部分支付</td><td>待处理</td><td>付款人将在订单状态页面看到跳窗，并收到电邮通知，需在 7 天内完成补款。更多信息：<a href="https://support.cregis.com/cregis-wallet-guide/zh-cn/payment_engine/introduction#bu-kuan-liu-cheng">补款流程</a>。</td></tr><tr><td>超额支付</td><td>待处理</td><td>付款人将在订单状态页面看到跳窗，并收到电邮通知，需在 7 天内完成部分退款。更多信息：<a href="https://support.cregis.com/cregis-wallet-guide/zh-cn/payment_engine/introduction#bu-fen-tui-kuan-liu-cheng">部分退款流程</a>。</td></tr><tr><td>支付超时</td><td>已取消</td><td>无需操作。</td></tr></tbody></table>

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>



4. 如果付款人完成全额退款或付款人未在有效时间内完成支付，库存将自动补货。
