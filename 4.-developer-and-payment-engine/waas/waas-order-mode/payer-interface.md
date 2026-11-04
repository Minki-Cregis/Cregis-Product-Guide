---
description: >-
  This chapter explains how a payer completes a payment. WaaS Order Mode offers
  two ways to accept payment: the Cregis built-in payment link (hosted checkout)
  and self-hosted payment acceptance website.
---

# Payer Interface

1. Cregis Built-in Payment Link\
   \
   This enables you to send the checkout\_url (received in the Create Order response) to your payers. All of the first payment, additional payment if needed, partial refund if needed, full refund if needed and the completion page are handled in a one-step flow, and the payer can be redirected back to your page after completion. For example: if the first payment is underpaid, the checkout page will be redirected to the additional payment page, if the first payment is overpaid, the checkout page will be redirected to the partial refund page and so on.<br>
   1. Choose the cryptocurrency on the checkout page: the payer can select one cryptocurrency to complete the payment. If the order currency differs from the payment currency, the system automatically performs the conversion using the real-time exchange rate. (Merchants can also restrict the accepted payment currencies via the tokens parameter in the API.)\
      ![](<../../../.gitbook/assets/image (1234).png>)<br>
   2.  Review the order details: payers can review the order details on the checkout page including the order amount, order number, product description and so on.

       <figure><img src="../../../.gitbook/assets/image (1235).png" alt=""><figcaption></figcaption></figure>


   3. Choose the payment network: after selecting the payment currency, the payer chooses the payment network.\
      ![](<../../../.gitbook/assets/image (1236).png>)<br>
   4. Pay to the generated address or QR code: once the selection is complete, the system generates a payment address and a QR code. The payer can either copy the address or scan the QR code to complete the payment.\
      ![](<../../../.gitbook/assets/image (1237).png>)<br>
   5. Pay with a third-party wallet: payers may also choose to use a third-party wallet to scan the QR code for payment. After scanning, the third-party wallet automatically fills in the currency, network and amount, allowing the payer to confirm the payment seamlessly.\
      ![](<../../../.gitbook/assets/image (1238).png>)<br>
   6. Completion and redirect: after a successful payment, the page is redirected to a payment completion page. After 5 seconds, the payer will be automatically redirected back to the merchant's website (specified via the success\_url field in the API).\
      ![](<../../../.gitbook/assets/image (1239).png>)<br>
   7. Underpaid: if the payment is partial (order status is Additional Payment Required), the checkout page will be directed to the additional payment page. The payer can use the QR code to pay the remaining balance. Once the payment is done, it is directed to the success page as in step f.\
      ![](<../../../.gitbook/assets/image (1240).png>)<br>
   8. Overpaid: if the payment is overpaid (the order status is paid because the refund and order flows are processed separately), the checkout page is directed to the partial refund page, which shows the refund reason and amount. The payer can fill in the refund information. Once completed, it is directed to the success page as in step f.\
      \
      \
      \
      \
      \
      <br>
   9. Full-refund: if the payment is partial paid with a non-stablecoin, still partial paid after the additional payment or the additional payment not completed within valid time, the checkout page is directed to the full refund page, which shows the refund reason and amount. The payer can fill in the refund information. Once completed, it is directed to the refund completion page.\
      \
      \
      \
      <br>
   10. Timeout: if the order times out (order status is expired), the checkout page is directed to the timeout page.\
       \
       \
       \
       \
       <br>
   11. AML hit: if the payment hits the AML rules (the order status will be cancelled), the checkout page is directed to the transaction cancelled page and the payer is notified to reach the merchant for the next step.<br>
2.
