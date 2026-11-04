---
description: >-
  This chapter explains the record pages available under WaaS Order Mode in the
  Cregis portal. Unless stated otherwise, every record page supports the same
  core actions.
---

# Core Records

1. Order Records - A record is created when the Create Order API responds with valid data.<br>
   1.  Order Records: To view order view, you can click Order Records under WaaS Order Mode.

       <figure><img src="../../../.gitbook/assets/image (1249).png" alt=""><figcaption></figcaption></figure>


   2.  Order Details: you can click on the record to view the order details, including the order information as well as the related payment, refund, and transfer information.

       <figure><img src="../../../.gitbook/assets/image (1250).png" alt=""><figcaption></figcaption></figure>


   3.  Filtering: you use the Filter icon in the upper-right corner to filter the order records (for example, by status, currency or creation time).

       <figure><img src="../../../.gitbook/assets/image (1251).png" alt=""><figcaption></figcaption></figure>


   4.  Timezone: click the timezone shown in the table header to switch the display timezone.

       <figure><img src="../../../.gitbook/assets/image (1252).png" alt=""><figcaption></figcaption></figure>


   5.  Export: use the Export icon in the upper-right corner to export the order records. The exported results are filtered by the conditions set in step 3 and the timezone follows the selection made in step 4.

       <figure><img src="../../../.gitbook/assets/image (1253).png" alt=""><figcaption></figcaption></figure>


   6.  Summary: when the filter is set to a specific currency, the summary at the bottom right shows the totals of partial payments, completed payments and transferred amounts.

       <figure><img src="../../../.gitbook/assets/image (1254).png" alt=""><figcaption></figcaption></figure>


2. Bulk Transfer Records - A record is created when the order(s) meet the transfer rules (see Section 1.5).<br>
   1.  Bulk Transfer Records: To view bulk transfer records, you can click Bulk Transfer Records under WaaS Order Mode.

       <figure><img src="../../../.gitbook/assets/image (1264).png" alt=""><figcaption></figcaption></figure>


   2.  Bulk Transfer Details: you can click on the record to view the bulk transfer details including each transfer record which groups the orders that share the same receiving address.

       <figure><img src="../../../.gitbook/assets/image (1265).png" alt=""><figcaption></figcaption></figure>


   3.  Filtering: you use the Filter icon in the upper-right corner to filter the bulk transfer records (for example, by status, currency or creation time).

       <figure><img src="../../../.gitbook/assets/image (1266).png" alt=""><figcaption></figcaption></figure>


   4.  Timezone: click the timezone shown in the table header to switch the display timezone.

       <figure><img src="../../../.gitbook/assets/image (1267).png" alt=""><figcaption></figcaption></figure>


   5.  Export: use the Export icon in the upper-right corner to export the bulk transfer records. The exported results are filtered by the conditions set in step 3 and the timezone follows the selection made in step 4.

       <figure><img src="../../../.gitbook/assets/image (1268).png" alt=""><figcaption></figcaption></figure>


   6.  Summary: when the filter is set to a specific currency, the summary at the bottom right shows the totals of transfer failed, transferring and transferred amounts.

       <figure><img src="../../../.gitbook/assets/image (1269).png" alt=""><figcaption></figcaption></figure>


