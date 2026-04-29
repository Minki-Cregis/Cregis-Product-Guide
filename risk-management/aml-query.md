# AML Query

## 1. What is AML Query?

Cregis AML is a risk management feature that helps users to identify, control and mitigate on-chain risks and is implemented through integration with Elliptic, a renowned crypto risk control service provider. Cregis AML supports Know Your Address (KYA) and Know Your Transaction (KYT) analyses and allows users to run manual queries and auto queries. Users may choose suitable features and methods based on their business requirements and manage on-chain transaction risks in a more efficient way.

Cregis AML function is available to all users and is charged based on the selected service provider and the number of queries. Subscribed users enjoy up to a 50% discount on query fees, and Business and Enterprise users also receive a certain number of free queries each month.

Please be advised that this service is provided by Cregis in partnership with Elliptic and Regtank. Under no circumstances shall Cregis or its partners be held responsible for any actual or potential legal or regulatory violations identified during the use of the service. You should be aware of risks linked to transactions, and exercise caution and independent judgment when making transactions.

## 2. Service Provider Introduction

Currently, Cregis AML has two partner service providers for risk control services, Elliptic and Regtank. Different service providers have different methods for risk assessment, support different blockchain networks, and charge different fees for queries. We suggest users select appropriate service providers that best meet their needs.

### 2.1. Elliptic

Elliptic detects the source and destination of on-chain funds, and assesses the level of association of the funds to wallet addresses with high money laundering risks and sanctioned addresses. It calculates risk scores of addresses or transactions based on the proportion of risky funds. The query fee for Elliptic is 2 USD per query, regardless of query subject or method. Subscribed users enjoy a certain discount on query fees.Elliptic's holistic query supports 49 blockchain networks. Here is a list of networks supported by Elliptic.

| Algorand            | Aptos       | Arbitrum          | Avalanche   | Base        | Binance Chain |
| ------------------- | ----------- | ----------------- | ----------- | ----------- | ------------- |
| Binance Smart Chain | Bitcoin     | Bittensor         | Cardano     | Celo        | Codex         |
| Core Chain          | Cosmos      | Crypto.com        | Dogecoin    | dYdX        | Ethereum      |
| Ethereum Classic    | Filecoin    | Fantom            | Flare       | Gnosis      | HAQQ          |
| Hedera              | Injective   | Internet Computer | Linea       | Litecoin    | Mantra        |
| MobileCoin          | Near        | Nillion           | Optimism    | Polkadot    | Polygon       |
| Ripple              | Sei         | Solana            | Stellar     | Sui         | Tezos         |
| TON                 | Tron        | Unichain          | Worldcoin   | XDC         | Zilliqa       |
| zkSync              | <p><br></p> | <p><br></p>       | <p><br></p> | <p><br></p> | <p><br></p>   |

### 2.2. Regtank

Regtank leverages on-chain data analysis and a risk labeling system to provide comprehensive assessments of wallets, transactions, and VASPs, displays entity information and risk labels, and identifies source and destination of funds as a supplement. The service fee for Regtank is 0.3 USD per query, regardless of query subject or method. Subscribed users enjoy a certain discount on query fees.Regtank supports the following 18 blockchain networks.

| Arbitrumone | Avalanche | Base     | Bitcoin  | Bitcoincash | Blast    |
| ----------- | --------- | -------- | -------- | ----------- | -------- |
| BSC         | Dash      | Dogecoin | Ethereum | Litecoin    | Optimism |
| Polygon     | Ripple    | Solana   | Tezos    | Ton         | Tron     |

## 3. Feature Description

Cregis AML provides two features, manual query and auto query, to meet users' needs under different scenarios.

### 3.1. Manual Query

Manual query enables users to conduct Know Your Address (KYA) and Know Your Transaction (KYT) analyses. Users are able to initiate an AML query on a wallet address or transaction, select a service provider to complete the query, and take appropriate risk control actions based on the query result.

To initiate a manual KYA query, users need to input the wallet address to be evaluated and the network it belongs to. Cregis AML then recognizes the entity associated with the target address. It also screens the source and destination of its fund, traces fund inflows and outflows, identifies the addresses and entities that have interacted with the targeted address, and analyzes their risk categories and characteristics. Source and destination risk exposure are estimated based on these analyses, and risk scores for source and destination of funds are calculated accordingly. The final risk score for the address is determined following the highest risk principle.

