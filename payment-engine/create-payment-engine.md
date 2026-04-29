# Create Payment Engine

1.  Click "Payment Engine" from the Cregis's Portal

    <figure><img src="../.gitbook/assets/image (789).png" alt=""><figcaption></figcaption></figure>



2.  After clicked, please fill in the "Project Name" and "Industry" related information.

    <figure><img src="../.gitbook/assets/image (790).png" alt=""><figcaption></figcaption></figure>



3.  Then, set up the merchant information including the "Merchant Name" and "Merchant Logo" that will be displayed on the Checkout Page.

    <figure><img src="../.gitbook/assets/image (791).png" alt=""><figcaption></figcaption></figure>



4.  Select the payment currency for payment engine. Also, a tooltip (?) will indicate the minimum payment amount required by the corresponding chain.

    <figure><img src="../.gitbook/assets/image (792).png" alt=""><figcaption></figcaption></figure>



5.  Set up the settlement currency. The settlement currency must be configured independently for each payment currency. (If a "Wallet Address" is not configured, you can add a new currency and address by following [this guide](https://support.cregis.com/wallet-and-transactions/token).)

    <figure><img src="../.gitbook/assets/image (793).png" alt=""><figcaption></figcaption></figure>



6.  If not all configured, you can still continue and configure later, but a pop-up window will remind you that if the payment currency does not have a settlement configuration, order will remain in the "Paid" status until the setup is completed. The system will automatically initiate settlement once the configuration is complete. (For subsequent configuration changes, please refer to [this manual section](https://support.cregis.com/payment-engine/payment-engine-configuration).)

    <figure><img src="../.gitbook/assets/image (794).png" alt=""><figcaption></figcaption></figure>



7.  After completing the configuration, verify with your Transaction Password.

    <figure><img src="../.gitbook/assets/image (795).png" alt=""><figcaption></figcaption></figure>



8.  Then, verify with your Google Authenticator code.

    <figure><img src="../.gitbook/assets/image (796).png" alt=""><figcaption></figcaption></figure>



9.  Upon completion, you will enter the Payment Engine page. You can click on Settings to view the relevant API access information.\
    <mark style="color:green;">Note: Do not easily disclose the project API key to others as it may lead to asset loss.</mark>

    <figure><img src="https://support.cregis.com/~gitbook/image?url=https%3A%2F%2F3263384427-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Fg3NzJ0yGNKhTsgI2zNjK%252Fuploads%252F0zH0rocmOyhTrTBcoPQV%252Fimage.png%3Falt%3Dmedia%26token%3D1b822e42-09f9-47b5-9914-df5917b514ea&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=41ba21a9&#x26;sv=2" alt=""><figcaption></figcaption></figure>



10. Before calling the API, you must add the IP address of the device calling the API to the IP Whitelist for security. Otherwise, the API will return an error. You can configure this in "IP Whitelist" by clicking "Create Group," entering the IP address, clicking "Save" and then completing authorization verification.

    <figure><img src="https://support.cregis.com/~gitbook/image?url=https%3A%2F%2F3263384427-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Fg3NzJ0yGNKhTsgI2zNjK%252Fuploads%252F9y7GsB6yUDOsYuZUzOjJ%252Fimage.png%3Falt%3Dmedia%26token%3D14e390d7-486c-48b1-b9d1-7011cdfeda81&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=1fccdfb&#x26;sv=2" alt=""><figcaption></figcaption></figure>



11. After the configuration is complete, the Payment Engine is ready for use. Please refer to [this development document](https://developer.cregis.com/api-reference/request-apis/payment/payment-engine-create) for the technical documentation.