3. Payment Exception Records - A record is created when a payment hits an AML rule or when a payment has been made but cannot be matched to any order receiving logic.<br>
   1.  Payment Exception Records: To view payment exception records, you can click Payment Exception Records under WaaS Order Mode.

       <figure><img src="../../../.gitbook/assets/image (1255).png" alt=""><figcaption></figcaption></figure>


   2.  Payment Exception Details: you can click on the record to view the payment exception details including received address, block time, reason, etc

       <figure><img src="../../../.gitbook/assets/image (1256).png" alt=""><figcaption></figcaption></figure>


   3.  Filtering: you use the Filter icon in the upper-right corner to filter the payment exception records (for example, by transaction hash, currency or creation time).

       <figure><img src="../../../.gitbook/assets/image (1257).png" alt=""><figcaption></figcaption></figure>


   4.  Timezone: click the timezone shown in the table header to switch the display timezone.

       <figure><img src="../../../.gitbook/assets/image (1258).png" alt=""><figcaption></figcaption></figure>


   5.  Export: use the Export icon in the upper-right corner to export the payment exception records. The exported results are filtered by the conditions set in step 3 and the timezone follows the selection made in step 4.

       <figure><img src="../../../.gitbook/assets/image (1259).png" alt=""><figcaption></figcaption></figure>


   6.  Summary: when the filter is set to a specific currency, the summary at the bottom right shows the total payment exception amount, transferred amount and transfer fee.

       <figure><img src="../../../.gitbook/assets/image (1260).png" alt=""><figcaption></figcaption></figure>


   7.  Self-transfer: merchants may transfer a payment exception themselves in the Cregis portal. Click the Transfer button to initiate it. Only the same token on the same chain can be transferred.

       <figure><img src="../../../.gitbook/assets/image (1261).png" alt=""><figcaption></figcaption></figure>


   8.  Receiving address and remark: merchants can manually enter the receiving address for the transfer and create a remark for it.

       <figure><img src="../../../.gitbook/assets/image (1262).png" alt=""><figcaption></figcaption></figure>


   9.  Service fee rate: if the Cregis team has assigned a fee rate to your project, the same rate applies across all currencies; otherwise, the default rate is 1%.\
       Minimum service fee: if the token to be transferred matches your configured transfer currency, the minimum fee mirrors the standard rate shown on the Receiving and Transfer page under Settings. If the Cregis team has waived the minimum service fee for your account, no minimum fee applies here either. Otherwise, the minimum fee follows the currency table below. For currencies not listed, a 1 USD equivalent (calculated at the real-time CoinMarketCap rate) applies.

       <figure><img src="../../../.gitbook/assets/image (1263).png" alt=""><figcaption></figcaption></figure>



| Token                                                                                                | Minimum Transaction Fee |
| ---------------------------------------------------------------------------------------------------- | ----------------------- |
| USDT-TRC20, USDT-ERC20                                                                               | 1 USDT                  |
| USDT-BEP20, USDT-Solana, USDT-Polygon, USDT-Avalanche-C, USDT-Arbitrum One                           | 0.5 USDT                |
| USDC-ERC20                                                                                           | 1 USDC                  |
| USDC-Base, USDC-BEP20, USDC-Solana, USDC-Polygon, USDC-Avalanche-C, USDC-Arbitrum One, USDC-Optimism | 0.5 USDC                |
| TRON                                                                                                 | 1 TRX                   |
| Solana                                                                                               | 0.0002 SOL              |
| BNB-BSC                                                                                              | 0.0002 BNB              |
| Ethereum, Base, Arbitrum One, Optimism                                                               | 0.0002 ETH              |
| Bitcoin                                                                                              | 0.00001 BTC             |

Please note that:<br>

* Transfer is only applicable if the payment exception is not AML-related. For AML-related exceptions, please contact the Cregis support team.<br>
* If the transaction fee is greater than or equal to the payment exception amount, the transfer will not be allowed.



4. Refund Records - A record is created when the received payment(s) do not fulfill the requirements of the submitted order<br>
   1.  Refund Records: To view refund records, you can click Refund Records under WaaS Order Mode.

       <figure><img src="../../../.gitbook/assets/image (1270).png" alt=""><figcaption></figcaption></figure>


   2.  Record Details: you can click on the record to view the record details including refund type, reason, etc

       <figure><img src="../../../.gitbook/assets/image (1271).png" alt=""><figcaption></figcaption></figure>


   3.  Filtering: you use the Filter icon in the upper-right corner to filter the refund records (for example, by order id, refund reason or refund type).

       <figure><img src="../../../.gitbook/assets/image (1272).png" alt=""><figcaption></figcaption></figure>


   4.  Timezone: click the timezone shown in the table header to switch the display timezone.

       <figure><img src="../../../.gitbook/assets/image (1273).png" alt=""><figcaption></figcaption></figure>


   5.  Export: use the Export icon in the upper-right corner to export the refund records. The exported results are filtered by the conditions set in step 3 and the timezone follows the selection made in step 4.

       <figure><img src="../../../.gitbook/assets/image (1274).png" alt=""><figcaption></figcaption></figure>


   6.  Summary: when the filter is set to a specific currency, the summary at the bottom right shows the total refund amount, refunded amount and refund fee.

       <figure><img src="../../../.gitbook/assets/image (1275).png" alt=""><figcaption></figcaption></figure>


   7.  Self-refund: merchants may proceed with a refund themselves in the Cregis portal. Click the Refund button to initiate it. Only the same token on the same chain can be refunded.

       <figure><img src="../../../.gitbook/assets/image (1276).png" alt=""><figcaption></figcaption></figure>


   8.  Receiving address and remark: merchants can manually enter the receiving address for the refund and create a remark for it.

       <figure><img src="../../../.gitbook/assets/image (1277).png" alt=""><figcaption></figcaption></figure>


   9.  Refund fixed fee: only a fixed fee applies based on the table below:

       <figure><img src="../../../.gitbook/assets/image (1278).png" alt=""><figcaption></figcaption></figure>



