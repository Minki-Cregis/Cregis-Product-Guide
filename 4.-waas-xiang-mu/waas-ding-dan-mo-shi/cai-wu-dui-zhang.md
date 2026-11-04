---
description: 每月财务对帐时，从「订单记录」或「批量转账记录」导出订单，即可快速取得所需的总额。
---

# 财务对账

To avoid any order status update towards Cancelled during the reconciliation, you could perform the reconciliation after the 7th day of each month because 7 days is the maximum additional payment pending time. After the 7th day, all the orders of the previous month will be in one of the terminal states: paid, transferred, cancelled or expired.



1.  Actual received amounts: if the merchant would like to check all the actual received amounts, filter the status by paid and transferred, and sum up the Actual Received Amount numbers. The actual received amount means all the amounts received from the payers, deducted by all the partial refund amounts. This is exactly what the payers sent to your sole use address. Please note that the amount unit is based on the received currency, so the merchant may need to separate the amounts by currency in order to obtain a correct sum.

    <figure><img src="../../.gitbook/assets/image (1310).png" alt=""><figcaption></figcaption></figure>


2.  Total service fees: if the merchant would like to find out all the service fees, look for the Service Fee column with the status of paid and transferred as well. This service fee unit is also based on the received currency, so the merchant may need to separate the amounts by currency in order to obtain a correct sum.

    <figure><img src="../../.gitbook/assets/image (1311).png" alt=""><figcaption></figcaption></figure>


3.  Understand how the service fee is deducted: the service fee deduction depends on the currency. If the payment currency is a stablecoin, the transfer amount will be exactly the same as the actual received amount. If it is a non-stablecoin, the transfer amount will be deducted by the service fee. The Deducted from column can help the merchant identify whether the transfer amount has been deducted by the service fee or not.

    <figure><img src="../../.gitbook/assets/image (1312).png" alt=""><figcaption></figcaption></figure>


4.  Transfer time and transaction hash: to find out the transfer time and the transaction hash, the merchant can map the Bulk Transfer ID from the order table to the Transfer table. Please note that one transfer can link up to multiple orders if they share the same receiving address.

    <figure><img src="../../.gitbook/assets/image (1313).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (1314).png" alt=""><figcaption></figcaption></figure>


5.  Payment information for each order: if the merchant would like to know the payment information for each order, map the Order ID from the order table to the Payment table.

    <figure><img src="../../.gitbook/assets/image (1315).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (1316).png" alt=""><figcaption></figcaption></figure>


6.  Cancelled orders that are processed to refund: to find out the cancelled orders that will proceed to refund, the merchant can map the Order ID from the order table to the Refund table. Please note that the refund amount is also based on the refund currency. The merchant can also check which refunds are not completed yet.

    <figure><img src="../../.gitbook/assets/image (1315).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (1317).png" alt=""><figcaption></figcaption></figure>

    \
    \
    \
    \
    \
    <br>
