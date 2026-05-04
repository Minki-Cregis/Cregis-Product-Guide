# 创建支付引擎

1.  从选单点击「支付引擎」

    <figure><img src="../.gitbook/assets/image (663).png" alt=""><figcaption></figcaption></figure>



2.  点击后，先填写「项目名称」及「行业」相关资讯

    <figure><img src="../.gitbook/assets/image (664).png" alt=""><figcaption></figcaption></figure>



3.  然后设定商户资讯，包括用于收银台显示的商户名称及品牌

    <figure><img src="../.gitbook/assets/image (666).png" alt=""><figcaption></figcaption></figure>



4.  选择支付引擎的支付币种及在工具提示(?)会提示该链所支援的最低支付数量

    <figure><img src="../.gitbook/assets/image (667).png" alt=""><figcaption></figcaption></figure>



5.  设定结算的币种，结算币种需按照支付币种独立进行配置。（如没有「钱包地址」配置，可在[此教学](https://support.cregis.com/cregis-wallet-guide/zh-cn/wallet_and_transaction/token_management)新增币种及地址）

    <figure><img src="../.gitbook/assets/image (668).png" alt=""><figcaption></figcaption></figure>



6.  如未配置也可以点击「继续」，稍后再配置，但会有视窗弹出提醒。若支付币种未完成结算配置，将会停留在「已支付」状态，直到结算配置完成，系统才会自动发起结算。（后续修改配置可参考[此手册分页](https://support.cregis.com/cregis-wallet-guide/zh-cn/payment_engine/configuration)）

    <figure><img src="../.gitbook/assets/image (669).png" alt=""><figcaption></figcaption></figure>



7.  完成配置后，验证交易密码。

    <figure><img src="../.gitbook/assets/image (670).png" alt=""><figcaption></figcaption></figure>



8.  然后验证谷歌验证码

    <figure><img src="../.gitbook/assets/image (671).png" alt=""><figcaption></figcaption></figure>



9.  完成后进入支付引擎页面，可以点选设定查看相关API存取资讯\
    <mark style="color:green;">注意：不要轻易将项目 API 金钥泄漏给他人，否则可能会导致资产损失。</mark>

    <figure><img src="../.gitbook/assets/image (672).png" alt=""><figcaption></figcaption></figure>



10. 在调用 API 前，请先在 IP 白名单添加调用 API 该设备的 IP 以确保安全，否则 API 将返回错误。设定可在「IP白名单」中，点击「建立群组」，输入 IP 位址并点击「储存」，然后进行身份验证即可。

    <figure><img src="../.gitbook/assets/image (673).png" alt=""><figcaption></figcaption></figure>



11. 完成配置后，支付引擎即可使用，技术文档请参考[此开发文件](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-engine-create)。<br>





