# Payment Link (Checkout Page)

Cregis provides an industry-standard checkout interface via its API, allowing merchants to facilitate payments for their customers. Merchants can redirect users from their website's payment page to this checkout interface, and upon payment completion, users are automatically redirected back to the website. This reduces the development and manpower costs required for merchants to build a payment system.

### **Checkout Page Payment Process**



1.  On the checkout page, the payer can select one cryptocurrency to complete the payment. If the order currency differs from the payment currency, the system will automatically perform the conversion using real-time exchange rates. (Merchants can also restrict the accepted payment currencies via the [`tokens`](https://developer.cregis.com/api-reference/request-apis/payment/payment-engine-create) parameter in the API.)

    <div align="left"><figure><img src=".gitbook/assets/螢幕截圖 2025-11-07 下午5.57.12.png" alt="" width="375"><figcaption></figcaption></figure></div>



2.  Payers can also review order details on the checkout page including the order amount, order number, product description, etc.

    <div align="left"><figure><img src=".gitbook/assets/螢幕截圖 2025-11-07 下午5.57.19.png" alt="" width="375"><figcaption></figcaption></figure></div>



3.  After selecting the payment currency, the payer will need to choose the payment network.

    <div align="left"><figure><img src=".gitbook/assets/螢幕截圖 2025-11-07 下午5.57.28.png" alt="" width="375"><figcaption></figcaption></figure></div>



4.  Once the selection is complete, the system will generate a payment address and a QR code. The payer can either copy the address or scan the QR code to complete the payment.

    <div align="left"><figure><img src=".gitbook/assets/螢幕截圖 2025-11-07 下午5.58.01.png" alt="" width="375"><figcaption></figcaption></figure></div>



5.  Payers may also choose to use a third-party wallet to scan the QR code for payment. After scanning, the third-party wallet will automatically fill in the currency, network and amount, allowing the payer to confirm the payment seamlessly.

    <div align="left"><figure><img src=".gitbook/assets/螢幕截圖 2025-11-07 下午5.58.11.png" alt="" width="375"><figcaption></figcaption></figure></div>



6.  After a successful payment, the page will redirect to a payment completion page. After 5 seconds, the user will be automatically redirected back to the merchant’s website (specified via the [`success_url`](https://developer.cregis.com/api-reference/request-apis/payment/payment-engine-create) field in the API). If the order status is in an [usual status](https://support.cregis.com/payment-engine/introduction#order-status), the payment completion page will also display the reason and automatically initiate corresponding processes such as sending emails for additional payment requests, partial refunds or full refunds.

    <div align="left"><figure><img src=".gitbook/assets/螢幕截圖 2025-11-07 下午5.56.19.png" alt="" width="375"><figcaption></figcaption></figure></div>



7.  If the payer does not complete the payment within the order's validity period, the order will automatically expire. By clicking the "Return" button, the payer will be redirected to the [`cancel_url`](https://developer.cregis.com/api-reference/request-apis/payment/payment-engine-create) submitted via the API.

    <div align="left"><figure><img src=".gitbook/assets/螢幕截圖 2025-11-07 下午5.55.44.png" alt="" width="375"><figcaption></figcaption></figure></div>

