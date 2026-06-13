# Collection

Collection is used to actively aggregate assets from the sub-addresses of a WaaS project into a designated collection address. This facilitates unified management of fund balances, improves capital efficiency, and reduces the costs of managing dispersed assets. Currently, the following three collection methods are supported:

* Manual Collection: After creating a collection rule, collection is initiated manually. The system will automatically filter sub-addresses that meet the criteria according to the rule, and collect all eligible assets within those addresses into the designated receiving address.
* API Collection: After initiating a collection request via API, it can be processed manually or handled automatically on the API Collection page. Users can specify the collection address and amount to precisely control collection behavior.
* Auto-Collection: After creating an automation rule, the system automatically initiates the collection without manual intervention. The system will automatically filter sub-addresses that meet the criteria according to the rule, and collect all eligible assets within those addresses into the designated receiving address.

#### Manual Collection

Users can configure collection rules in advance and manually trigger collection tasks when needed. The system will filter sub-addresses that meet the criteria according to the rules for collection.

> Navigation Path: WaaS Project → Collection → Rule Configuration

**Create a Collection Rule**

*   Click the "Add" button on the page to enter the creation page.<br>

    <figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
*   Configure the collection rule, including Rule Name, Collection Currency, Collection Amount, and Destination Address. The collection amount supports the following four modes:

    * No Limit: Collects funds from all addresses. If the address balance is less than or equal to the minimum sending amount, collection will not be performed.
    * Greater Than or Equal To: Only collects addresses with a balance greater than or equal to the specified amount.
    * Less Than or Equal To: Only collects addresses with a balance less than or equal to the specified amount.
    * Amount Range: Only collects addresses with a balance within the specified amount range.

    <figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
* Once the configuration is complete, click the "Confirm" button for Google Authenticator verification. Upon successful verification, the rule is successfully created.

**Initiate Collection**

*   After the rule is created, click the "Start Collection" button in the rule list to initiate the collection.<br>

    <figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
*   Enter the Collection Confirmation page. The system will automatically filter sub-addresses that meet the criteria based on the current rule and display the estimated collectable amount/count. Click the "Confirm" button after verification.<br>

    <figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>
*   Enter the transaction password, then click the "Confirm" button to start the collection.<br>

    <figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>
*   Once the collection starts, you can view the collection progress on the "Task Records" page.<br>

    <figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

#### API Collection

After the business system invokes the API collection, the system generates a pending collection task and displays it on the API Collection page. Collection can be triggered manually or via automated tasks when needed.

> Navigation Path: WaaS Project → Collection → API Collection

**Initiate an API Collection Request**

* Please go to the "[Developer Documentation](https://developer.cregis.com/quickstart)" to understand the detailed method for invoking API collection requests.

**Process API Collection Manually**

* On the API Collection page, multiple collection requests can be selected in batches to be processed simultaneously (collect or reject).
*   If performing a batch collection operation, please filter by the specified currency first before operating. Since the on-chain processing mechanisms differ for different currencies, the system does not support cross-currency batch collection.<br>

    <figure><img src="../../.gitbook/assets/image (1053).png" alt=""><figcaption></figcaption></figure>
* After selecting the collection requests to be processed, click the "Collect" button to enter the Collection Confirmation page. Confirm and select the Gas Fee, then click the "Confirm" button.
*   Enter the transaction password, then click the "Confirm" button to start the collection.<br>

    <figure><img src="../../.gitbook/assets/image (1054).png" alt=""><figcaption></figcaption></figure>
*   Once the collection starts, you can click the collection progress button at the bottom right of the API Collection page to view the progress.<br>

    <figure><img src="../../.gitbook/assets/image (1055).png" alt=""><figcaption></figcaption></figure>

**Process API Collection Automatically**

* After creating an automated task, the system will automatically process eligible API collection requests according to the rules. Please refer to "Auto-Collection" below for details.

#### Auto-Collection

Users can create automated tasks, and the system will automatically trigger and filter eligible sub-addresses for collection without manual intervention. To learn more about the automation features, please go to "Auto-Collection / Signature".

#### Collection Gas Fee Rule Description

To ensure transactions can be successfully submitted to the chain while accounting for fee model differences across various blockchain networks, Cregis adopts differentiated Gas (Gas Fee / Resource) deduction mechanisms for different networks. During the collection process, the system automatically detects whether the Gas (Gas Fee / Resource) is sufficient and performs top-ups automatically. The specific rules are as follows:

**Tron Network**

The Tron network utilizes a Resource Model (Bandwidth / Energy) rather than traditional Gas Fees. When a transaction occurs on the Tron network, Cregis will automatically consume resources in the following order:

* When performing Tron network native asset (TRX) collection:
  * Priority is given to consuming address resources (Bandwidth): If the sender's address has sufficient resources, address resources will be consumed first.
  * When Bandwidth is insufficient, TRX will be burned to offset resources (Bandwidth): If resources are insufficient, the system will burn TRX in the address and convert it into resources to complete the transaction.
* When performing Tron network token (such as USDT) collection:
  * Priority is given to consuming address resources (Bandwidth, Energy): If the sender's address has sufficient resources, address resources will be consumed first.
  * When resources are insufficient, Cregis will sponsor the resources: Cregis automatically replenishes the required resources to ensure the transaction can be completed normally. The sponsored resources will be deducted from the team account balance.
  * If the above methods still cannot meet the transaction requirements: The system will burn TRX in the address and convert it into resources to complete the transaction.

**Other Network Currency Collection**

* Priority is given to using the address Gas Fee: If the sender's address has a sufficient Gas Fee, the collection transaction can be performed directly.
* If the address Gas Fee is insufficient: The system will automatically top up the Gas Fee from the collection receiving address to the address being collected.
