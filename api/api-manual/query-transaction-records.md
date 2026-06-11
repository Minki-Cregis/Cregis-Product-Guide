# Query Transaction Records

In WaaS projects, transaction history is used to view all business records related to fund flows under the current project, helping users track withdrawals, sub-address transactions, and collection records. Transaction history is mainly divided into the following three categories:

* Withdrawal History
* Transaction History
* Collection History

#### Withdrawal History

Withdrawal History is used to view withdrawal requests initiated via API. Depending on the source of the withdrawal, it is categorized into:

* Wallet Withdrawal: Refers to withdrawal request records initiated through the wallet withdrawal API.
* Sub-address Withdrawal: Refers to withdrawal request records initiated through the sub-address withdrawal API.

<figure><img src="../../.gitbook/assets/image (1050).png" alt=""><figcaption></figcaption></figure>

#### Transaction History

Transaction History is used to view transaction records related to the sub-addresses of the WaaS project. Including:

* Receive
* Send

Excluding:

* Collection-related transactions (Collection, Gas Fee Top-up)

Transaction History is categorized into:

* History: Displays transaction records in their final state (Successful, Failed, Canceled).
* In Progress: Displays transaction records that are currently still pending confirmation on the chain.

<figure><img src="../../.gitbook/assets/image (1051).png" alt=""><figcaption></figcaption></figure>

#### Collection History

Collection History is used to view transaction records related to sub-address collection in the WaaS project. Including:

* Collection (Manual Collection, Auto-Collection)
* Gas Fee Top-up

Collection History is categorized into:

* History: Displays collection transaction records in their final state (Successful, Failed, Canceled).
* In Progress: Displays collection transaction records that are currently still pending confirmation on the chain.

<figure><img src="../../.gitbook/assets/image (1052).png" alt=""><figcaption></figcaption></figure>