To initiate a manual KYT query, users need to select the direction of the query (incoming or outgoing), and input the network, receiving address and transaction hash of the transaction to be screened. Cregis AML will trace the source or destination of the funds involved in the transaction based on the user's selected direction, recognize entities linked to the funds and their risk profiles and characteristics, and calculate risk score for the transaction accordingly.

**User Manual**

Before using the AML query function, please ensure that you are a subscribed user. For subscription steps, please refer to [this page.](../account-management/images-and-media/manage-your-pricing-plan-old.md)

Navigate to the AML Query Page and click "<mark style="color:green;">**New Query**</mark>", or click the icon <img src="../.gitbook/assets/image (400).png" alt="" data-size="line">next to address on the transaction detail page.

<div><figure><img src="../.gitbook/assets/image (236).png" alt=""><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/image (238).png" alt=""><figcaption></figcaption></figure></div>

First, select the query type. For transaction queries, you need to enter the direction, network, recipient address, transaction hash, and service provider. For address queries, enter the network, address, and provider, and input the address you wish to query.

<figure><img src="../.gitbook/assets/image (797).png" alt=""><figcaption></figcaption></figure>

Please note that different service providers have varying fees and supported networks. You can click "Compare Service Providers" to view more details.

<figure><img src="../.gitbook/assets/image (798).png" alt=""><figcaption></figcaption></figure>

After clicking "View", the system will display a reminder message.

<figure><img src="../.gitbook/assets/image (392).png" alt=""><figcaption></figcaption></figure>

Then, you will need to enter your transaction password to complete verification.

<figure><img src="../.gitbook/assets/image (393).png" alt=""><figcaption></figcaption></figure>

After verification is completed, you can view the query results.

<figure><img src="../.gitbook/assets/image (394).png" alt=""><figcaption></figcaption></figure>

You may also check the details in record page including source risk score and destination risk score.

<figure><img src="../.gitbook/assets/image (230).png" alt=""><figcaption></figcaption></figure>

### 3.2. Auto Query

With auto query, Cregis AML helps users screen their API incoming transactions based on predefined rules, conduct risk analyses for transactions they care about most, and apply risk controls according to query results. Users need to create and manage their rules on the desktop application, while query results can be seen on both desktop applications and mobile applications.

To start auto query, users have to create query rule(s):

* Set up triggered rules which specify projects, tokens and amounts for transaction monitoring. Users may create multiple rules, but can only create one rule for each project. Within each rule, different trigger amounts can be set for different tokens.
* Define a specific risk control threshold based on business needs and risk preferences. Pick a number between 0 and 10.0 as the threshold, and Cregis AML will flag a transaction as dangerous when its risk score is higher than the threshold.
* Pick one or more risk alert recipient. Cregis AML will send risk alerts to assigned recipient(s) when it identifies a dangerous transaction.

When a rule is configured and enabled, Cregis AML will automatically conduct Know Your Transaction analysis on incoming transactions that trigger the rule. Then Cregis AML assesses whether a transaction is dangerous according to the risk threshold in the rule it triggered. When a dangerous transaction is identified, Cregis AML will disable the receiving address, and send risk alerts to assigned alert recipient. If a project/address is disabled, Cregis AML will no longer screen any incoming transactions of the project/address until it's manually enabled.

When a dangerous transaction is identified, Cregis AML disables the incoming address, stops API callback and funds collection of the address, and sends risk alerts to assigned alert recipients. Users who receive a risk alert can proceed to review query details to learn about risk specifics. If the risk is within the acceptable range, users may manually push a callback and enable the address.

**User Manual of setting up automatic AML queries**

First, navigate to the following page and click "Create."

<figure><img src="../.gitbook/assets/image (231).png" alt=""><figcaption></figcaption></figure>

After clicking, you can begin creating a rule

<figure><img src="../.gitbook/assets/image (232).png" alt=""><figcaption></figcaption></figure>

* Rule Name: Name your rule
* API Project: Select the project whose transactions you want to monitor. Please note that only one rule can be applied to a project.
* Token: Choose the cryptocurrency and set the minimum amount that will trigger an automatic AML query

<figure><img src="../.gitbook/assets/image (233).png" alt=""><figcaption></figcaption></figure>

* Service Provider: Select the service provider you wish to use for the query.
* Risk Classification Criteria: Can be set between 0.0 (Safe) - 10.0 (Extremely Risky). When a transaction's risk score exceeds your set threshold, it will be flagged as a risky transaction, triggering alert notifications and automatically disabling the project address.
* Alert Recipients: Designate team members to receive risk alerts

