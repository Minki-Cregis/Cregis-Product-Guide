---
description: 本章说明 Cregis 客户端在 WaaS 订单模式下的各类记录页面。除另有说明外，每个记录页面均支援相同的核心操作。
---

# 核心记录

1. 订单记录 - 当「创建订单」API 回传有效数据时，即会建立一笔记录。<br>
   1.  订单记录：如需查看订单记录，请在 WaaS 订单模式下点击「订单记录」。

       <figure><img src="../../.gitbook/assets/image (1326).png" alt=""><figcaption></figcaption></figure>


   2.  查看详情：您可以点击该笔记录查看订单详情包括订单资讯及相关的付款、退款与转账资讯。

       <figure><img src="../../.gitbook/assets/image (1327).png" alt=""><figcaption></figcaption></figure>


   3.  筛选：使用右上角的「筛选」图示筛选订单记录（例如按状态、币种或创建时间）。

       <figure><img src="../../.gitbook/assets/image (1328).png" alt=""><figcaption></figcaption></figure>


   4.  时区：点击表头显示的时区，即可切换显示时区。

       <figure><img src="../../.gitbook/assets/image (1329).png" alt=""><figcaption></figcaption></figure>


   5.  导出：使用右上角的「导出」图示导出订单记录。导出结果按步骤 3 所设的条件筛选，时区则跟随步骤 4。

       <figure><img src="../../.gitbook/assets/image (1330).png" alt=""><figcaption></figcaption></figure>


   6.  汇总：当筛选条件为特定币种时，右下角会显示部分支付、已完成支付及已转账金额的总数。

       <figure><img src="../../.gitbook/assets/image (1331).png" alt=""><figcaption></figcaption></figure>


2. 批量转账单记录 - 当订单满足转账规则时（第一页第五部分），即会建立一笔记录。<br>
   1.  批量转账单记录：如需查看批量转账单记录，请在 WaaS 订单模式下点击「批量转账单记录」。

       <figure><img src="../../.gitbook/assets/image (1332).png" alt=""><figcaption></figcaption></figure>


   2.  查看详情：点击记录查看批量转账单详情，同时可查看每条转账单记录。转账单是其同一收款地址的订单归为一组。

       <figure><img src="../../.gitbook/assets/image (1333).png" alt=""><figcaption></figcaption></figure>


   3.  筛选：使用右上角的「筛选」图示筛选批量转账单记录（例如按状态、币种或创建时间）。

       <figure><img src="../../.gitbook/assets/image (1334).png" alt=""><figcaption></figcaption></figure>


   4.  时区：点击表头显示的时区，即可切换显示时区。

       <figure><img src="../../.gitbook/assets/image (1335).png" alt=""><figcaption></figcaption></figure>


   5.  导出：使用右上角的「导出」图示导出批量转账单记录。导出结果按步骤 3 所设的条件筛选，时区则跟随步骤 4。

       <figure><img src="../../.gitbook/assets/image (1336).png" alt=""><figcaption></figcaption></figure>


   6.  汇总：当筛选条件为特定币种时，右下角会显示转账失败、转账中及已转账金额的总数。

       <figure><img src="../../.gitbook/assets/image (1337).png" alt=""><figcaption></figcaption></figure>


