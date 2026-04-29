# Introduction

Cregis Payment Engine offers a one-stop cryptocurrency payment solution for businesses. Merchants can quickly integrate the system through a simple API. We provide a pre-designed checkout page for immediate use, while also allowing merchants to customize their own interface based on specific needs. When a merchant initiates a payment request, the system generates a unique payment address, and funds are deposited into the Cregis wallet. Through a 10-minute automatic settlement mechanism, funds are swiftly transferred to the merchant's designated wallet. Merchants can use the Cregis desktop application to view order status, settlement data, and other transaction details at any time, making payment management effortless. We support multi-chain and multi-currency payments, ensuring efficient and flexible fund transfers, and delivering a secure and convenient cryptocurrency payment experience for our clients.

## **Payment Rules**

Cregis supports multiple currencies and chains as [order currencies](https://developer.cregis.com/api-reference/request-apis/payment/payment-order-currency), [payment currencies and settlement currencies](https://developer.cregis.com/api-reference/request-apis/payment/payment-pay-currency) including fiat currencies and cryptocurrencies. If the order currency differs from the payment currency, Cregis will obtain the latest exchange rate in real time and convert and lock the exchange rate for the entire order validity period.

## Settlement Rules

* **Regular Settlement**: If the pending settlement amount reaches or exceeds the equivalent of 50 USDT (testing phase) / 500 USDT (live phase), settlement will occur every 10 minutes.
* **Minimum Threshold Settlement**: If the accumulated pending settlement amount remains below the equivalent of 50 USDT (testing phase) / 500 USDT (live phase), a Minimum Threshold Settlement will be triggered. This ensures merchants receive a payout at least once every 24 hours. To facilitate testing for newly onboarded merchants, the first transaction under 50 USDT will automatically trigger this settlement within 10 minutes.
* **Settlement Amount**: The amount will be credited after deducting transaction fees.
* **Settlement Address**: When setting up the payment engine, merchants can select internal Cregis wallet addresses. Funds can also be settled to an external address after the settlement process.
* **Exchange Rate for Settlement**: Calculations are based on the real-time exchange rate from CoinMarketCap. The rate will be fixed once the order is created.

If fiat settlement is required, please [contact us](https://www.cregis.com/appointment/) for inquiries.



### Order Status

| Order Status | Accept / Set Limits for "Overpayment" or "Partial Payment" | Order Paid & Will Be Settled | Description                                                  |
| ------------ | ---------------------------------------------------------- | ---------------------------- | ------------------------------------------------------------ |
| Pending      | Not Applicable                                             | ✗                            | The order has been created and is still within valid period. |
| Expired      | Not Applicable                                             | ✗                            | The order has been created and has passed the valid period.  |
| Paid         | ✗                                                          | ✓                            | Amount Received = Amount Paid                                |
| Overpaid     | ✓                                                          | ✓                            | Amount Received < Amount Paid                                |
| Partial Paid | ✓                                                          | ✓                            | Amount Received > Amount Paid                                |



## Additional Payment Rule

### **Trigger Conditions**

If a payment meets all of the following conditions, the order will enter the additional payment process and trigger a [`paid_partial`](https://developer.cregis.com/api-reference/callback/payment-engine) callback:

1. The order does not accept partial payments.
2. It is the first payment for the order.
3. Amount Paid < Order Amount OR Amount Paid < (Order Amount - Underpayment Tolerance) ([`underpaid_tolerance`](https://developer.cregis.com/api-reference/request-apis/payment/payment-engine-create)).
4. The payment currency is a stablecoin.



### Additional Payment Flow

1. The system will send an additional payment email to the payer (the email address filled at [`payer_email`](https://developer.cregis.com/api-reference/request-apis/payment/payment-engine-create) when the order was created).
2. The payer can access the payment page via the link provided in the email.
3. The payment currency and network will be the same as the first payment.
4. The balance amount will be calculated by converting the original order amount (in its currency) at the current exchange rate and then subtracting the already paid amount.
5. The additional payment must be completed within a 7-day time limit. If this limit is exceeded, the order will be proceeded to full refund process.
6. Upon successful balance payment, a [`paid_remain`](https://developer.cregis.com/api-reference/callback/payment-engine) callback will be triggered.



## **Refund Rules**

### **Partial Refund**

#### **Trigger Conditions**

If an order meets all of the following conditions, it will enter the partial refund process and trigger a [`paid_over`](https://developer.cregis.com/api-reference/callback/payment-engine) callback:

1. The order does not accept overpayments.
2. Amount Paid > Order Amount OR Amount Paid > Order Amount + Overpayment Tolerance ([`overpaid_tolerance`](https://developer.cregis.com/api-reference/request-apis/payment/payment-engine-create)).
3. The payment currency is a stablecoin.



#### **Partial Refund Process**

1. The system will send a partial refund email to the payer (the email address filled at [`payer_email`](https://developer.cregis.com/api-reference/request-apis/payment/payment-engine-create) when the order was created).
2. The payer can access the partial refund page via the link provided in the email.
3. The refund currency and network will be the same as the first payment.
4. The partial refund amount will be calculated by taking the Amount Paid and subtracting the original order amount (converted at the exchange rate).
5. The partial refund must be completed within a 7-day time limit. If this limit is exceeded, the order will be automatically fully refunded.
6. After a successful partial refund, the order will be settled.



### **Full Refund**

#### **Trigger Conditions**

An order will enter the full refund process if any of the following conditions are met:

1. The order does not accept partial payments, and it was paid with a non-stablecoin was underpaid.
2. The additional payment was not completed within the 7-day time limit.
3. The partial refund was not completed within the 7-day time limit.
4. After the second payment in the additional payment process, the Amount Paid is still < Order Amount OR Amount Paid < Order Amount - Underpayment Tolerance ([`underpaid_tolerance`](https://developer.cregis.com/api-reference/request-apis/payment/payment-engine-create)).

#### Full Refund Process

* The system will send a full refund email to the payer (the email address filled at [`payer_email`](https://developer.cregis.com/api-reference/request-apis/payment/payment-engine-create) when the order was created).
* The payer can access the full refund page via the link provided in the email.
* The refund currency and network will be the same as the first payment.
* The full refund amount will be the total of all amounts paid.
* The full refund must be completed within a 7-day time limit.
* If the 7-day time limit is exceeded, the payer must contact customer support to handle the subsequent steps.
* After the refund is completed, the system will trigger a [`refunded`](https://developer.cregis.com/api-reference/callback/payment-engine) callback.



### Other Refund Information



* A service fee will be charged for each refund. The specific fee amount will be clearly displayed on the refund page and will be deducted directly from the refund amount.

