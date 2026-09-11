# Signing

Once a transaction completes the necessary approval process, it enters the signing stage. When a transaction meets the signing conditions and the current account possesses signing permissions, it is routed to Tasks > Signatures. Signers can sign or reject the transaction. Cregis supports both single-transaction signing and batch signing to help teams process pending transactions efficiently. Once signed, you can view the processed signature history under Tasks > Signed.

**Important Notes**

* If the recipient address is blacklisted, the transaction can only be rejected; signing is not permitted.
* Batch signing only supports transactions of the same cryptocurrency in a single operation. Mixed-currency batch signing is not supported.
* Batch signing only supports single-recipient transfers initiated by single-sig wallets and transactions initiated via API.
* Transactions initiated by multi-sig wallets, Swap applications, or batch transfer functions do not support batch signing and must be processed individually.

## Single-Transaction Signing

Because signing mechanisms differ between single-sig and multi-sig wallets, single-transaction signing is processed based on the outgoing wallet type.

### **Single‑Signature Wallet Transaction Signing**

#### **Cregis Desktop**

For transactions initiated by a single-sig wallet, only one person is required to execute the signature. Navigate to Tasks > Signature, locate the transaction, and click Review on the right side.

<figure><img src="../../.gitbook/assets/image (1131).png" alt=""><figcaption></figcaption></figure>

On the signature details page, review the transaction details and choose an action:

* **Sign**: Authorize the transaction for execution.
* **Reject**: Decline the transaction and stop the signing process. _(Note: If the recipient is a blacklisted address, you can only select Reject.)_

<figure><img src="../../.gitbook/assets/image (1132).png" alt=""><figcaption></figcaption></figure>

Click Sign. In the gas fee pop-up window, confirm the gas fee and click Confirm.

<figure><img src="../../.gitbook/assets/image (1133).png" alt=""><figcaption></figcaption></figure>

Perform identity verification: enter your Transaction Password and click Confirm.

<figure><img src="../../.gitbook/assets/image (1134).png" alt=""><figcaption></figcaption></figure>

After verification, you will be directed to the signing page. Upon successful signing, the system automatically broadcasts the transaction to the blockchain and displays a success prompt.

<figure><img src="../../.gitbook/assets/image (1135).png" alt=""><figcaption></figcaption></figure>

#### **Cregis Mobile**

You can see pending signature items from the Home Page's To-Do section or from **Tasks**. Click on an item to view the transaction details. After confirming the signature, the estimated **Gas Fee** will be displayed.

<div><figure><img src="../../.gitbook/assets/img_v3_0211n_2a2f1841-b696-4306-a26e-ac2d350311hu.jpg" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/img_v3_0211n_59d8f41d-05bc-42fa-ac1f-e85802daeehu.jpg" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/img_v3_0211n_8301a720-3c40-4f02-b68a-a74a42b39dhu.jpg" alt=""><figcaption></figcaption></figure></div>

After clicking Send, you need to complete the transaction password verification. The signing is then successfully completed.

<figure><img src="../../.gitbook/assets/img_v3_0211n_1dd1d744-a9e2-4569-bf30-baf5e65f65hu.jpg" alt="" width="375"><figcaption></figcaption></figure>

### **Multi-Signature Wallet Transaction Signing**

#### **Cregis Desktop**

Multi-sig wallet transactions must satisfy the wallet's configured signature threshold. Navigate to Tasks > Signature, select the target multi-sig transaction, and click Review.

<figure><img src="../../.gitbook/assets/image (1136).png" alt=""><figcaption></figcaption></figure>

Review the transaction details and choose an action:

* **Sign**: Authorize the transaction (requires participation from other signers).
* **Reject**: Decline the transaction and stop the signing process. _(Note: If the recipient is blacklisted, you can only select Reject.)_

<figure><img src="../../.gitbook/assets/image (1137).png" alt=""><figcaption></figcaption></figure>

Click Sign, enter your Transaction Password, and click Confirm.

<figure><img src="../../.gitbook/assets/image (1138).png" alt=""><figcaption></figcaption></figure>