After completing the settings, click "Submit" and complete identity verification to finalize the creation process. The rule must be enabled after successful creation before it becomes active.

All rule activities (creation, editing, enabling, and deletion) are logged and can be viewed in the log page.

<figure><img src="../.gitbook/assets/image (234).png" alt=""><figcaption></figcaption></figure>

## 4. Query Results

### 4.1. Address Query (KYA)

The results of manual query include risk score, risk level, entity associated with the address and its label, and query details of fund source and fund destination.

1. **Risk Score & Risk Level**

The risk score of an address ranges from 0.0 to 10.0, and a higher score indicates a higher risk level. A risk score of 0 means that the relative risk is minimal, while a risk score of 10.0 signals an extremely high risk. Since each service provider has its own scoring mechanism, query results are categorized based on the risk classification methods recommended by the service provider.Please note that the following risk classification methods are recommended by the service provider based on general scenarios, and they may not be suitable for users with specific risk control requirements. To ensure the security of funds and operations, users are advised to account for their own needs and circumstances and assess the risk profile of an address or transaction based on the risk score and query details.The correspondence between risk scores and risk levels recommended by Elliptic is as follows.

| **Range**   | **Risk Levels**   |
| ----------- | ----------------- |
| \[0,2.5)    | Low/Safe          |
| \[2.5,7.5)  | Medium/Suspicious |
| \[7.5,10.0] | High/Dangerous    |

The correspondence between risk scores and risk levels recommended by Regtank is as follows.

| **Range**  | **Risk Levels**   |
| ---------- | ----------------- |
| \[0,3.0]   | Low/Safe          |
| (3.0,7.0]  | Medium/Suspicious |
| (7.0,10.0] | High/Dangerous    |

Regtank takes a different way to label and categorize addresses and calculate risk scores than Elliptic. Therefore, a significant number of addresses, particularly those belonging to Exchanges and commercial wallets, may be flagged as suspicious when using Regtank for risk assessment. In practice, addresses with a score below 6 are generally considered to have lower risk. Users are advised to review the query details and make their own judgment based on their risk appetite.

2. **Associated Entity & Label**

Associated entity refers to the name of the corporation, organization, project or other entity that owns the target address. Entity label is a tag applied by the service provider that reflects the category or risk feature of the target address or associated entity, such as Exchange, Bank, Mixing Service, etc.

Associated entity and label help users to have a complete view on the risk profile of the target address. Cregis AML utilizes address label database to tag target addresses. Please refer to Appendix B or the lists of labels provided by Elliptic. When an address belongs to a self-custody wallet or individual wallet, or when the information about the associated entity is not included in the service provider's database, the associated entity and label will be displayed as unknown.

3. **Query Details**

Query details include information for fund source and destination. Cregis AML provides risk scores and risk-linked entities for both source and destination. Users can further review the risk category, contribution value, and contribution percentage of each risk-linked entity.

* Source/Destination Risk Score\
  Source/Destination risk scores are also assigned on a scale of 0.0-10.0. Higher risk scores indicate larger risks. The overall risk score of an address equals the higher value of source and destination risk scores.
* Risk-linked Entity\
  From the perspective of source risks, a risk-linked entity is an entity labelled as risky by Cregis AML that has sent funds to the address of interest. From the perspective of destination risks, a risk-linked entity is an entity labelled as risky by Cregis AML that has received funds from the address of interest. A risk-lined entity is usually an enterprise, an organization or a group. An entity that cannot be identified is shown as Unknown. Users can also review the details of risk-lined entities, including:
  * Risk Category\
    The risk category is the type of risk an entity is linked to, such as Scam, Thief, Dark Service, etc. Cregis AML utilizes the address label database of our partner to determine the risk category of an entity. A summary of risk categories and descriptions can be found in the appendix.
  * Contribution Value\
    From the perspective of source risks, contribution value refers to the amount of fund inflows from a risk-linked entity to the address of interest, priced in the US dollar. From the perspective of destination risks, contribution value refers to the amount of fund outflows from the address of interest to a risk-linked entity, priced in the US dollar.
  * Contribution Percentage\
    The contribution percentage is the incoming/outgoing funds of a risk-linked entity as a proportion to the total incoming/outgoing funds, in percentage terms.

### 4.2. Transaction Query (KYT)

For transactions that trigger auto queries, Cregis AML provides risk scores and query details.

1. **Risk Score**

