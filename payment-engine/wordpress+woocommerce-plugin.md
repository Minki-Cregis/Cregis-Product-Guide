---
hidden: true
---

# WordPress+WooCommerce Plugin

## Introduction



**What is WordPress and WooCommerce?**

WordPress is one of the world's most popular content management systems. It's an open-source platform that allows anyone to create and manage websites without requiring extensive technical knowledge. WooCommerce is a free e-commerce plugin for WordPress that transforms your WordPress website into a fully functional online store. The key difference is that WordPress is the platform for creating websites in general while WooCommerce is specifically designed for e-commerce and runs on top of WordPress.&#x20;



**What is Cregis Payment for WooCommerce?**

Cregis Payment for WooCommerce is a plugin that integrates the Cregis cryptocurrency payment gateway with your WooCommerce store. This integration allows your customers to pay for products using popular cryptocurrencies including USDT, USDC, BTC, SOL, ETH, TRX and BNB.

Once installed and configured, the plugin automatically handles cryptocurrency payments, converts them to your preferred settlement currency, manages order statuses in real-time and provides a seamless checkout experience for your customers. The plugin also includes features for handling common cryptocurrency payment scenarios such as overpayments and partial payment.

No coding is required – Just simply install the plugin, enter your Cregis credentials and your store will be ready to accept cryptocurrency payments.



## Prerequisites



Before setting up Cregis Payment, ensure you have the following items ready:

* A WordPress website running version 5.0 or higher with WooCommerce plugin (version 3.0 or higher) installed and activated.
* You should have at least one product created in your WooCommerce store.
* A SSL certificate installed on your website to enable HTTPS, which is required for secure cryptocurrency transactions.
* A Cregis merchant account, which you can create by following the setup guide in the next section.



## Merchant Setup Guide