After verification, you will enter a waiting page. You must wait for other wallet members to join until the signature threshold is met.

<figure><img src="../../.gitbook/assets/image (1139).png" alt=""><figcaption></figcaption></figure>

Once the signature request is initiated, other online members of the wallet will receive an invitation notification.&#x20;

<figure><img src="../../.gitbook/assets/image (1140).png" alt=""><figcaption></figcaption></figure>

They must click Multi-Sig Invitation, review the details, and click Join.

<figure><img src="../../.gitbook/assets/image (1141).png" alt=""><figcaption></figcaption></figure>

Joining members must complete identity verification by entering their Transaction Password and clicking Confirm.

<figure><img src="../../.gitbook/assets/image (1142).png" alt=""><figcaption></figcaption></figure>

When the number of participating members reaches the required threshold, the initiator clicks Confirm.

<figure><img src="../../.gitbook/assets/image (1143).png" alt=""><figcaption></figcaption></figure>

In the gas fee pop-up window, confirm the gas fee and click Confirm.

<figure><img src="../../.gitbook/assets/image (1144).png" alt=""><figcaption></figcaption></figure>

Enter the transaction signing page. Upon successful signing, the system automatically broadcasts the transaction to the blockchain and displays a success prompt.

<figure><img src="../../.gitbook/assets/image (1145).png" alt=""><figcaption></figcaption></figure>

#### **Cregis Mobile App**

You can see pending signature items from the Home Page's To-Do section or from **Tasks**. Click on an item to view the transaction details. After confirming the signature, you will need to verify the transaction password.

<div><figure><img src="../../.gitbook/assets/img_v3_0211n_30dae840-0b7e-4016-84f1-912e4afc92hu.jpg" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/img_v3_0211n_30dae840-0b7e-4016-84f1-912e4afc92hu (1).jpg" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/img_v3_0211n_5ec37ddb-a909-48c6-b94c-c1806217dchu.jpg" alt=""><figcaption></figcaption></figure></div>

Once verification is complete, you will enter the multi‑signature process. **If you are the initiator**, you can see which members have joined.\
When the number of joined multi‑signature signers reaches the minimum signing threshold, the signature initiator will see the estimated Gas Fee and can confirm it.

<div><figure><img src="../../.gitbook/assets/img_v3_0211n_b860422e-3d79-4920-9560-b4e0f81333hu.jpg" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/img_v3_0211n_d0b67906-8aee-4691-ad4d-1359317d9bhu.jpg" alt=""><figcaption></figcaption></figure></div>



## Batch Signing

Navigate to Tasks > Signature and click Batch Process in the top right corner.

<figure><img src="../../.gitbook/assets/image (1151).png" alt=""><figcaption></figcaption></figure>

Select the cryptocurrency you wish to batch sign and click View.

<figure><img src="../../.gitbook/assets/image (1146).png" alt=""><figcaption></figcaption></figure>

Select the target transactions and choose an action:

* **Sign**: Authorize the execution of selected transactions.
* **Reject**: Decline selected transactions and stop the signing process.

<figure><img src="../../.gitbook/assets/image (1147).png" alt=""><figcaption></figcaption></figure>

Click Sign. Review the summary statistics for the batch operation and click Confirm.

<figure><img src="../../.gitbook/assets/image (1148).png" alt=""><figcaption></figcaption></figure>

In the gas fee pop-up window, confirm the gas fee and click Confirm.

<figure><img src="../../.gitbook/assets/image (1149).png" alt=""><figcaption></figcaption></figure>

Enter your Transaction Password for identity verification and click Confirm.

<figure><img src="../../.gitbook/assets/image (1150).png" alt=""><figcaption></figcaption></figure>

Upon successful verification, the system executes the batch signing process.

<figure><img src="../../.gitbook/assets/image (1152).png" alt=""><figcaption></figcaption></figure>

When handling multiple pending signatures, use batch signing to process multiple transactions at once.

<figure><img src="../../.gitbook/assets/image (1153).png" alt=""><figcaption></figcaption></figure>

<br>
