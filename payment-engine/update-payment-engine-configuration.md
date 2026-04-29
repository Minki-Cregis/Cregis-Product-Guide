# Update Payment Engine Configuration

## **Payment Currency & Settlement Configuration**



### Add Payment Currency



1.  Users can modify their payment and settlement currency in the client portal.

    <figure><img src="../.gitbook/assets/image (779).png" alt=""><figcaption></figcaption></figure>



2.  Click "Add Payment Currency". The user can then select a new payment currency and set the settlement currency. The system will display the corresponding transaction fee rate. Finally, select the settlement wallet and address.

    <figure><img src="../.gitbook/assets/image (780).png" alt=""><figcaption></figcaption></figure>



3.  Complete identity verification

    <figure><img src="../.gitbook/assets/image (781).png" alt=""><figcaption></figcaption></figure>



4.  After successful verification, the currency will be added to the list.

    <figure><img src="../.gitbook/assets/image (782).png" alt=""><figcaption></figcaption></figure>



### Bulk Edit Settlement Settings



1.  Once the payment engine has at least one payment currency, users can use the "Bulk Edit Settlement Settings" option to modify settlement wallets and addresses in bulk.

    <figure><img src="../.gitbook/assets/image (783).png" alt=""><figcaption></figcaption></figure>



2.  After clicking, you can modify the settlement wallet and address for each currency. Upon completion, click confirm, and the changes will take effect after verification.

    <figure><img src="../.gitbook/assets/image (784).png" alt=""><figcaption></figcaption></figure>



## **Order Overpaid & Underpaid Configuration (For API V1 Users Only)**



Recommend: Upgrade to the [payment engine's latest API V2 version](https://developer.cregis.com/api-reference/request-apis/payment/payment-engine-create) to handle "Overpayment" and "Partial Payment" logic via the API.



1.  To accept all "Overpayments" or "Partial Payments", you can select "Accept" for "Overpaid Orders" and "Partially Paid Orders" in the "Order Processing" page.

    <figure><img src="../.gitbook/assets/image (786).png" alt=""><figcaption></figcaption></figure>



2.  To set upper and lower limits for "Overpayment" or "Partial Payment", select "Add Order Currency" in the "Payment Accuracy Settings" within the portal. Then, set the corresponding tolerance upper and lower limits for "Overpayment" or "Partial Payment" for the "Order Currency". (If the payer uses a different "Payment Currency", the system will perform real-time exchange rate conversion.)

    <figure><img src="../.gitbook/assets/image (787).png" alt=""><figcaption></figcaption></figure>



## **Merchant Information Configuration**



1.  For the merchant information displayed on the checkout page such as name, logo, etc, modifications can be made in the "Merchant Information" section under "Settings".

    <figure><img src="../.gitbook/assets/image (788).png" alt=""><figcaption></figcaption></figure>



## Notification Settings



1.  Users can configure project notifications themselves. The available options are listed below. Click the toggles for enablement.

    * **Abnormal Callback:** When a system callback fails.
    * **Enable/Disable Project:** When the system enables or disables a project.
    * **Reset API Key:** When a project's API Key is reset.

    <figure><img src="../.gitbook/assets/image (733).png" alt=""><figcaption></figcaption></figure>



2.  To notify multiple people, you can select the relevant team members in "Edit".

    <figure><img src="../.gitbook/assets/image (734).png" alt=""><figcaption></figcaption></figure>





