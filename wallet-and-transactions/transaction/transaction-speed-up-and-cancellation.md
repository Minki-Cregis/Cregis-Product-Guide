# Transaction Speed Up and Cancellation

When a transaction cannot be completed due to low gas fees, users can use the speed-up or cancellation feature. Please note this feature is only available for <mark style="color:green;">**BTC and ETH-based**</mark> cryptocurrencies.

## **ETH Series**

### **Transaction Speed Up**

Click "<mark style="color:green;">**Speed Up**</mark>" in the pending transaction.

<figure><img src="../../.gitbook/assets/image (133).png" alt=""><figcaption></figcaption></figure>

After clicking, if the token has more than one pending transaction, a transaction speed-up list page will pop up. Operate in order from the smallest Nonce to the largest by clicking "Speed Up." If the token has only one pending transaction, skip this step.

<figure><img src="../../.gitbook/assets/image (134).png" alt=""><figcaption></figcaption></figure>

Clicking "Speed Up" will expand the transaction details and provide options for the speed-up gas fee. Click to choose from different gas fee options. Users can also customize the gas fee.

<figure><img src="../../.gitbook/assets/image (135).png" alt=""><figcaption></figcaption></figure>

Custom gas fee settings are divided into <mark style="color:green;">**Advanced Mode**</mark> and <mark style="color:green;">**Standard Mode**</mark>:

* **Advanced Mode**: Uses the <mark style="color:green;">**EIP-1559 protocol**</mark>, which applies a new fee calculation method to accelerate transaction confirmation. This mode theoretically reduces gas fees compared to Standard Mode. In Advanced Mode, users can customize the Max Fee and Max Priority Fee, allowing precise control to ensure transaction priority. This mode is particularly suitable for users who need high-priority confirmation while aiming to save on fees.
* **Standard Mode**: Based on the traditional gas fee structure, users can set the Gas Price and Gas Limit to determine the transaction fee. Although this mode is gradually being replaced by the EIP-1559 protocol, it remains suitable for users who are unfamiliar with the new mode or prefer traditional fee settings.

<figure><img src="../../.gitbook/assets/image (136).png" alt=""><figcaption></figcaption></figure>

Once the setup is complete, proceed with identity verification.

<figure><img src="../../.gitbook/assets/image (699).png" alt=""><figcaption></figcaption></figure>

After authentication is complete, you will see a "Speeding Up" tag.

<figure><img src="../../.gitbook/assets/image (137).png" alt=""><figcaption></figcaption></figure>

After the speed-up is complete, you will see an "Sped Up" tag.<img src="../../.gitbook/assets/image (695).png" alt="" data-size="line">

<figure><img src="../../.gitbook/assets/image (138).png" alt=""><figcaption></figcaption></figure>

### Transaction Cancellation

Click "<mark style="color:green;">**Cancel"**</mark> within a pending transaction.

<figure><img src="../../.gitbook/assets/image (139).png" alt=""><figcaption></figcaption></figure>

After clicking, if the token has more than one pending transaction, a transaction cancellation list page will pop up. Operate in order from the smallest Nonce to the largest by clicking "Cancel." If the token has only one pending transaction, skip this step.

<figure><img src="../../.gitbook/assets/image (140).png" alt=""><figcaption></figcaption></figure>

Clicking "Cancel" will expand the transaction details and provide options for the cancellation gas fee. Click to choose from different gas fee options. Users can also customize the gas fee. Since canceling a transaction involves resending a transaction with an amount of $0, the sending amount here is displayed as 0.

<figure><img src="../../.gitbook/assets/image (141).png" alt=""><figcaption></figcaption></figure>

After completing the setup, proceed with identity verification.

<figure><img src="../../.gitbook/assets/image (704).png" alt=""><figcaption></figcaption></figure>

After successful cancellation, the user interface will show two transaction records. The one with an amount of 0 is the record for the cancellation transaction, while the previous record will have a "Cancelled" tag.

## BTC Series

### **Transaction Speed Up**

Click "<mark style="color:green;">**Speed Up**</mark>" in the pending transaction.

<figure><img src="../../.gitbook/assets/image (705).png" alt=""><figcaption></figcaption></figure>

Once clicked, transaction details will expand with an option to increase the gas fee. Users can choose from different gas fee options or customize the fee.

<figure><img src="../../.gitbook/assets/image (707).png" alt=""><figcaption></figcaption></figure>

CUsers can set the Gas Price and Gas Limit when customizing the gas fee. The system will automatically estimate the gas fee as a reference.

<figure><img src="../../.gitbook/assets/image (708).png" alt=""><figcaption></figcaption></figure>

After completing the setup, click "Confirm" and proceed with identity verification.

<figure><img src="../../.gitbook/assets/image (694).png" alt=""><figcaption></figcaption></figure>

Once verification is successful, a "Speeding Up" tag will appear. If the waiting time is too long, users can choose to accelerate again by adjusting the gas fee.

<figure><img src="../../.gitbook/assets/image (711).png" alt=""><figcaption></figcaption></figure>

After the acceleration is complete, an "Speed up" tag will be displayed.<img src="../../.gitbook/assets/image (709).png" alt="" data-size="line">

<figure><img src="../../.gitbook/assets/image (710).png" alt=""><figcaption></figcaption></figure>

### **Transaction Cancellation**

In the pending transaction, click "<mark style="color:green;">**Cancel**</mark>".

<figure><img src="../../.gitbook/assets/image (712).png" alt=""><figcaption></figcaption></figure>

Clicking will expand the transaction details, showing an option to set the gas fee for cancellation. Users can choose from various gas fee options or customize the fee.

For BTC cancellations, the Replace-by-Fee (RBF) method is used, which sends a new transaction with the same UTXO as the original. As a result, the transaction amount is <mark style="color:green;">**displayed as $0.**</mark>

<figure><img src="../../.gitbook/assets/image (713).png" alt=""><figcaption></figcaption></figure>

After completing the setup, proceed with identity verification.

<figure><img src="../../.gitbook/assets/image (714).png" alt=""><figcaption></figcaption></figure>

Upon successful cancellation, the user interface will display two transaction records: one with an amount of $0, representing the cancellation request, and the earlier record will show a "Cancelled" tag.

<figure><img src="../../.gitbook/assets/image (715).png" alt=""><figcaption></figcaption></figure>