The risk score ranges from 0.0 to 10.0.&#x20;

The risk score calculated by Elliptic is directly correlated with the contribution ratio of risky funds to the source of funds for the outgoing address. The higher the contribution ratio of risky funds, the higher the risk score. When multiple types of risks are detected, Elliptic adopts a Highest Risk Principle to calculate the risk score. The correspondence between the two is shown in the following table:

<table data-header-hidden><thead><tr><th width="204.6328125"></th><th></th><th></th><th></th><th></th><th></th><th></th></tr></thead><tbody><tr><td>Risk Score</td><td>0.0</td><td>1.0</td><td>2.5</td><td>5.0</td><td>7.5</td><td>10.0</td></tr><tr><td>Contribution Ratio of Risky Funds </td><td>＜1%</td><td>10%</td><td>25%</td><td>50%</td><td>75%</td><td>＞99%</td></tr></tbody></table>

2. **Query Detail**

Query details show risk-linked entities of the sending address of the target transaction, i.e., risky entities which have sent funds to the sending address. Users can review the risk category, contribution value and contribution percentage of each risk-linked entity.

* Risk Category\
  The risk category is the type of risk an entity is linked to, such as Scam, Thief, Dark Service, etc. Cregis AML utilizes the address label database of our partner to determine the risk category of an entity. A summary of risk categories and descriptions can be found in Appendix A.
* Contribution Value\
  The contribution value is the amount of fund inflows to the sending address from a risk-linked entity, priced in the US dollar.
* Contribution Percentage\
  The contribution percentage is the proportion of funds received from a risk-linked entity to total funds received in percentage terms.

## 5. Use Case

### **5.1. Pre-transaction Risk Control**

Pre-transaction risk control aims to identify, assess and control risks before making a transaction to avoid abnormal transactions caused by operational errors or malicious behaviors and prevent major financial losses. Users may conduct manual queries on receiving addresses before important transactions are made and learn about risk exposure. The risk exposure of a receiving address can be used as a preliminary risk indicator for the risk profile of the receiving address.

If the risk score of a receiving address is high, it is strongly recommended that users do not transact with it to avoid risks of financial loss as well as operational, legal and regulatory risks. If the risk score falls in the medium risk range, it is suggested that users should double check the entity of recipient and the security of receiving address by other means, and proceed with the transaction after the address is verified as safe.

### **5.2. Transaction Monitoring**

Transaction monitoring employs automated technologies to screen and monitor transactions at low latency, identify potential risks and suspicious behaviors, and ensure transaction compliance and asset security. An inflow of risky assets may increase the risk exposure of the receiving address, which is a common risk factor in crypto transactions. For users with a high frequency of payment collections and uncertain sources of funds, the auto query feature enables real-time monitoring of incoming transactions. Cregis AML helps to identify potential risks and isolate respective receiving addresses, thus preventing greater losses caused by a spread of risk.

When a transaction is labelled as dangerous, Cregis recommends that users check and learn about the risk level of the transaction in a timely manner. In most cases, users are advised not to use the receiving address to avoid a spread of risk to other addresses. If the risk is assessed as acceptable, users may manually enable the receiving address.

## 6. Limitation of AML Feature

**Cregis AML is NOT able to cover all risk factors.** \
Cregis AML tracks and identifies risks based on the risk database provided by crypto risk management service providers such as Elliptic. The database covers 50 networks and includes over 6.4 billion addresses, transaction records and relative risk information. However, due to the limited scope of the database and the lag of data updates, it is not possible for Cregis AML to record and label every risky address and suspicious fund flows, and thus not all risk factors are identified. Users should use the query results as a reference to risk identification and management, rather than a sole piece of definitive evidence.

**The results provided by Cregis AML are time-sensitive.** \
Cregis AML adopts a risk assessment model based on historical behaviors. Risk is identified if and only if the address involved in the fund flow has a history of suspicious activities and has been marked accordingly. If the risky activities of an address are not detected or an activity happens after the query is completed, these risks cannot be captured in the query result. Therefore, query results provided by Cregis AML are a holistic evaluation of the known risky activities associated with the query target when the query is made. The results may not be used to predict future risk profiles. When users initiate queries at different times, the results may be different.

## 7. FAQ

* **Why did my query fail? What should I do when it fails?**\
  A query failure is usually caused by insufficient team balance or an error in the third party server. If it's caused by insufficient team balance, you can top up and conduct a manual query to learn about the risk level of the address of interest.

