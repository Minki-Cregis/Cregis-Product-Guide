---
hidden: true
---

# Order Logic

## Additional payment process

* **Triggering conditions**
  * When merchants configure to not accept partial paid order via API
  * The additional payment process only supports orders paid by stablecoins. Non-stablecoin partial paid order will go through full refund process
* **Email notification**
  * Cregis will send a pay order remains notification email to payee. The payee's email address needs to be passed in by the merchant through the order creation API.
  * User accesses additional payment checkout page via email
* **Payment Rules**
  * Users have 24-hours to complete the additional payment of remaining order amount after receiving email notification
  * The remaining order amount would be calculated using the original order's exchange rate , and users would need to pay using the original payment cryptocurrency and network
* **Follow-up process**
  * If users do not complete paying the remaining order amount within 24 hours, the order will enter the full refund process.
  * When the user completes the payment, Cregis will notify the merchant through order callback. For callback details, please refer to the payment engine callback API document.
  * When the user completes the payment, the order will be automatically settled according to the settlement rules.

## **Partial Refund Process**

* **Triggering conditions**
  * When merchants configure to not accept overpaid orders via API
  * Partial Refund Process only supports orders paid by stablecoins, non-stablecoin partial paid order will go through full refund process
* **Email notification**
  * Cregis will send a refund notification email to the payee. The payee's email address needs to be passed in by the merchant through the order creation API.The user can enter the refund application page and provide the refund address within 24 hours after Cregis sends out the refund email.
* **Refund rules**
  * The difference to be refunded will be calculated based on the exchange rate locked in the original order, and the partial refund will be returned in the payment currency and payment network of the original order.A refund handling fee will be charged for each refund. The handling fee amount will be clearly displayed on the refund request page and will be deducted directly from the refund amount.
* **Follow-up process**
  * Cregis will refund within 24 hours after receiving the refund address from the user. After the refund is completed, Cregis will notify the refunding user of the refund details by email.When Cregis completes the partial refund, Cregis will notify the merchant through order callback. For callback details, please refer to the payment engine callback API document.If the user fails to submit a partial refund application on the refund application page within 24 hours, the order will enter the full refund process.

## Full refund process

* **Triggering conditions**
  * If the merchant configures NOT to accept overpaid order or partial paid order through API configuration
    * Partial payment orders paid in non-stablecoins will directly enter the full refund process
  * Partial payment orders that are not completed within 24 hours
* **Email notification**
  * Cregis will send a full refund notification email to the payee. The payee's email address needs to be passed in by the merchant through the order creation API.The user can enter the refund application page and provide the refund receiving address according to the instructions in the email within 24 hours after Cregis sends out the refund email.
* **Refund rules**
  * The refund will be paid in the original payment currency and payment network.A refund handling fee will be charged for each refund. The handling fee amount will be clearly displayed on the refund request page and will be deducted directly from the refund amount.
* **Follow-up process**
  * Cregis will refund within 24 hours after receiving the refund receiving address replied by the user. When the refund is completed, Cregis will notify the user of the refund details by email. When Cregis completes the refund, Cregis will notify the merchant through the order callback. For callback details, please refer to the payment engine callback API document.If the user fails to submit a full refund application on the refund application page within 24 hours, no refund will be provided afterwards.



## Full refund process

| Order Status | Accept / Set Limits for "Overpayment" or "Partial Payment" | Order Paid | Description                                                  |
| ------------ | ---------------------------------------------------------- | ---------- | ------------------------------------------------------------ |
| Pending      | Not Applicable                                             | ✗          | The order has been created and is still within valid period. |
| Expired      | Not Applicable                                             | ✗          | The order has been created and has passed the valid period.  |
| Paid         | ✗                                                          | ✓          | Amount Received = Amount Paid                                |
| Overpaid     | ✓                                                          | ✓          | Amount Received < Amount Paid                                |
| Partial Paid | ✓                                                          | ✓          | Amount Received > Amount Paid                                |