1. Download the Cregis portal from [https://support.cregis.com/getting-started/quickstart](https://support.cregis.com/getting-started/quickstart) and create your merchant account. Once you have access to the portal, complete your full account setup by following the step-by-step guide available at [https://support.cregis.com/payment-engine/create-payment-engine](https://support.cregis.com/payment-engine/create-payment-engine). This includes settlement wallet configuration, API credentials generation and selecting your supported cryptocurrencies.<br>
2.  A critical step is adding your e-commerce platform's server IP address to the Cregis portal's IP whitelist. Then navigate to Settings > IP Whitelist in the Cregis portal, add your server IP address and save the changes. Without proper IP whitelisting, API requests from your store will be rejected.<br>

    <figure><img src="../.gitbook/assets/image (1101).png" alt=""><figcaption></figcaption></figure>



## Install and Configure the Plugin



1.  Log in to your WordPress admin dashboard and navigate to Plugins > Add New. Search for "Cregis Payment for WooCommerce" and look for the plugin created by cregisproduct. Click Install Now, then Activate to complete the installation.<br>

    <figure><img src="../.gitbook/assets/image (1099).png" alt=""><figcaption></figcaption></figure>



2.  After installation, you'll see Cregis Payment in the left sidebar menu. Click on Cregis Payment > Settings to access the configuration page. You'll need to copy three pieces of information from your Cregis portal: the Base URL, Project ID and API Key. These can all be found in the Cregis portal under Settings. Enter these values in the plugin settings and click Save Changes.<br>

    <figure><img src="../.gitbook/assets/image (1102).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../.gitbook/assets/image (1103).png" alt=""><figcaption></figcaption></figure>



3. Once you've set up the required information, products sold on your e-commerce platform will automatically accept cryptocurrency payments.<br>
4.  The order amount is based on your WooCommerce store currency settings, which you can find at WooCommerce > Settings > Currency options > Currency. (Please make sure your currency is supported by our available currencies which you can find here: [https://developers.cregis.com/en/payment-engine-supported-currencies/](https://developers.cregis.com/en/payment-engine-supported-currencies/)).

    <figure><img src="../.gitbook/assets/image (1104).png" alt=""><figcaption></figcaption></figure>


5.  The product price is individually based on each product at Products > All Products > \[Select Product] > Sale price.

    <figure><img src="../.gitbook/assets/image (1105).png" alt=""><figcaption></figcaption></figure>


6. If your store currency is USD and the listed currency is a USD-pegged stablecoin, the exchange rate will be 1:1. Otherwise, the exchange rate between your product's listed price and the currency selected by the payer will be based on the real-time exchange rate from CoinMarketCap.<br>
7. The payer's email address is automatically collected during checkout and will be used to handle cases of overpayment and underpayment.<br>
8.  The available payment currencies for payers are determined by which cryptocurrencies you've activated in your Cregis portal.

    <figure><img src="../.gitbook/assets/image (1106).png" alt=""><figcaption></figcaption></figure>


9.  In Web3 payments, it's common to encounter overpayments or partial payment. You can configure tolerance levels in the plugin settings using percentages to control the upper and lower limits you'll accept. For example, if you set an underpayment tolerance of 2% and an overpayment tolerance of 5% on a $100 order, you'll accept payments between $98 and $105.

    <figure><img src="../.gitbook/assets/image (1107).png" alt=""><figcaption></figcaption></figure>


10. Each payment request has a valid time of 60 minutes by default. You can adjust this based on your needs, with a minimum of 10 minutes and a maximum of 1440 minutes (24 hours).

    <figure><img src="../.gitbook/assets/image (1108).png" alt=""><figcaption></figcaption></figure>



## Checkout Flow & Inventory Impact



1.  In the checkout page of your e-commerce platform, an additional payment option called "Cregis Payment" will be available in the Payment options section. The payer can select this option and click Place Order. Please note that if product quantity is configured in inventory (Products > All Products > Select one product > Product data section > Inventory > Quantity), it will be deducted automatically based on the quantity in the cart when the payer clicks the "Place Order" button.

    <figure><img src="../.gitbook/assets/image (1110).png" alt=""><figcaption></figcaption></figure>



2. The checkout page is an industry-standard interface for accepting cryptocurrency payments. The payer can select their preferred cryptocurrency and complete the payment following the on-screen instructions. For a detailed step-by-step flow of the checkout process, you can refer to the checkout product manual at [https://support.cregis.com/payment-engine/payment-link-checkout-page](https://support.cregis.com/payment-engine/payment-link-checkout-page).\
   ![](<../.gitbook/assets/image (1111).png>)<br>
3. When payment is done in checkout page, it will be redirected to your order status page. Please note that there will be a few status according to different payment status. Below is the table you can refer to.

<table><thead><tr><th width="153.4140625">Payment Status</th><th width="130.03125">Order Status</th><th>Followup Action</th></tr></thead><tbody><tr><td>Paid in Full</td><td>Completed</td><td>No action required.</td></tr><tr><td>Underpaid</td><td>On hold</td><td>Payers will see an alert on the order status page and receive an email notification to complete the additional payment within 7 days. For more information: <a href="https://support.cregis.com/payment-engine/introduction#additional-payment-flow">https://support.cregis.com/payment-engine/introduction#additional-payment-flow </a></td></tr><tr><td>Overpaid</td><td>On hold</td><td>Payers will see an alert on the order status page and receive an email notification to request a partial refund within 7 days. For more information: <a href="https://support.cregis.com/payment-engine/introduction#partial-refund-process">https://support.cregis.com/payment-engine/introduction#partial-refund-process</a></td></tr><tr><td>Payment Timeout</td><td>Completed</td><td>No action required.</td></tr></tbody></table>

<figure><img src="../.gitbook/assets/image (1112).png" alt=""><figcaption></figcaption></figure>



4. Inventory will be automatically restocked if full refund is completed by payer or the payer does not complete the payment within valid time.