<figure><img src="../.gitbook/assets/image (235).png" alt=""><figcaption></figcaption></figure>

* **Is there a charge for a failed query?**\
  No. Failed queries will not be charged.
* **Why is my manual query results page showing no risk score or query details?**\
  This indicates that there is no record of any risky activities of the target address in the risk database. The target address might just be created and has no transaction records, and it's also possible that there are no records of fund interactions between the target address and flagged addresses in the database. Cregis AML labels such addresses as safe based on their historical records. However, users need to consider other risks such as scams and phishing attacks.
* **Why is my auto query results page showing no results?**\
  Reasons for empty results include: 1) information about this transaction has not been included in the database; 2) our database does not contain any risk information related to the source of funds for the queried transaction. In the second case, the transaction can usually be viewed as a safe one, but it is not possible to rule out all potential risks.
* **Why are there details for risk-linked entities while the risk score is 0.0?**\
  It means that the total amount of funds associated with all risk-linked entities accounts for less than 1% of total funds of the target address. Since the proportion of risky funds is very low, the risk score is determined to be 0.0.
* **Why is the contribution value of a risk-linked entity shown as 0.00 while the contribution percentage is positive?**\
  It happens when the inflow/outflow of funds of this entity is less than USD 0.01 and the total fund amount of the target address is less than USD 100. The proportion of risky funds to total funds exceeds 0.01%, and thus the contribution percentage is positive.
* **What does "Ignored Small Amounts" mean in the query detail part when I use Regtank as my service provider? Why do addresses under this category receive a risk score of 5?**\
  A: Regtank uses fund tracing analysis and node risk aggregation to calculate the risk score. As the tracing depth increases, the contribution of a node address to the target address or transaction generally decreases. When a node’s fund contribution falls below 0.01% and the address does not belong to any labeled entity in the Regtank database, Regtank stops evaluating its risk to save computing resources. Such addresses are categorized as "Ignored Small Amounts". In the query detail part, the fund contribution for "Ignored Small Amounts" represents the combined contribution of all such addresses. Since the risk of these addresses is unknown, Regtank assigns them a default risk score of 5.<br>

## 8. Appendix

### A. Elliptic-Risk category, description and example

| **Risk Category**                  | **Description**                                                                                                                                                                                                                                                                                            | **Example**                       |
| ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------- |
| Criminal Organisation              | A group of individuals engaged in organized crime                                                                                                                                                                                                                                                          | The Shadow Brokers                |
| Coin Swap Service                  | Coin swap service with fixed exchange rate, which usually doesn't require login or KYC                                                                                                                                                                                                                     | <p><br></p>                       |
| Credit Card Data Vendor            | Online card vendor that provides illegal credentials and other illegal personal financial information                                                                                                                                                                                                      | <p>JokerStash.store<br></p>       |
| Dark Forum                         | TOR-only online forum                                                                                                                                                                                                                                                                                      | DNM Avengers                      |
| Child Sexual Abuse Material Vendor | Vendor that provides child sexual abuse materials in exchange for crypto assets                                                                                                                                                                                                                            | <p><br></p>                       |
| Dark Market-Centralized            | TOR-only market that sells illegal goods and services via centralized infrastructure                                                                                                                                                                                                                       | Dream Market                      |
| Dark Market-Decentralized          | TOR-only market that sells illegal goods and services via decentralized infrastructure                                                                                                                                                                                                                     | Wall Street Market                |
| Dark Service                       | Illegal service, including hackers, wallets and web hosting services                                                                                                                                                                                                                                       | PinPays                           |
| Dark Vendor Shop                   | TOR-only individual vendor in the dark market that sells illegal goods and services                                                                                                                                                                                                                        | Euroarms                          |
| Extortion                          | Entity obtaining funds from individuals or groups by means of force or threat                                                                                                                                                                                                                              | Ashley Madison Extortion          |
| Far-Left/Far-Right Extremism       | <p>Entity which, (a) convicted of crimes directly related to far-left/ far-right extremist activities, or (b) identified and verified by multiple legal sources (with evidence) that has long been inciting violence, sexual abuse or other major crimes like far-left/ far-right extremist speech<br></p> | <p><br></p>                       |
| High Transaction Fee               | Entity involved in above-average transaction fees related to miners, which could be signs of losses or crimes                                                                                                                                                                                              | <p><br></p>                       |
| Known Criminal                     | Individual known to be engaged in illegal activities. Usually associated with criminal organizations.                                                                                                                                                                                                      | Ross Ulbricht and Carl Mark Force |
| Malware                            | Software aiming to impair or disable computers and computer systems                                                                                                                                                                                                                                        | <p>Trickbot<br></p>               |
| OFAC Sanctioned Entity             | Entity sanctioned by the Office of Foreign Assets Control (OFAC) of the US Department of the Treasury                                                                                                                                                                                                      | <p><br></p>                       |
| Phishing                           | A fraudulent activity in which the message sender attempts to deceive the recipient into leaking important personal information, transferring funds or installing malwares. The message sender usually impersonates a representative of a legal organization                                               | TRON Web Wallet Phishing          |
| Ponzi Scheme                       | A fraudulent activity in which original investors get rapidly paid off by funds from later investors so as to cultivate a belief in the success of a company that doesn't exist                                                                                                                            | <p><br></p>                       |
| Ransomware                         | Cryptovirology-based malware that threatens to publish victims' data or terminate access to the data unless a ransom is paid                                                                                                                                                                               | WannaCry 2.0                      |
| Scam                               | Any other type of fraudulent activities                                                                                                                                                                                                                                                                    | Prodeum                           |
| Terrorist Organization             | Organization involved in terrorism or related activities                                                                                                                                                                                                                                                   | ISIS                              |
| Thief                              | <p>Recipient of stolen funds<br></p>                                                                                                                                                                                                                                                                       | Stolen CoinSecure Funds           |