| Token                                                                                                | Refund Fixed Fee |
| ---------------------------------------------------------------------------------------------------- | ---------------- |
| USDT-TRC20, USDT-ERC20                                                                               | 1 USDT           |
| USDT-BEP20, USDT-Solana, USDT-Polygon, USDT-Avalanche-C, USDT-Arbitrum One                           | 0.5 USDT         |
| USDC-ERC20                                                                                           | 1 USDC           |
| USDC-Base, USDC-BEP20, USDC-Solana, USDC-Polygon, USDC-Avalanche-C, USDC-Arbitrum One, USDC-Optimism | 0.5 USDC         |
| TRON                                                                                                 | 1 TRX            |
| Solana                                                                                               | 0.0002 SOL       |
| BNB-BSC                                                                                              | 0.0002 BNB       |
| Ethereum, Base, Arbitrum One, Optimism                                                               | 0.0002 ETH       |
| Bitcoin                                                                                              | 0.00001 BTC      |

Please note that:



* If the refund fee is greater than or equal to the refund amount, the refund will not be allowed.



5. Callback Error - A record is created when the callbacks that could not be delivered to your callback URL<br>
   1.  Callback Error Records: To view callback error, you can click Callback Error under WaaS Order Mode.

       <figure><img src="../../../.gitbook/assets/image (1279).png" alt=""><figcaption></figcaption></figure>


   2.  Record Details: you can click on the record to view the callback, payment and wallet payout related information.

       <figure><img src="../../../.gitbook/assets/image (1280).png" alt=""><figcaption></figcaption></figure>


   3.  Filtering: you use the Filter icon in the upper-right corner to filter the callback error records (for example, by callback url, callback time, etc).

       <figure><img src="../../../.gitbook/assets/image (1281).png" alt=""><figcaption></figcaption></figure>


   4.  Timezone: click the timezone shown in the table header to switch the display timezone.

       <figure><img src="../../../.gitbook/assets/image (1282).png" alt=""><figcaption></figcaption></figure>


   5.  Retry or ignore: merchants may retry or ignore each callback. Bulk retry or ignore actions are also available for multiple selected callbacks on the left.

       <figure><img src="../../../.gitbook/assets/image (1283).png" alt=""><figcaption></figcaption></figure>


   6.  Retry with a new callback URL: if the merchant would like to change the callback URL for the retry of one particular record, click Retry on that record.

       <figure><img src="../../../.gitbook/assets/image (1284).png" alt=""><figcaption></figcaption></figure>


6. History Callback - A record is created when the callbacks are successfully delivered to your callback URL<br>
   1.  History Callback Records: To view history callback, you can click History Callback under WaaS Order Mode.

       <figure><img src="../../../.gitbook/assets/image (1285).png" alt=""><figcaption></figcaption></figure>


   2.  Record Details: you can click on the record to view the callback, payment and wallet payout related information.

       <figure><img src="../../../.gitbook/assets/image (1286).png" alt=""><figcaption></figcaption></figure>


   3.  Filtering: you use the Filter icon in the upper-right corner to filter the history callback records (for example, by callback url, callback time, etc).

       <figure><img src="../../../.gitbook/assets/image (1287).png" alt=""><figcaption></figcaption></figure>


   4.  Timezone: click the timezone shown in the table header to switch the display timezone.<br>

       <figure><img src="../../../.gitbook/assets/image (1288).png" alt=""><figcaption></figcaption></figure>









