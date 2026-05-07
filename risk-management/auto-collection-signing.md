# Auto-Collection/Signing

## What is Auto-Collection/ Signing?

This automated feature allows users to perform automatic fund collection and transaction signing based on preset rules, eliminating the need for manual monitoring by the enterprise. Once the rules are set, the system can operate 24/7 according to the configured rules, significantly reducing manual intervention. For example, while enterprises previously had to manually collect funds daily, with this automated feature, users can set intervals for automatic fund collection. Additionally, collection can be triggered when a specific cryptocurrency reaches a certain amount. Currently, the auto-signing feature is limited to API withdrawals and is only available for single-signature wallets. Furthermore, all these automated functions are performed locally, requiring no custodial sharding actions. Users only need to stay online to execute them, ensuring system security while greatly improving operational efficiency for businesses requiring frequent transactions.<br>

<figure><img src="../.gitbook/assets/image (828).png" alt=""><figcaption></figcaption></figure>

## Pricing and Activation Process

* Currently, the automated feature is only available to monthly subscription users and requires an additional payment of USD $500 per month. To activate, go to the account interface below and click "Activate."

<figure><img src="../.gitbook/assets/image (401).png" alt=""><figcaption></figcaption></figure>

* After clicking, a window will pop up where users can select the desired number of months and press "Submit."

<figure><img src="../.gitbook/assets/image (405).png" alt=""><figcaption></figcaption></figure>

* After submitting the order, you can proceed with payment immediately. Once the payment is successful, the feature will be activated.

<figure><img src="../.gitbook/assets/image (404).png" alt=""><figcaption></figcaption></figure>

## User Manual

<mark style="color:green;">**Before proceeding, please ensure that the automation feature has been activated.**</mark>

1\. Navigate to the automated feature page and click "Create Rule."

<figure><img src="../.gitbook/assets/image (826).png" alt=""><figcaption></figcaption></figure>

2\. Create an Auto-collection Rule

After clicking "Create Rule," a sidebar will pop up to begin configuration.

<figure><img src="../.gitbook/assets/image (821).png" alt=""><figcaption></figcaption></figure>

**Basic Settings**&#x20;

When creating a rule, first set the name and type. After selecting the "Auto-collection" type, a section will pop up requiring the selection of the collection type and WaaS project.<br>

<figure><img src="../.gitbook/assets/image (829).png" alt=""><figcaption></figcaption></figure>

Collection types include System Collection and API Collection. System Collection automatically collects funds from sub-addresses that meet the rules you set. API Collection processes collection requests initiated via API based on the rules you configure.

<figure><img src="../.gitbook/assets/image (830).png" alt="" width="305"><figcaption></figcaption></figure>

\
\
**Trigger Conditions**

Trigger rules require setting the cryptocurrency, collection time, and receiving address conditions.

*   Cryptocurrency \
    Each rule can only define one type of cryptocurrency. When adding, the system will display the available cryptocurrencies pre-configured in the wallet of the selected API project. Once the cryptocurrency is selected, you must set the amount that will trigger Auto-Collection. You can specify both "greater than" and "less than" conditions. For example, to trigger collection between $100 and $200, set "greater than or equal to 100" and "less than or equal to 200." \
    <mark style="color:green;">**Please note, if the conditions are not logically valid, the rule cannot be created. For example, setting "less than or equal to 50" and "greater than or equal to 51" will not be allowed.**</mark><br>

    <figure><img src="../.gitbook/assets/image (831).png" alt="" width="296"><figcaption></figcaption></figure>
*   Execution Actions \
    Users can choose to execute Auto-Collection either at regular intervals or at a specific time each day. <mark style="color:green;">**The time is currently based on UTC+8.**</mark><br>

    <figure><img src="../.gitbook/assets/image (832).png" alt=""><figcaption></figcaption></figure>
* Receiving Address \
  The receiving address currently only supports addresses from the wallet of the selected project. The system will automatically set the default receiving address of that wallet.

<figure><img src="../.gitbook/assets/image (408).png" alt="" width="300"><figcaption></figcaption></figure>

*   After completion, click "Submit." Identity verification is required after submission. The rule is created once verification is successful.<br>

    <figure><img src="../.gitbook/assets/image (833).png" alt=""><figcaption></figcaption></figure>
*   After creation, the rule must be enabled to take effect. Enabling requires the current device to have the wallet shard imported and password and Google two-factor authentication. The feature starts officially after successful verification.<br>

    <figure><img src="../.gitbook/assets/image (835).png" alt=""><figcaption></figcaption></figure>
*   After successful collection, go to the project address page, where "Auto-collection" will be displayed. **Note: The client must remain online during auto-collection; otherwise, the process will be interrupted.**

    <figure><img src="../.gitbook/assets/image (837).png" alt=""><figcaption></figcaption></figure>

3\. Create an Auto-Signing Rule

After clicking "Create Rule," a sidebar will pop up to begin configuration.<br>

<figure><img src="../.gitbook/assets/image (838).png" alt=""><figcaption></figcaption></figure>

**Basic Settings**&#x20;

When creating a rule, first set the name and type. After selecting the "Auto Signing" type, a section will pop up requiring the selection of the withdrawal type and withdrawal wallet. <mark style="color:green;">**Please note that only single-signature wallets are supported, and the default payment address will be used for signing and withdrawals.**</mark><br>

<figure><img src="../.gitbook/assets/image (839).png" alt=""><figcaption></figcaption></figure>

**Trigger Conditions**

The trigger conditions require setting cryptocurrency, withdrawal type, and execution action.

* Cryptocurrency

