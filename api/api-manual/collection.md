# Collection

Collection is used to actively aggregate assets from the sub-addresses of a WaaS project into a designated collection address. This facilitates unified management of fund balances, improves capital efficiency, and reduces the costs of managing dispersed assets. Currently, the following three collection methods are supported:

*   Manual Collection

    Manual collection supports the following two methods:

    * **Rule-based Collection**
      * Create a collection rule and manually initiate a collection task. The system automatically identifies sub-addresses that meet the rule conditions and transfers all eligible assets from those addresses to the specified destination address.
    * **Quick Collection**
      * Initiate a collection task directly without creating a collection rule. Users can manually select the asset and destination address. The system automatically identifies eligible sub-addresses based on the selected asset and transfers all eligible assets to the specified destination address. This method is ideal for temporary or one-time collection scenarios.
* API Collection
  * After initiating a collection request via API, it can be processed manually or handled automatically on the API Collection page. Users can specify the collection address and amount to precisely control collection behavior.
* Auto-Collection
  * After creating an automation rule, the system automatically initiates the collection without manual intervention. The system will automatically filter sub-addresses that meet the criteria according to the rule, and collect all eligible assets within those addresses into the designated receiving address.

## Manual Collection

Manual collection supports two methods: **Rule-based Collection** and **Quick Collection**. Users can choose the appropriate method based on their business requirements.

### **Method 1: Rule-based Collection**

Users can configure collection rules in advance and manually trigger collection tasks when needed. The system will filter sub-addresses that meet the criteria according to the rules for collection.

Navigation Path: WaaS → Collection → Rule Configuration

**Create a Collection Rule**

Click the "Add" button on the page to enter the creation page.

<figure><img src="../../.gitbook/assets/image (1187).png" alt=""><figcaption></figcaption></figure>

Configure collection rules, including Rule Name, Collection Cryptocurrency, Collection Amount, and Destination Address. The Collection Amount supports the following four modes:

* No Limit: Collects funds from all addresses. If an address balance is less than or equal to the minimum transfer amount, collection will not be performed.
* Greater Than or Equal To: Collects only from addresses with a balance greater than or equal to the specified amount.
* Less Than or Equal To: Collects only from addresses with a balance less than or equal to the specified amount.
* Amount Range: Collects only from addresses with a balance within the specified amount range.

<figure><img src="../../.gitbook/assets/image (1189).png" alt=""><figcaption></figcaption></figure>

Once configured, click Confirm to complete Google Authenticator verification. After successful verification, the rule is created.

**Initiate Collection**

After the rule is created, click Start in the rule list to initiate collection.

<figure><img src="../../.gitbook/assets/image (1190).png" alt=""><figcaption></figcaption></figure>

On the collection confirmation page, the system will automatically filter sub-addresses that meet the criteria based on the current rule, and display the estimated collection amount and number of transactions. After reviewing, click Confirm.

<figure><img src="../../.gitbook/assets/image (1191).png" alt=""><figcaption></figcaption></figure>

Enter your Transaction Password and click Confirm to begin collection.

<figure><img src="../../.gitbook/assets/image (1194).png" alt=""><figcaption></figcaption></figure>

Once initiated, you will automatically enter the collection progress page. You can subsequently view the detailed logs under Task History.

<figure><img src="../../.gitbook/assets/image (1195).png" alt=""><figcaption></figcaption></figure>

### **Method 2: Quick Collection**

Quick Collection allows you to initiate a collection task directly without creating a collection rule in advance. It is ideal for temporary or one-time collection scenarios.

Navigation: WaaS → Collection → Rule Configuration → Quick Collection

**Initiate a Quick Collection**

Click the "**Quick Collection"** button to open the **Collection Confirmation** page.

<figure><img src="../../.gitbook/assets/image (1182).png" alt=""><figcaption></figcaption></figure>

Configure the Collection Currency, Collection Amount, and Deposit Address. The collection amount supports the following four modes:

* No Limit: Collects funds from all addresses. If the address balance is less than or equal to the minimum sending amount, collection will not be performed.
* Greater Than or Equal To: Only collects addresses with a balance greater than or equal to the specified amount.
* Less Than or Equal To: Only collects addresses with a balance less than or equal to the specified amount.
* Amount Range: Only collects addresses with a balance within the specified amount range.

<figure><img src="../../.gitbook/assets/image (1183).png" alt=""><figcaption></figcaption></figure>

The system automatically filters eligible sub-addresses based on the selected asset and collection amount, and displays the estimated collectible amount and number of eligible addresses.Review the information and click "**Start Collection"**.

<figure><img src="../../.gitbook/assets/image (1184).png" alt=""><figcaption></figcaption></figure>

Enter your Transaction Password, then click "**Confirm"** to start the collection.

<figure><img src="../../.gitbook/assets/image (1185).png" alt=""><figcaption></figcaption></figure>

Once the collection starts, you will be automatically redirected to the **Collection Details** page. You can also monitor the task later on the **Task Record** page.

<figure><img src="../../.gitbook/assets/image (1186).png" alt=""><figcaption></figcaption></figure>

## API Collection

After the business system invokes the API collection, the system generates a pending collection task and displays it on the API Collection page. Collection can be triggered manually or via automated tasks when needed.

Navigation Path: WaaS Project → Collection → API Collection

### **Initiate an API Collection Request**

* Please go to the "[Developer Documentation](https://developer.cregis.com/quickstart)" to understand the detailed method for invoking API collection requests.

### **Process API Collection Manually**

* On the API Collection page, multiple collection requests can be selected in batches to be processed simultaneously (collect or reject).
*   If performing a batch collection operation, please filter by the specified currency first before operating. Since the on-chain processing mechanisms differ for different currencies, the system does not support cross-currency batch collection.<br>

    <figure><img src="../../.gitbook/assets/image (1053).png" alt=""><figcaption></figcaption></figure>
* After selecting the collection requests to be processed, click the "Collect" button to enter the Collection Confirmation page. Confirm and select the Gas Fee, then click the "Confirm" button.
*   Enter the transaction password, then click the "Confirm" button to start the collection.<br>

    <figure><img src="../../.gitbook/assets/image (1054).png" alt=""><figcaption></figcaption></figure>
*   Once the collection starts, you can click the collection progress button at the bottom right of the API Collection page to view the progress.<br>

    <figure><img src="../../.gitbook/assets/image (1055).png" alt=""><figcaption></figcaption></figure>

### **Process API Collection Automatically**

* After creating an automated task, the system will automatically process eligible API collection requests according to the rules. Please refer to "Auto-Collection" below for details.

## Auto-Collection

Users can create automated tasks, and the system will automatically trigger and filter eligible sub-addresses for collection without manual intervention. To learn more about the automation features, please go to "[Auto-Collection / Signature](../../risk-management/auto-collection-signing.md)".

## Collection Gas Fee Rule Description

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
