---
description: >-
  This chapter explains what WaaS Order Mode is, the payment rules, the core
  records and the rules that govern transfers, additional payments, refunds and
  service fees.
hidden: true
---

# WaaS Order Mode

1. What is WaaS Order Mode?\
   \
   WaaS Order Mode is a payment receiving solution built on the Cregis self-custodial wallet. It inherits the core principle of self-custody, ensuring that all funds for each merchant are completely isolated. This solution enables merchants to receive crypto payments directly into their own self-custodial wallet without the need to manually handle address assignment. Merchants enjoy a simple and seamless receiving experience, and the API integration is kept as straightforward as possible.\
   \
   The product is designed for online businesses such as e-commerce platforms, SaaS, gaming, forex, digital content and similar merchants that want to accept crypto payments on a per order basis with minimal integration effort and receive the funds directly in their own wallet with real time payment notification.<br>
2. Payment Rules<br>
   1. **Supported cryptocurrencies**: Cregis accepts **23 cryptocurrencies** (including USDT, USDC, ETH, BTC, SOL, TRX and BNB).<br>
   2. **Enable the currencies you accept**: in the Receiving and Transfer settings, you enable the cryptocurrencies you want to accept and set up a receiving address for each of them.<br>
   3. **Order in fiat, receive in crypto**: instead of pricing your orders in crypto, you can set the order amount in a fiat currency (order currency). When a payer pays, Cregis converts the order amount into the payment currency at the real-time CoinMarketCap exchange rate.<br>
   4. **Instant notifications**: Upon payment receipt, Cregis notifies merchants in real time with the payment status. Merchants can then take appropriate action based on the status whether it’s an exact payment, partial payment, overpayment, timeout or cancelled.<br>
3. The Core Records\
   \
   WaaS Order Mode keeps six types of records across the payment lifecycle. Understanding these records helps you follow what happens to every order, and use the portal, API and callbacks correctly.<br>
   1. **Order Record**: created when you create an order. It stores all the information you submitted via API such as the order amount, order currency, payment tokens, valid time, payer information, etc.<br>
   2.  **Payment Record**: created when a payer's payment is matched to an order by the receiving logic. It links the order with the sender address, receiving address, transaction hash and other on-chain information.


   3.  **Refund Record**: initiated when the received payment(s) do not fulfill the requirements of the submitted order, so that you can refund the amount to the payer.


   4. **Bulk Transfer Record**: created when the order(s) meet the transfer rules. It records the time and orders the batch transfer of funds to your self-custodial address was initiated.<br>
   5. **Transfer Record**: created at the same time as a bulk transfer record. It groups the orders by the same payment receiving address and records the transfer information from the payment receiving address to your self-custodial wallet address.<br>
   6.  **Payment Exception Record**: created when a payment hits an AML rule or when a payment has been made but cannot be matched to any order receiving logic. It allows you to continue the transfer or refund the payment.


4. Record Statuses\
   \
   Each record moves through a defined status. The sections below list the status of orders, refunds and payment exceptions with their meanings.<br>
   1. Order Status<br>
      1. **New**: the order has been created but has not received any payment yet, and is still within its valid time.<br>
      2. **Additional Payment Required**: - a payment has been received but does not yet satisfy the order amount, so the payer is required to make an additional payment. If the order includes the payer's email, an additional payment email will be sent to the payer automatically. Otherwise, you are required to send the payment address from the callback to the payer to complete the additional payment. The additional payment amount can also be found in the callback or in a Query Order API request.<br>
      3. **Paid**: the payment has been received and is within the merchant's tolerance level, but the amount has not yet been transferred to your self-custodial wallet.<br>
      4. **Transferred**: the amount has been transferred to your address. This is the end of the order flow.<br>
      5. **Cancelled**: the order is required to be refunded or has hit an AML rule, so the order cannot continue. This is the end of the order flow. Depending on the situation, either a refund or a payment exception flow will be triggered.<br>
      6. **Expired**: the order has expired and no longer accepts payment. This is the end of the order flow.<br>
   2. Refund Status<br>
      1. **Pending**: the refund has been triggered.<br>
      2. **Refunding**: the refund has been initiated, and is being processed.<br>
      3. **Refund Successful**: the amount has been refunded to the destination address.<br>
      4. **Refund Failed**: the refund has failed and manual intervention is required. This is very unlikely.<br>
   3. Payment Exception Status<br>
      1. **Pending**: the payment exception has been triggered.<br>
      2. **Transferring**: the payment exception has been initiated, and is being processed.<br>
      3. **Transfer Successful**: the amount has been transferred to the destination address.<br>
      4.  **Transfer Failed**: the transfer has failed and manual intervention is required. This is very unlikely.


