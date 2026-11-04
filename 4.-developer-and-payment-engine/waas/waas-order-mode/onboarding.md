---
description: >-
  This chapter walks you through creating a project, setting permissions, payout
  external verification, API integration and notification settings.
---

# Onboarding

1. Create Project (Recommend the business owner or an assigned representative complete the project creation)<br>
   1.  Create the project: if you have no project yet, create one from the WaaS landing page; if you already have WaaS project(s), click "Create Project" in the project dropdown list.

       <figure><img src="../../../.gitbook/assets/image (1217).png" alt=""><figcaption></figcaption></figure>

       <figure><img src="../../../.gitbook/assets/image (1218).png" alt=""><figcaption></figcaption></figure>


   2.  Enter the project name

       <figure><img src="../../../.gitbook/assets/image (1219).png" alt=""><figcaption></figcaption></figure>


   3.  Turn on the Deposit Method toggle and select Order Mode.

       <figure><img src="../../../.gitbook/assets/image (1220).png" alt=""><figcaption></figcaption></figure>


   4.  If you would like to use the Cregis built-in checkout page, we highly recommend creating the Merchant Name and Merchant Logo, so your customers can recognize you when they enter the checkout page. If these are left blank, the checkout page is still usable, but no name or logo is shown. You can also change them later in the Merchant Information page under Settings.

       <figure><img src="../../../.gitbook/assets/image (1221).png" alt=""><figcaption></figcaption></figure>

       <br>
   5.  If you would like to not only accept payments but also make payouts, you can turn on the Payout toggle and select the payout wallet. Please note that once this is enabled, the project can submit an API payout request. This API request is the step before wallet signing that completes the payout process.

       <figure><img src="../../../.gitbook/assets/image (1223).png" alt=""><figcaption></figcaption></figure>


   6.  Create and continue to the Receiving and Transfer page.

       <figure><img src="../../../.gitbook/assets/image (1224).png" alt=""><figcaption></figcaption></figure>


   7.  The last step is to set up your transfer address for receiving payments. For each payment currency you want to accept, select one of your transfer wallets and its wallet address. A payment currency only becomes available after you complete this currency setting here. You can change this later when you come back to this Receiving and Transfer page under Settings.

       <figure><img src="../../../.gitbook/assets/image (1225).png" alt=""><figcaption></figcaption></figure>


   8.  You can assign different roles to different team members by granting different permissions. Below are the permissions specific to WaaS Order Mode.\
       \
       \- Enable Refund & Payment Exception Transfer: Allow to proceed refund and payment exception transfer\
       \
       \- Edit Transfer Setting: Allow to configure the transfer wallet and wallet address\
       \
       For the common permissions used in both WaaS Order Mode and WaaS Sub-Address Mode, please check the [team role page](https://support.cregis.com/team/role).<br>

       <figure><img src="../../../.gitbook/assets/image (1226).png" alt=""><figcaption></figcaption></figure>


   9.  Payout External Verification: you could enable external verification for further security. For details, please check [here](https://support.cregis.com/api/api-manual/payout-external-verification).

       <figure><img src="../../../.gitbook/assets/image (1227).png" alt=""><figcaption></figcaption></figure>


2. API Integration (for designated development teams only)<br>
   1.  Get your credentials: go to the Developer page under Settings. You will find the Project ID, API Key and Base URL for integration. Apply the Project ID as the pid parameter in API requests; use the API Key to create the sign parameter by following [the signature guide](https://developers.cregis.com/en/waas-authentication/); and use Base URL + Path (e.g. https://t-abcdefgh.cregis.dev + /api/v1/create\_order) as the API request endpoint. Please note: DO NOT easily disclose the project API key to others, as it may lead to asset loss.

       <figure><img src="../../../.gitbook/assets/image (1228).png" alt=""><figcaption></figcaption></figure>


   2.  Add the calling IP to the whitelist: before calling the API, you must add the IP address of the device calling the API to the IP Whitelist for security. Otherwise, the API will return an error. You can configure this in "IP Whitelist" by clicking "Create Group", entering the IP address, clicking "Save", and then completing the authorization verification.

       <figure><img src="../../../.gitbook/assets/image (1229).png" alt=""><figcaption></figcaption></figure>


   3.  Start integrating: once everything is set up, the development team can use the Create Order request to create an order, retrieve the relevant information and present it to the payer to process the payment. For more information, see Page 3: Payer Interface, which explains how to present the information to the payer. The development team can also use Query Order to check historical orders and get the latest information for an order. In addition, the Cregis system provides real-time updates by sending callback messages across different order, refund and payment exception statuses.

       <figure><img src="../../../.gitbook/assets/image (1230).png" alt=""><figcaption></figcaption></figure>


3. Notification Settings<br>
   1.  Notification page: you can configure the project notification settings on the Notification page under Settings. There are 4 types of notifications:\
       \
       i. Callback Error (In-app): When a callback is not able to be sent to the callback URL\
       \
       ii. Enable / Disable Project (In-app + Email): When the merchant enables or disables the project in the Developer page under Settings\
       \
       iii. Reset API Key (In-app + Email): When the merchant clicks and confirms Reset API Key in the Developer page under Settings\
       \
       iv. Insufficient team balance to cover service charges (In-app + Email): When the total service charge is larger than the team balance\
       \
       v. Payment Exception Notification (Email): When a payment exception is received<br>

       <figure><img src="../../../.gitbook/assets/image (1231).png" alt=""><figcaption></figcaption></figure>


   2.  Enable or disable: you can turn the toggle on or off to enable or disable each notification.

       <figure><img src="../../../.gitbook/assets/image (1232).png" alt=""><figcaption></figcaption></figure>


   3.  Choose the receivers: you can also select the receivers by clicking "Edit" and ticking the assigned team members who should receive the notification.

       <figure><img src="../../../.gitbook/assets/image (1233).png" alt=""><figcaption></figcaption></figure>

       \
       \
       \
       <br>