3. 异常支付单记录 - 当在付款触发 AML 规则时或付款已完成但无法匹配任何订单收款逻辑时建立。<br>
   1.  异常支付单记录：如需查看异常支付单记录，请在 WaaS 订单模式下点击「异常支付单记录」。

       <figure><img src="../../.gitbook/assets/image (1338).png" alt=""><figcaption></figcaption></figure>


   2.  查看详情：点击记录查看异常支付单详情，包括收款地址、链上时间、原因等资讯。

       <figure><img src="../../.gitbook/assets/image (1339).png" alt=""><figcaption></figcaption></figure>


   3.  筛选：使用右上角的「筛选」图示筛选异常支付单记录（例如按交易哈希、币种或创建时间）。

       <figure><img src="../../.gitbook/assets/image (1340).png" alt=""><figcaption></figcaption></figure>


   4.  时区：点击表头显示的时区，即可切换显示时区。

       <figure><img src="../../.gitbook/assets/image (1341).png" alt=""><figcaption></figcaption></figure>


   5.  导出：使用右上角的「导出」图示导出异常支付单记录。导出结果按步骤 3 所设的条件筛选，时区则跟随步骤 4。

       <figure><img src="../../.gitbook/assets/image (1342).png" alt=""><figcaption></figcaption></figure>


   6.  汇总：当筛选条件为特定币种时，右下角会显示异常支付单、已转账及转账手续费的总数。

       <figure><img src="../../.gitbook/assets/image (1343).png" alt=""><figcaption></figcaption></figure>


   7.  自行转账：商户可在 Cregis 客户端自行转账异常支付。点击「转账」按钮即可发起；仅限同链同币。

       <figure><img src="../../.gitbook/assets/image (1344).png" alt=""><figcaption></figcaption></figure>


   8.  收款地址及备注：商户可手动输入转账的收款地址，并为该笔转账设定备注。

       <figure><img src="../../.gitbook/assets/image (1345).png" alt=""><figcaption></figcaption></figure>


   9.  服务费率：如 Cregis 团队已为您的项目设定费率，所有币种均采用相同费率；否则预设费率为 1%。\
       最低服务费：如待转账的币种与您已设定的转账币种一致，最低费用将与「设定」→「收款及转账」页面所示的标准收费相同。如 Cregis 团队已为您的帐户减免最低服务费，此处亦不收取最低费用。否则，最低费用按下表币种而定；未列入表中的币种，按等值 1 USD 收取（以 CoinMarketCap 即时汇率换算）。

       <figure><img src="../../.gitbook/assets/image (1346).png" alt=""><figcaption></figcaption></figure>



| 币种                                                                                                   | 最低交易手续费     |
| ---------------------------------------------------------------------------------------------------- | ----------- |
| USDT-TRC20, USDT-ERC20                                                                               | 1 USDT      |
| USDT-BEP20, USDT-Solana, USDT-Polygon, USDT-Avalanche-C, USDT-Arbitrum One                           | 0.5 USDT    |
| USDC-ERC20                                                                                           | 1 USDC      |
| USDC-Base, USDC-BEP20, USDC-Solana, USDC-Polygon, USDC-Avalanche-C, USDC-Arbitrum One, USDC-Optimism | 0.5 USDC    |
| TRON                                                                                                 | 1 TRX       |
| Solana                                                                                               | 0.0002 SOL  |
| BNB-BSC                                                                                              | 0.0002 BNB  |
| Ethereum, Base, Arbitrum One, Optimism                                                               | 0.0002 ETH  |
| Bitcoin                                                                                              | 0.00001 BTC |

请注意：<br>

* 仅异常支付单与 AML 不相符时才可在客户端进行转账。如与 AML 有关，请联络 Cregis 支援团队。<br>
* 如交易手续费大于或等于异常支付单金额，将不允许转账。



4. 退款记录 - 当已收的款项不符合所提交订单要求时建立<br>
   1.  退款单记录：如需查看退款单记录，请在 WaaS 订单模式下点击「退款单记录」。

       <figure><img src="../../.gitbook/assets/image (1347).png" alt=""><figcaption></figcaption></figure>


   2.  查看详情：点击记录查看退款单详情，包括退款类型、原因等资讯。

       <figure><img src="../../.gitbook/assets/image (1348).png" alt=""><figcaption></figcaption></figure>


   3.  筛选：使用右上角的「筛选」图示筛选退款单记录（例如按订单号、退款原因或退款类型）。

       <figure><img src="../../.gitbook/assets/image (1349).png" alt=""><figcaption></figcaption></figure>


   4.  时区：点击表头显示的时区，即可切换显示时区。

       <figure><img src="../../.gitbook/assets/image (1350).png" alt=""><figcaption></figcaption></figure>


   5.  导出：使用右上角的「导出」图示导出退款单记录。导出结果按步骤 3 所设的条件筛选，时区则跟随步骤 4。

       <figure><img src="../../.gitbook/assets/image (1351).png" alt=""><figcaption></figcaption></figure>


   6.  汇总：当筛选条件为特定币种时，右下角会显示退款单、已退款及退款手续费的总数。

       <figure><img src="../../.gitbook/assets/image (1352).png" alt=""><figcaption></figcaption></figure>


   7.  自行退款：商户可在 Cregis 客户端自行退款。点击「退款」按钮即可发起；仅限同链同币。

       <figure><img src="../../.gitbook/assets/image (1353).png" alt=""><figcaption></figcaption></figure>


   8.  收款地址及备注：商户可手动输入退款的收款地址，并为该笔退款设定备注。

       <figure><img src="../../.gitbook/assets/image (1354).png" alt=""><figcaption></figcaption></figure>


   9.  退款固定手续费：仅收取固定费用，按下表币种而定：

       <figure><img src="../../.gitbook/assets/image (1355).png" alt=""><figcaption></figcaption></figure>



