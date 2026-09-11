# Team Activity

## What is Team Collaboration?

Team collaboration is Cregis's transaction management and multi-person co-handling capability designed for enterprise teams. Through mechanisms such as approval and signing, enterprises can segregate transaction initiation, business approval, and transaction signing. Different roles participate together to complete transaction processing, thereby reducing single-point operational risks and establishing a more standardized, secure fund management workflow.

For example, an enterprise can configure the following workflow: Employee initiates transaction → Finance approves → Department Head approves → Signer signs → Transaction broadcast to the blockchain.

Through team collaboration, enterprises can assign different members to different business stages based on their internal fund management policies, achieving segregation of duties, multi-person re-checking, and audit logging.

Team collaboration is suitable for the following scenarios:

* **High-Value Transaction Approva**l: Large transfers require manager approval before execution.
* **Multi-Person Joint Fund Managemen**t: Transactions require multiple members to participate in confirmation or signing.
* **Segregation of Duties**: Business operators initiate transactions, finance personnel handle approvals, and signers perform signing.
* **Transaction Risk Control**: Initiated transactions trigger manual approval when specific conditions are met.
* **Enterprise Fund Management**: Establish standardized fund operation workflows through approval and signing mechanisms.

## Collaboration Workflow

Cregis team collaboration primarily revolves around transaction initiation, policy matching, approval, signing, and broadcasting to the blockchain.

Typical Transaction Workflow:

Initiate Transaction → Policy Matching → Approval → Signing → Broadcast to Blockchain

**1. Initiate Transaction**

Team members or business systems can initiate transactions based on their assigned permissions. Transactions can originate from different operational entry points, such as:

* Wallet / Sub-address
* WaaS API
* App Store

Once a transaction is initiated, Cregis determines whether it needs to enter the approval process based on the team's configured policies.

**2. Policy Matching**

The system matches enabled [policies](../../risk-management/policy-engine.md) based on transaction conditions.

* _Example:_ When a single transfer amount is $$ $\ge 100,000\text{ USDT}$ $$, approval is required.

If a transaction meets the policy conditions, it enters the corresponding approval workflow. If no policy is triggered, it proceeds directly to the signing stage. Whether approval is required depends entirely on the matched policy.

**3. Approval**

If a transaction triggers a policy, it undergoes approval sequentially according to the configured workflow:

* _Example:_ Employee initiates → Finance approves → Department Head approves

Approvers can view detailed transaction information and select either:

* Approve
* Reject

Once all approval nodes complete their review, the transaction proceeds to the signing stage. If any approval node rejects the transaction, execution stops immediately.

**4. Signing**

Upon approval, the transaction enters the signing stage. Members with signing permissions can sign the transaction. The specific members required to sign depend on the triggered policy or the wallet's signing rules. Once the signing criteria are met, Cregis submits the transaction to be broadcast onto the blockchain.

* Single-Sig: The transaction proceeds as soon as any single member specified by the policy completes the signature.
* Multi-Sig: Specified members participate in signing. The transaction proceeds only after the number of signatures reaches the threshold set for the wallet.

**5. Broadcast to Blockchain**

After signing is completed, the transaction is broadcast to the blockchain. The final outcome is determined by the on-chain execution result.

## **Roles in Collaboration**

In team collaboration, different members can perform distinct duties:

<table data-header-hidden><thead><tr><th width="183.57421875"></th><th></th></tr></thead><tbody><tr><td><strong>Role</strong></td><td><strong>Primary Responsibilities</strong></td></tr><tr><td>Initiator</td><td>Initiates transaction requests</td></tr><tr><td>Approver</td><td>Reviews transactions against business requirements and approves or rejects them</td></tr><tr><td>Signer</td><td>Signs transactions to authorize broadcasting to the blockchain</td></tr><tr><td>Viewer</td><td>Views collaboration requests and transaction processing statuses</td></tr></tbody></table>