### B. Elliptic-Entity labels

| Label                              | Description                                                                                                                                                                                                                                                                                     | Label                    | Description                                                                                                                                                                                                                                                  |
| ---------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ATM                                | Automated teller machines (ATMs) that allow the purchase or sale of crypto assets using fiat currency                                                                                                                                                                                           | Forum                    | Online discussion forum                                                                                                                                                                                                                                      |
| <p>Authentication<br></p>          | A service that allows users to prove their unique identity when accessing specific websites without entering login credentials, thereby enhancing security.                                                                                                                                     | Gambling                 | Gambling service                                                                                                                                                                                                                                             |
| Bitcoin Faucet                     | Websites that give away free Bitcoin or reward users with Bitcoin for completing tasks.                                                                                                                                                                                                         | Hardware Wallet          | Physical hardware wallets used to store crypto assets                                                                                                                                                                                                        |
| Bridge                             | Contracts or services used to transfer assets from one blockchain to another                                                                                                                                                                                                                    | High Transaction Fee     | Entity involved in above-average transaction fees related to miners, which could be signs of losses or crimes                                                                                                                                                |
| Broker                             | Entities that represent clients in the buying and selling of crypto assets but do not maintain an order book                                                                                                                                                                                    | Hosting                  | Web hosting services                                                                                                                                                                                                                                         |
| Charity                            | Non-profit or charitable organizations that accept Bitcoin donations                                                                                                                                                                                                                            | Investment Syndicate     | Group investment providers, such as crypto asset risk operators or multi-level marketing schemes                                                                                                                                                             |
| Child Sexual Abuse Material Vendor | Vendor that provides child sexual abuse materials in exchange for crypto assets                                                                                                                                                                                                                 | Known Criminal           | Individuals known to be engaged in illegal activities. Usually associated with criminal organizations.                                                                                                                                                       |
| Coin Swap Service                  | Coin swap service with fixed exchange rate, which usually doesn't require login or KYC                                                                                                                                                                                                          | Law Enforcement          | Known law enforcement                                                                                                                                                                                                                                        |
| Credit Card Data Vendor            | Online carding shops that provide illegal credentials and other illicit personal financial information                                                                                                                                                                                          | Layer 2                  | Blockchain scaling solutions built on Layer 1 blockchains                                                                                                                                                                                                    |
| Crypto Exchange                    | Exchanges where customers can only trade crypto assets in exchange for other crypto assets                                                                                                                                                                                                      | Malware                  | Software aiming to impair or disable computers and computer systems                                                                                                                                                                                          |
| Criminal Organization              | A group of individuals engaged in organized crime                                                                                                                                                                                                                                               | Marijuana Vendor Shop    | Cannabis dispensaries registered in regulated jurisdictions                                                                                                                                                                                                  |
| Dark Forum                         | TOR-only online forum                                                                                                                                                                                                                                                                           | Merchant                 | Online legal sellers or vendors                                                                                                                                                                                                                              |
| Dark Market-Centralized            | TOR-only market that sells illegal goods and services via centralized infrastructure                                                                                                                                                                                                            | Microtransaction Service | Websites that facilitate microtransactions, such as freelance platforms or browser plugins that generate crypto assets                                                                                                                                       |
| Dark Market-Decentralized          | TOR-only market that sells illegal goods and services via decentralized infrastructure                                                                                                                                                                                                          | Mine                     | Newly minted crypto assets created as part of the mining/validation process                                                                                                                                                                                  |
| Dark Service                       | Illegal service, including hackers, wallets and web hosting services                                                                                                                                                                                                                            | Miner                    | Services for mining and generating new crypto assets                                                                                                                                                                                                         |
| Dark Vendor Shop                   | TOR-only individual vendor in the dark market that sells illegal goods and services                                                                                                                                                                                                             | Misc Service             | Various uncategorized services, vendors, or organizations                                                                                                                                                                                                    |
| Data                               | Vendors that provide data to end users                                                                                                                                                                                                                                                          | Mixer                    | Services used for privacy or money laundering purposes that allow crypto assets to be mixed or obfuscated to anonymize funds                                                                                                                                 |
| DeFi                               | Decentralized financial platform                                                                                                                                                                                                                                                                | News                     | Online news releasing service                                                                                                                                                                                                                                |
| Decentralized Exchange             | A decentralized service that provides cryptocurrency-to-cryptocurrency exchange                                                                                                                                                                                                                 | NFT Marketplace          | 让创作者能够向用户出售NFT的市场                                                                                                                                                                                                                                            |
| Entertainment                      | Vendors that provide streaming media, television, movies, and other entertainment services                                                                                                                                                                                                      | OFAC Sanctioned Entity   | Entity sanctioned by the Office of Foreign Assets Control (OFAC) of the US Department of the Treasury                                                                                                                                                        |
| Escrow                             | Vendors that provide escrow services for transactions between two parties                                                                                                                                                                                                                       | Outsourcing Provider     | Websites that facilitate freelance opportunities                                                                                                                                                                                                             |
| Exchange                           | Centralized service providers that offer fiat-to-crypto and crypto-to-crypto exchange services                                                                                                                                                                                                  | Payment Service Provdier | Online payment service providers that accept multiple payment methods                                                                                                                                                                                        |
| Extortion                          | Entity obtaining funds from individuals or groups by means of force or threat                                                                                                                                                                                                                   | Peer to Peer Exchange    | Platforms where individual buyers and sellers can exchange crypto assets for other assets                                                                                                                                                                    |
| Far-Left/Far-Right Extremism       | Entity which, (a) convicted of crimes directly related to far-left/ far-right extremist activities, or (b) identified and verified by multiple legal sources (with evidence) that has long been inciting violence, sexual abuse or other major crimes like far-left/ far-right extremist speech | Phishing                 | A fraudulent activity in which the message sender attempts to deceive the recipient into leaking important personal information, transferring funds or installing malwares. The message sender usually impersonates a representative of a legal organization |
| Financial Service                  | Financial service organizations that provide loans, bonds, derivatives, and other financial products                                                                                                                                                                                            | Research Chemicals       | Bulk chemical retailers for laboratory use only                                                                                                                                                                                                              |
| Political Campaign                 | Political campaign or organization                                                                                                                                                                                                                                                              | Scam                     | Any other type of fraudulent activities                                                                                                                                                                                                                      |
| Ponzi Scheme                       | A fraudulent activity in which original investors get rapidly paid off by funds from later investors so as to cultivate a belief in the success of a company that doesn't exist                                                                                                                 | Shielded                 | Shielded addresses use cryptographic techniques to conceal on-chain information such as the sender's address and transaction amount                                                                                                                          |
| Privacy Wallet                     | Cryptocurrency wallets that help users avoid blockchain deanonymization features                                                                                                                                                                                                                | Software Wallet          | Intangible software wallets used to store crypto assets                                                                                                                                                                                                      |
| Ransomware                         | Cryptovirology-based malware that threatens to publish victims' data or terminate access to the data unless a ransom is paid                                                                                                                                                                    | Terrorist Organization   | Organization involved in terrorism or related activities                                                                                                                                                                                                     |
| Reported Loss                      | Losses caused by disruptions or forks                                                                                                                                                                                                                                                           | User                     | A forum or social mediauser                                                                                                                                                                                                                                  |
| Thief                              | Recipient of stolen funds                                                                                                                                                                                                                                                                       | Validator                | Nodes responsible for executing transactions on the blockchain                                                                                                                                                                                               |
| Token                              | Representations of specific assets, utilities, intangible assets, or crypto assets                                                                                                                                                                                                              | Venture Capital          | Venture capital organizations that work with startups, early-stage companies, and emerging companies considered to have high growth potential                                                                                                                |
| Token Sale                         | Crowdfunding, presales, or other sales related to the launch of tokens or other crypto assets                                                                                                                                                                                                   | VPN Vendor               | Providers of Virtual Private Network (VPN) services                                                                                                                                                                                                          |
| Trading Platform                   | Providers of exchange software and services that do not operate exchanges                                                                                                                                                                                                                       | <p><br></p>              | <p><br></p>                                                                                                                                                                                                                                                  |

