# 查询订单相关记录

## 订单记录



1.  如需查阅订单记录，可在支付引擎内的「支付记录」查阅。

    <figure><img src="../.gitbook/assets/image (519).png" alt=""><figcaption></figcaption></figure>



2.  点击记录可查看订单详情

    <figure><img src="../.gitbook/assets/image (523).png" alt=""><figcaption></figcaption></figure>



3.  右上方的图标可导出订单记录

    <figure><img src="../.gitbook/assets/image (524).png" alt=""><figcaption></figcaption></figure>



## 结算记录



1.  如需查阅结算记录，可在支付引擎内的「结算记录」查阅。

    <figure><img src="../.gitbook/assets/image (520).png" alt=""><figcaption></figcaption></figure>



2.  点击记录可查看结算详情

    <figure><img src="../.gitbook/assets/image (153).png" alt=""><figcaption></figcaption></figure>



3.  右上方的图标可导出结算记录

    <figure><img src="../.gitbook/assets/image (154).png" alt=""><figcaption></figcaption></figure>



## 异常支付单记录



1.  如支付在订单逻辑以外，异常支付单可在支付引擎内的「异常支付单记录」查阅。

    <figure><img src="../.gitbook/assets/image (1044).png" alt=""><figcaption></figcaption></figure>



2.  点击记录可查看异常支付详情

    <figure><img src="../.gitbook/assets/image (1045).png" alt=""><figcaption></figcaption></figure>



3.  右上方的图标可导出结算记录

    <figure><img src="../.gitbook/assets/image (1046).png" alt=""><figcaption></figcaption></figure>



4.  商户可透过 Cregis 客户端，点击「转账」按钮，自行转账支付异常支付单款项。

    <figure><img src="../.gitbook/assets/image (1047).png" alt=""><figcaption></figcaption></figure>



5.  转账币种选择： 您可以选择已配置的结算货币（设置 → 支付币种及结算）或同一链上的相同币种。

    <figure><img src="../.gitbook/assets/image (1048).png" alt=""><figcaption></figcaption></figure>



6.  接收方： 若转账币种为已配置的结算币种，接收方将自动使用您配置的结算地址。对于其他币种，可手动输入接收方。

    <figure><img src="../.gitbook/assets/image (1049).png" alt=""><figcaption></figcaption></figure>



7.  备注： 您可添加有关转账的备注信息。这备注会被保存，并可在异常支付单详情页面（如步骤 2 所示）查看。

    <figure><img src="../.gitbook/assets/image (1050).png" alt=""><figcaption></figcaption></figure>



8.  手续费率： 若 Cregis 团队已为您的项目分配费率，该费率将适用于所有货币；否则，默认费率为 1%。\
    \
    最低收单手续费： 若转账币种与您配置的结算币种相同，最低费用将反映于「设置 → 支付币种及结算」中的结算币种内。若 Cregis 团队已为您的免除最低收单手续费，此处亦将免除。否则，最低收单手续费将根据下表。对于未列出的币种，将使用 1 美元等值（通过 CoinMarketCap 实时汇率计算）。<br>

    <figure><img src="../.gitbook/assets/image (1051).png" alt=""><figcaption></figcaption></figure>



<table data-search="false"><thead><tr><th width="496.5">币种</th><th>最低收单手续费</th></tr></thead><tbody><tr><td>USDT-TRC20, USDT-ERC20</td><td>1 USDT</td></tr><tr><td>USDT-BEP20, USDT-Solana, USDT-Polygon, USDT-Avalance-C, USDT- Arbitrum One</td><td>0.5 USDT</td></tr><tr><td>USDC-ERC20</td><td>1 USDC</td></tr><tr><td>USDC-Base, USDC-BEP20, USDC-Solana, USDC-Polygon, USDC-Avalance-C, USDC-Arbitrum One, USDC-Optimism</td><td>0.5 USDC</td></tr><tr><td>TRON</td><td>1 TRX</td></tr><tr><td>Solana</td><td>0.0002 SOL</td></tr><tr><td>BNB-BSC</td><td>0.0002 BNB</td></tr><tr><td>Ethereum, Base, Arbitrum One, Optimism</td><td>0.0002 ETH</td></tr><tr><td>Bitcoin</td><td>0.00001 BTC</td></tr></tbody></table>

请注意：

* 转账仅适用于非 AML 的异常支付单。若涉及 AML，请联系 Cregis 团队。
* 若手续费大于或等于异常支付单金额，将不允许转账。
* 您可以在转账前，将转账币种配置为结算币种，以使用您标准的最低收单手续费和费率。