Only one cryptocurrency can be set per rule. When adding, the system will display the currencies already set in the selected withdrawal wallet. After setting the currency, specify the amount that triggers auto-signing. Both "greater than" and "less than" conditions can be set simultaneously. For example, to set $100–$200, set "greater than or equal to 100" and "less than or equal to 200."

<mark style="color:green;">**Please note, if the conditions are illogical, the rule cannot be created. For example, setting "less than or equal to 50" and "greater than or equal to 51" will be rejected.**</mark><br>

<figure><img src="../.gitbook/assets/image (841).png" alt="" width="293"><figcaption></figcaption></figure>

* Withdrawal Type \
  Since only API withdrawals are currently supported, this section requires selecting the API for withdrawals.

<figure><img src="../.gitbook/assets/image (842).png" alt="" width="294"><figcaption></figcaption></figure>

* Execution Actions \
  Scheduled signing can be configured here. Additionally, users need to set the interval (in minutes) for signing. If multiple transactions are triggered, they will be bundled on-chain, which may save gas fees on certain chains. The custom execution time is based on the local time of the device on which the automatic collection task is currently enabled.\
  **Note: If members in different time zones enable the same rule at different times, the system will trigger the rule based on each operator's local time zone, which may result in multiple collection executions within the same period.**

<figure><img src="../.gitbook/assets/image (411).png" alt="" width="278"><figcaption></figcaption></figure>

* After completion, click "Submit." Identity verification is required after submission. The rule is created once verification is successful.



* After creating the rule, you must enable it for it to take effect. During activation, you will need to enter your password and complete Google two-factor authentication (2FA). Once verification is successful, the rule will be officially active and ready for use.

<figure><img src="../.gitbook/assets/image (414).png" alt=""><figcaption></figcaption></figure>

* After you enable the rule, you can go to Team activity page, where the status will display "Operating Auto Sign" <mark style="color:green;">**Please note that you must remain online during the Auto-Signing process; otherwise, it will be interrupted.**</mark>

<figure><img src="../.gitbook/assets/image (415).png" alt=""><figcaption></figcaption></figure>

4\. Edit and Delete Automation Rules

* Edit Rules

Established rules can be edited in the rule configuration page. Before editing, you must first disable the rule, and identity verification is required when disabling the rule.

<figure><img src="../.gitbook/assets/image (844).png" alt=""><figcaption></figcaption></figure>

* Delete Rules \
  Established rules can be deleted from the rule configuration page. Before deleting, the rule must first be disabled, and identity verification will be required during the disabling process.

<figure><img src="../.gitbook/assets/image (845).png" alt=""><figcaption></figcaption></figure>

5\. View Automation Logs

In the execution logs, you can track the activity of each rule, including the date, time, operator, and action taken.

<figure><img src="../.gitbook/assets/image (846).png" alt=""><figcaption></figcaption></figure>

On this page, users can also filter the logs by operation date, operator, or log type.

<figure><img src="../.gitbook/assets/image (847).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (848).png" alt=""><figcaption></figcaption></figure>

The search bar also supports searching for related records using the rule name or ID.

<figure><img src="../.gitbook/assets/image (849).png" alt=""><figcaption></figcaption></figure>

6\. Triggering Auto-Collection

When the conditions of an Auto-Collection rule are met, the system will automatically execute the collection. Users can check the details of the Auto-Collection on the project address page.

<figure><img src="../.gitbook/assets/image (850).png" alt=""><figcaption></figcaption></figure>

* The details will show the runtime, start time, number of collections, and total amount collected. Additionally, the transaction history will list each collection.

<figure><img src="../.gitbook/assets/image (851).png" alt=""><figcaption></figcaption></figure>

* If there are insufficient gas fees, the Auto-Collection will pause, and a prompt will appear notifying the user to top up. The user can directly click "Recharge" on this screen and recharge using the provided address or QR code. After recharging, the system will resume the action at the next trigger point.

<figure><img src="../.gitbook/assets/image (852).png" alt=""><figcaption></figcaption></figure>

7\. Triggering Auto-Signing

* When the conditions for an auto-signing rule are met, the system will automatically perform the signing. Users can view the signing details in the collaboration section, and an "Auto-Signing in Progress" icon will appear in the lower-right corner.

<figure><img src="../.gitbook/assets/image (422).png" alt=""><figcaption></figcaption></figure>

* The details will show the runtime, start time, the number of signed transactions, total amount, and the gas fees used for signing. The transaction history will also list each signed transaction. If there are insufficient gas fees, the auto-signing process will be paused, and a prompt will notify you to top up. You can top up directly from this screen by clicking "Top Up," and using the address and QR code provided. Once the top-up is complete, the action will resume at the next trigger point.

<figure><img src="../.gitbook/assets/image (660).png" alt=""><figcaption></figcaption></figure>



## Real-World Scenarios

The actual setup should be tailored to the user's specific needs. Below are examples of how Auto-Collection/Auto-Signing can be configured in various scenarios:

**Scenario 1: I want to collect USDT from the project's sub-addresses on a daily basis.**

In this case, as long as there is USDT in the project's addresses, it will trigger the Auto-Collection rule. The user only needs to set the cryptocurrency (USDT) and customize the daily collection time, such as at 12:00 PM each day.

<figure><img src="../.gitbook/assets/image (423).png" alt="" width="295"><figcaption></figcaption></figure>

**Scenario 2: Automatically sign withdrawals under USDT $100 on weekends.**

In this case, you need to set cryptocurrency (USDT), the specific days for auto-signing (weekends), and the interval between each signing. For example, you can specify that the system checks every 30 minutes on Saturdays and Sundays for any withdrawals under $100 and signs them automatically.

<figure><img src="../.gitbook/assets/image (424).png" alt="" width="300"><figcaption></figcaption></figure>