### C. Regtank-Entity labels

| Label                     | Description                                                                                                                           | Label                           | Description                                                                                                                                                  |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Exchange                  | Crypto Exchange                                                                                                                       | Wallet                          | Specific wallets, such as those used for advertising ICOs or company wallets                                                                                 |
| Donations                 | Addresses used by projects, companies, or non-profit associations to raise funds                                                      | Decentralized Servie            | Decentralized cryptocurrency platforms that are not exchanges, such as DeFi platforms and smart contracts                                                    |
| Mining Pool               | Addresses used by a group of pooled miners                                                                                            | Decentralized Exchange          | Decentralized Exchange                                                                                                                                       |
| Cloud Mining              | Addresses used for mining with remote computing power                                                                                 | Closed Exchange                 | Non-public exchange                                                                                                                                          |
| Token                     | Smart contract addresses representing the ERC20 standard on Ethereum or equivalent standards on other blockchains                     | Suspicious                      | Addresses associated with fraud reports that are unconfirmed or have not yet resulted in legal action                                                        |
| Service                   | Non-exchange entities belonging to centralized cryptocurrency platforms, such as payment processors, lending platforms, and merchants | Mixing Service                  | <p>Centralized platforms that help users mix their funds with those of other users<br></p>                                                                   |
| Airdrop                   | Addresses used to distribute free cryptocurrencies or tokens to other wallets                                                         | Scam                            | Addresses associated with fraud                                                                                                                              |
| ICO                       | Addresses used to raise funds for new cryptocurrency projects                                                                         | Hack                            | Addresses used to attack or exploit cryptocurrency platforms, resulting in platform fund losses due to the attack or exploitation                            |
| Gambling                  | Addresses used by crypto casinos                                                                                                      | Phishing                        | An activity in which the attacker steals private keys and other sensitive data by impersonating a trusted entity, resulting in financial loss for the victim |
| Darkweb                   | Addresses and entities associated with darknet activities, such as darknet markets, stolen funds, and similar illicit operations      | Community Reported Scam         | Fraud addresses reported by users in online forums or communities but not yet officially confirmed                                                           |
| Sanction List             | Addresses on the sanctions list of OFAC (the U.S. Office of Foreign Assets Control).                                                  | Ongoing Legal Action            | Addresses involved in ongoing litigation or cases under review                                                                                               |
| Terrorism                 | Addresses or entities associated with terrorist activities                                                                            | Cross-chain Bridge Protocol     | Entities that use smart contract technology to exchange different cryptocurrencies across different blockchains, including custodial wallet addresses        |
| Child Abuse               | Addresses associated with child exploitation                                                                                          | Unspent Output                  | Unspent funds on the blockchain that are available to be used in subsequent transactions                                                                     |
| Block Reward              | Rewards received by miners upon successfully mining new cryptocurrency                                                                | Payment Channel                 | Payment channels opened for using the Lightning Network                                                                                                      |
| Ignored Small Amounts     | The proportion of funds that is so small that it's ignored by the algorithm and not subjected to risk tracing.                        | Peeling Chain of Unknown Origin | Peeling chains with unknown source addresses                                                                                                                 |
| Maximum Exploration Depth | The algorithm reached its exploration limit and found no entity names                                                                 | Large Transaction               | <p>A transaction that has more than 200 inputs/outputs. Cautious review on the transaction is recommended<br></p>                                            |
| Mixing Pattern            | Decentralized function that allows users to quickly and efficiently mix their funds with those of other users                         | Secondary Coin Creation         | The creation of new ERC20 tokens                                                                                                                             |
| Secondary Coin Removal    | The burning of new ERC20 tokens.                                                                                                      | Bank                            | Addresses belonging to a bank                                                                                                                                |
