# 修改支付引擎配置

## 支付币种及结算配置



### 添加支付币种



1.  用户可于客户端修改支付及结算币种。

    <figure><img src="../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>



2.  点击「添加支付币种」，使用者可选择新的支付币种及设定结算币种，系统会显示相应的交易手续费率。最后选择结算用的钱包及地址。

    <figure><img src="../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>



3.  进行身份验证

    <figure><img src="../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>



4.  验证成功后，币种会添加到列表。

    <figure><img src="../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>



### 批量修改结算设定



1.  当支付引擎持有至少一种支付币种后，用户可于「批量修改结算设定」批量修改结算钱包及地址。

    <figure><img src="../.gitbook/assets/image (69).png" alt=""><figcaption></figcaption></figure>



2.  点击后即可按各种币种，修改结算钱包及地址，完成后点击确认，验证后即可。

    <figure><img src="../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>



## 订单处理配置（仅 API V1 用户）



建议：升级至[支付引擎最新的 API V2 版](https://developer-cn.cregis.com/api-reference/request-apis/payment/payment-engine-create)，于 API 进行「超额支付」及「部分支付」逻辑。



1.  如接受所有的「超额支付」或「部分支付」，可在客户端于「超额支付订单」及「部分支付订单」选择「接受」。

    <figure><img src="../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure>



2.  如对「超额支付」或「部分支付」设定上下限，可在客户端于「支付准确度设置」选择「新增订单币种」，然后对「订单币种」设定相对的「超额支付」或「部分支付」的容忍上下限。 （如付款人使用其他「支付币种」，系统会实时进行汇率换算）

    <figure><img src="../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure>



## 商户资讯配置



1.  对于收银台显示的商户资讯（如名称，Logo等），可在「设置」的「商户信息」栏进行修改。

    <figure><img src="../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>



## 通知设定



1.  用户可自行设置项目的通知，选项包括以下。如有需要，点击开启即可。

    1. 异常回调：系统自动回调失败时
    2. 启用／禁用项目：当系统启用或禁用项目时
    3.  重置API Key：重置项目API Key时

        <figure><img src="../.gitbook/assets/image (532).png" alt=""><figcaption></figcaption></figure>


2.  如需通知多人，可在「编辑」选择相关的团队成员。

    <figure><img src="../.gitbook/assets/image (531).png" alt=""><figcaption></figcaption></figure>







