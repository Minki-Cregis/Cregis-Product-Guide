# Policy Engine

## What is a Policy Engine?

The Policy Engine is a comprehensive risk management tool in Cregis, offering flexible solutions for withdrawal management. It allows users to set detailed rules and automate actions to regulate withdrawal requests from team members, with future plans to support automatic signing and withdrawals for improved efficiency and reduced manual risks. Currently, it supports policy customization for transaction, payment request initiation, and API withdrawals, enabling users to tailor policies to their needs, such as limiting withdrawals to specific tokens or setting time restrictions. The Policy Engine also includes a daily log feature for monitoring and reviewing policy execution, ensuring transparency, tracking, and auditing of all actions to enhance risk management and safeguard assets.

## Creation Policy

1. ### Accessing the Policy Engine Page

Navigate to the Policy Engine page by selecting "Risk Control" > "Policy." To begin setting up a process, click "Start Creation"

<figure><img src="../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

2. ### Action Creation

Click the "+" to create a **policy**. First, name the **policy** and then select the corresponding type. The types are Manual Transfer and API Payout:

**Manual Transfer:** Transactions transferred via Cregis, including manual transfers from the wallet and manual transfers from addresses within the WaaS project.

**API Payout:** Transactions transferred via API, including all wallet payouts from wallets or sub-addresses made for WaaS projects.

<figure><img src="../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

After selecting the type, you can add rules. Please note: Users can set more than one rule for a wallet, and the relationship between the rules is "OR". You can configure trigger rules and actions based on your actual scenario. Finally, submit and verify to successfully create the policy.

<figure><img src="../.gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

## **Edit and Delete Policies**

You can find the options to edit and delete in the following location.

<div><figure><img src="../.gitbook/assets/image (49).png" alt=""><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure></div>

## **Trigger Rule Explanation**

**Operation Initiation Configuration**

The trigger conditions for rules vary depending on the **policy** type. Manual Transfer requires configuring members and withdrawal wallets, while API Payout requires configuring the WaaS project and the payout type.

<div><figure><img src="../.gitbook/assets/image (939).png" alt="" width="310"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/image (940).png" alt="" width="308"><figcaption></figcaption></figure></div>

**Operation Time**

Operation Time is used to restrict operations (Manual Transfer, Payout Transfer) for this **policy** type. Users can choose "All Day" or "Specified Time" as a condition. If specifying a time, start and end times must be set, and multiple time periods are supported.\
<mark style="color:green;">**Please note: This time is based on UTC+8.**</mark>

**Token**

In this field, users can select the token for the initiation, choosing either any token or a specific token.

* Amount Condition Explanation: Users can set limits for the selected sending currency based on a single transaction, daily, or monthly amount.

**Execution Action Explanation**\
We provide three types of execution actions for configuration. The following are the configurable execution actions:

**Reject:** The system automatically rejects the withdrawal.

<figure><img src="../.gitbook/assets/image (941).png" alt=""><figcaption></figcaption></figure>

**Approval:** Requires setting up an approval workflow, including defining approval nodes and signers.

<figure><img src="../.gitbook/assets/image (942).png" alt=""><figcaption></figcaption></figure>

**Signature:** Requires setting up signers.

<figure><img src="../.gitbook/assets/image (943).png" alt=""><figcaption></figcaption></figure>

## **Practical Usage Scenarios**

Actual settings should be based on the user's own needs. The following are some policy engine configuration scenarios.

**Scenario 1: I want to restrict Bitcoin withdrawals. All Bitcoin-related withdrawals must undergo approval, and the API service is not used. The trigger conditions and execution actions are as follows.**

**Trigger Condition Settings**

Select the specified token, Bitcoin, and set all transfer limits to trigger the condition when the amount is greater than or equal to 0.

<figure><img src="../.gitbook/assets/image (944).png" alt="" width="291"><figcaption></figcaption></figure>

**Execution Action Settings**

Select "Initiate Approval Process" as the execution action, and configure the corresponding approvers and signers.

<figure><img src="../.gitbook/assets/image (945).png" alt="" width="295"><figcaption></figcaption></figure>

**Scenario 2: Withdrawal requests are not allowed outside of working hours, for example, from 7 PM to 7 AM the next day.**

**Trigger Condition Settings**

Note that two separate time settings need to be configured here.

<figure><img src="../.gitbook/assets/image (946).png" alt="" width="289"><figcaption></figcaption></figure>

**Execution Action Settings**

Simply select "Reject".

<figure><img src="../.gitbook/assets/image (947).png" alt=""><figcaption></figcaption></figure>