5. Transfer Rules\
   \
   The funds you receive are transferred to your self-custodial wallet in batches according to the rules below. You can review and adjust the transfer settings on the Receiving and Transfer page.<br>
   1. **Regular Transfer**: when the accumulated pending transfer amount reaches or exceeds the equivalent of 50 USDT (testing phase) / 500 USDT (live phase), a transfer is executed every 10 minutes.<br>
   2. **Minimum Threshold Transfer**: if the accumulated pending transfer amount remains below the Regular Transfer threshold above, a Minimum Threshold Transfer is triggered. This ensures that funds are transferred at least once every 24 hours. To facilitate testing for newly onboarded merchants, the first transaction below the Regular Transfer threshold will automatically trigger this Minimum Threshold Transfer within 10 minutes.<br>
   3. **Transfer Amount**: the accumulated amount of all not-yet-transferred order(s).<br>
   4.  **Transfer Address**: you can select internal Cregis self-custodial wallet addresses to receive the funds.


6.  Additional Payment<br>

    When the first payment is less than the order amount, the order does not fail immediately. Instead, it enters an additional payment process and trigger additional\_payment\_required callback, allowing the payer to complete the remaining balance. This additional payment process is triggered only when all of the following conditions are met.<br>

    * The actual amount received is less than the order amount minus the underpayment tolerance (default is 0).<br>
    * The first payment for the order.



    * The payment currency is a stablecoin. <br>

    Please note that payment currency will be the same as the first payment. The balance amount is calculated by the order amount subtracting the paid amount. The additional payment must be completed within a 7-day time limit; if this limit is exceeded, the order proceeds to the full refund process.\
    \
    To complete the additional payment, the payer can choose one of the below methods:<br>

    * You can check the callback to find the additional payment address and give it to the payer to complete payment.<br>
    * If the payer is paying through the Checkout page, the page will be redirected to the additional payment page automatically.<br>
    * If the payer's email was provided via API Create Order request, the system will send an additional payment email automatically. The payer can open the payment page from the link in the email and complete the payment.<br>
7.  Refund\
    \
    When the payment(s) received do not match the order requirements, a refund is initiated so that the excess or the total can be returned to the payer. Refunds are divided into partial refund and full refund.\
    \
    a. Partial Refund（Overpayment）\
    \
    When the payment amount exceeds the order amount, the original order amount will proceed through the normal transfer process while the excess amount will be directed to the refund process. In this situation, a partial refund callback will also be triggered, allowing merchants to handle the transfer and refund in parallel. The partial refund will be triggered under the following condition:



    * The actual amount paid is greater than the order amount plus the overpayment tolerance (default is 0).<br>

    b. Full Refund<br>

    When invalid payment(s) are received, a full refund will be triggered. In this situation, both a refund callback and an order callback (cancelled) will be triggered simultaneously, so the original order flow is automatically cancelled. The full refund will be triggered under one of the following conditions:<br>

    * The actual amount paid is less than the order amount minus the underpayment tolerance (default is 0), and the payment currency is a non-stablecoin.<br>
    * The additional payment was not completed within the 7-day time limit.<br>
    * After the second payment in the additional payment, the actual amount paid is still less than the order amount minus the underpayment tolerance (default is 0).

    \
    Both refunds can be completed by one of the below methods:<br>

    * Merchants can enter the refund record and initiate the refund.<br>
    * If the payer is paying through the Checkout page, the page will be redirected to the refund page automatically.<br>
    * If the payer's email was provided via Create Order API request, the system will send a refund email to the payer. The payer can open the refund page from the link in the email.<br>
    * Contact the Cregis support team for assistance.<br>

    Please note that the refund currency will be the same as the first payment. For the link in the payer email, it is only valid for up to 7 days if the refund is not processed; after 7 days, you are required to process the refund in the Cregis portal or contact the Cregis support team.<br>
8. Service Fees

| Charge Type       | Charge Model             | Charge from                    |
| ----------------- | ------------------------ | ------------------------------ |
| Order Service Fee | Percentage / Minimum Fee | Team Balance / Transfer Amount |
| Refund Fee        | Fixed Fee                | Transfer Amount                |
| Payment Exception | Percentage / Minimum Fee | Transfer Amount                |



