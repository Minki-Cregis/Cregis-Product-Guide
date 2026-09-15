# Payout External Verification

Payout External Verification adds an additional approval layer controlled by the customer's business system before a payout request (Wallet Payout and Sub-Address Payout) enters the Cregis approval workflow.When this feature is enabled, payout requests are not processed immediately after they are submitted. Instead, Cregis sends the payout request to the customer's configured external verification system through a callback API. The customer can then review the request based on their own business rules, risk control policies, or approval workflow, and submit the verification result back to Cregis.Cregis processes the payout request according to the returned verification result:

* **Approved (ok):** The payout request proceeds with the subsequent approval, signing, and blockchain transaction process.
* **Rejected (deny):** The payout request is terminated, and no signing or blockchain broadcasting will be performed.

By integrating Payout External Verification with internal approval, risk management, or compliance systems, enterprises can implement customized payout approval workflows, strengthen fund security, and enhance risk control capabilities.

## **Enable Payout External Verification**

Log in to the Cregis, then navigate to **WaaS > Settings > Callback Setting**. Click **Enable** under Payout External Verification.

<figure><img src="../../.gitbook/assets/image (1170).png" alt=""><figcaption></figcaption></figure>

In the confirmation dialog, click **Confirm**.

<figure><img src="../../.gitbook/assets/image (1171).png" alt=""><figcaption></figcaption></figure>

On the **Configure Callback URL** page, enter or paste the callback URL that will receive payout verification requests, then click **Test Connection**.

<figure><img src="../../.gitbook/assets/image (1172).png" alt=""><figcaption></figcaption></figure>

The system will attempt to connect to the specified callback URL. If the test is successful, the message **"Connection test successful. The server responded normally."** will be displayed. Click **OK**.

<figure><img src="../../.gitbook/assets/image (1173).png" alt=""><figcaption></figcaption></figure>

Complete identity verification. Payout External Verification will then be enabled successfully.

<figure><img src="../../.gitbook/assets/image (1174).png" alt=""><figcaption></figcaption></figure>

**Edit Callback URL**

Log in to the Cregis, then navigate to **WaaS > Settings > Callback Setting**. Click **Edit** under Payout External Verification.

<figure><img src="../../.gitbook/assets/image (1175).png" alt=""><figcaption></figcaption></figure>

On the **Configure Callback URL** page, enter or paste the new callback URL, then click **Test Connection**.

<figure><img src="../../.gitbook/assets/image (1176).png" alt=""><figcaption></figcaption></figure>

The system will attempt to connect to the specified callback URL. If the test is successful, the message **"Connection test successful. The server responded normally."** will be displayed. Click **OK**.

<figure><img src="../../.gitbook/assets/image (1177).png" alt=""><figcaption></figcaption></figure>

Complete identity verification, then click **Confirm**. The callback URL will be updated successfully.

<figure><img src="../../.gitbook/assets/image (1178).png" alt=""><figcaption></figcaption></figure>

**Disable Payout External Verification**

Log in to the Cregis, then navigate to **WaaS > Settings > Callback Setting**. Click **Disable** under Payout External Verification.

<figure><img src="../../.gitbook/assets/image (1179).png" alt=""><figcaption></figcaption></figure>

In the confirmation dialog, click **Confirm**.

<figure><img src="../../.gitbook/assets/image (1180).png" alt=""><figcaption></figcaption></figure>

Complete identity verification, then click **Confirm**. Payout External Verification will be disabled successfully.

<figure><img src="../../.gitbook/assets/image (1181).png" alt=""><figcaption></figcaption></figure>