| 币种                                                                                                   | 退款固定手续费     |
| ---------------------------------------------------------------------------------------------------- | ----------- |
| USDT-TRC20, USDT-ERC20                                                                               | 1 USDT      |
| USDT-BEP20, USDT-Solana, USDT-Polygon, USDT-Avalanche-C, USDT-Arbitrum One                           | 0.5 USDT    |
| USDC-ERC20                                                                                           | 1 USDC      |
| USDC-Base, USDC-BEP20, USDC-Solana, USDC-Polygon, USDC-Avalanche-C, USDC-Arbitrum One, USDC-Optimism | 0.5 USDC    |
| TRON                                                                                                 | 1 TRX       |
| Solana                                                                                               | 0.0002 SOL  |
| BNB-BSC                                                                                              | 0.0002 BNB  |
| Ethereum, Base, Arbitrum One, Optimism                                                               | 0.0002 ETH  |
| Bitcoin                                                                                              | 0.00001 BTC |

请注意：



* 如退款手续费大于或等于退款金额，将不允许退款。



5. 异常回调 - 当回调未能送达至回调网址<br>
   1.  异常回调记录：如需查看异常回调记录，请在 WaaS 订单模式下点击「异常回调」。

       <figure><img src="../../.gitbook/assets/image (1356).png" alt=""><figcaption></figcaption></figure>


   2.  查看详情：点击记录查看回调详情、支付信息及钱包提币等资讯。

       <figure><img src="../../.gitbook/assets/image (1357).png" alt=""><figcaption></figcaption></figure>


   3.  筛选：使用右上角的「筛选」图示筛选异常回调记录（例如按回调网址、回调时间等）。

       <figure><img src="../../.gitbook/assets/image (1358).png" alt=""><figcaption></figcaption></figure>


   4.  时区：点击表头显示的时区，即可切换显示时区。

       <figure><img src="../../.gitbook/assets/image (1359).png" alt=""><figcaption></figcaption></figure>


   5.  重试或忽略：商户可对单笔回调执行重试或忽略；亦可在左侧点选对多笔回调执行批量重试或批量忽略。

       <figure><img src="../../.gitbook/assets/image (1360).png" alt=""><figcaption></figcaption></figure>


   6.  以新回调网址重试：如商户想更改某一笔回调网址，可点击该记录上的「重试」，再输入。

       <figure><img src="../../.gitbook/assets/image (1361).png" alt=""><figcaption></figcaption></figure>


6. 历史回调 - 当回调已成功送达至回调网址<br>
   1.  历史回调记录：如需查看历史回调记录，请在 WaaS 订单模式下点击「历史回调」。

       <figure><img src="../../.gitbook/assets/image (1362).png" alt=""><figcaption></figcaption></figure>


   2.  查看详情：点击记录查看回调详情、支付信息及钱包提币等资讯。

       <figure><img src="../../.gitbook/assets/image (1366).png" alt=""><figcaption></figcaption></figure>


   3.  筛选：使用右上角的「筛选」图示筛选历史回调记录（例如按回调网址、回调时间等）。

       <figure><img src="../../.gitbook/assets/image (1364).png" alt=""><figcaption></figcaption></figure>


   4.  时区：点击表头显示的时区，即可切换显示时区。

       <figure><img src="../../.gitbook/assets/image (1365).png" alt=""><figcaption></figcaption></figure>







