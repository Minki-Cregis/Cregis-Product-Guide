# Report

This page provides a complete query of wallet transaction records, covering team wallet and Waas project transactions, supporting enterprises in clearly reviewing all details. You can filter as needed and export data as Excel files for reconciliation or other financial tasks.

## **Viewing Record Details**

Users can click on a record to view its details.

<figure><img src="../../.gitbook/assets/image (1033).png" alt=""><figcaption></figcaption></figure>

\
A window will pop up displaying the detailed record of the transaction.

<figure><img src="../../.gitbook/assets/image (1034).png" alt=""><figcaption></figcaption></figure>

## **Changing Time Zone**

Users can click on the transaction time to change the time zone for the displayed data. Exported data will also follow the currently selected time zone.

<figure><img src="../../.gitbook/assets/image (1035).png" alt=""><figcaption></figcaption></figure>

## **Exporting Transaction Records**

Click the export button in the top right corner to select the date range for export. Please note that the export date range currently cannot exceed 12 months, and the exported data will be adjusted according to the currently selected time zone.

<figure><img src="../../.gitbook/assets/image (1036).png" alt=""><figcaption></figcaption></figure>

After clicking "Export," the system will begin preparing the file. Processing time depends on the data volume. Once completed, you can download it from "Export History." You can also view and download historical export files from other team members there.

**Note:** The exported file is a compressed package. Transactions in the "Batch Transfer" category (on-chained via packaging technology) currently share the same transaction hash. Therefore, the detailed breakdown of these transactions will be generated separately and saved in a file with "batch" in its name within the compressed package.

<figure><img src="../../.gitbook/assets/image (1037).png" alt=""><figcaption></figcaption></figure>

## **Transaction Type Explanation**

<table><thead><tr><th width="211.171875">Transaction Type</th><th width="152.8984375">Sent/Received</th><th width="337.4140625">Definition</th><th width="491.6328125">Trigger Scenario</th></tr></thead><tbody><tr><td>Manual Wallet Sent</td><td>Sent</td><td>Wallet withdrawal initiated from the client</td><td>Clicking "Send" from the wallet, team member initiating a payment request, deposits via on-chain transactions (Team, Crypto Card)</td></tr><tr><td>API Initiates Sent</td><td>Sent</td><td>Transfer out request initiated via API</td><td>Transactions sent via API requests, including all transfers from main addresses and sub-addresses</td></tr><tr><td>Collection Sent</td><td>Sent</td><td>Project sub-address collection withdrawal</td><td>Triggered during project collections, transferring out from sub-addresses; API-triggered collections (each instance involves both a Sent and a Receive)</td></tr><tr><td>Collection Receive</td><td>Received</td><td>Project sweep transfer into the wallet</td><td>Triggered during project collections, transferring into the wallet from sub-addresses; API-triggered collections (each instance involves both a Sent and a Receive)</td></tr><tr><td>Gas Fee (Collection) Sent</td><td>Sent</td><td>Funds transferred out from the main wallet to pay for collection gas fees</td><td>When gas fees are required for a collection (each instance involves both a Sent and a Receive)</td></tr><tr><td>Gas Fee (Collection) Receive</td><td>Received</td><td>Project sub-address receives funds to pay for collection gas fees</td><td>When gas fees are required for a collection (each instance involves both a Sent and a Receive)</td></tr><tr><td>Standard Receive</td><td>Received</td><td>When an address receives a fund transfer</td><td>Includes all receipts to main addresses and sub-addresses</td></tr><tr><td>Parallel Sent</td><td>Sent</td><td>Transactions sent out in a packaged form (Currently grouped as one transaction type as they cannot be split)</td><td>When a user has multiple transactions of the same series sent on-chain in a packaged form simultaneously</td></tr></tbody></table>
