# Role

The functionalities available to team members are determined by their assigned roles. Cregis supports the creation, editing, and deletion of roles, allowing precise management of each member's permissions within the team. Each role's scope of permissions can be finely tuned to meet specific needs. The Super Administrator role, which includes all permissions, cannot be edited or deleted.

## Permission Definition

Configure access levels by assigning these permissions to different team roles.

### **Wallet**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>Create Wallet</td><td>Allows creating new wallets.</td></tr></tbody></table>

<mark style="color:green;">**Please note that Wallet-specific permissions are managed separately, please refer to**</mark> [<mark style="color:blue;">**wallet member management**</mark>](../wallet-and-transactions/wallet/wallet-member-management.md)<mark style="color:green;">**.**</mark>

### **Task**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>Approval</td><td>Allows processing workflows where the assigned approver is oneself.</td></tr><tr><td>View All Collaborative Data</td><td>Allows viewing full collaboration logs (requests, approvals, signatures).</td></tr><tr><td>Initiate Payment Request</td><td>Allows submitting payment requests.</td></tr><tr><td>Signature</td><td>Allows processing workflows where the assigned signer is either oneself or not specified.</td></tr></tbody></table>

<mark style="color:green;">**Please note that approval and signature permission depend on workflow rules and shard ownership.**</mark>

### WaaS

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>View</td><td>Allows viewing all projects in the API page.</td></tr><tr><td>Create API</td><td>Allows creating new projects for the team.</td></tr><tr><td>Callback Handling</td><td>Allows processing callback records, including feeding or ignoring.</td></tr><tr><td>API Access</td><td>Allows viewing API Keys and gateway servers.</td></tr><tr><td>Collection</td><td>Allows collecting funds from project sub-addresses.</td></tr><tr><td>Reset API Key</td><td>Allows resetting API Keys.</td></tr><tr><td>Add address</td><td>Allows manually creating addresses for projects.</td></tr><tr><td>Transaction</td><td>Allows initiating transactions from project sub-addresses.</td></tr><tr><td>Disable the address</td><td>Allows enabling/disabling project sub-addresses.</td></tr><tr><td>Notification</td><td>Allows modifying project notification settings.</td></tr></tbody></table>

### **Payment Engine**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>View</td><td>Allows viewing the Payment Engine page.</td></tr><tr><td>Create API</td><td>Allows creating new Payment Engine projects.</td></tr><tr><td>Edit</td><td>Allows editing project name and notifications configuration.</td></tr><tr><td>API Access</td><td>Allows viewing API Keys and gateway servers for the project.</td></tr><tr><td>Reset API Key</td><td>Allows resetting API Keys for the project.</td></tr><tr><td>Settlement Settings</td><td>Allows configuring settlement rules for the project.</td></tr></tbody></table>

### **Report**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>View</td><td>Allows viewing team transaction history across all wallets.</td></tr><tr><td>Export</td><td>Allows exporting billing records.</td></tr></tbody></table>

### **Policy**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>View</td><td>Allows accessing the policy page.</td></tr><tr><td>Add New Policy</td><td>Allow adding a new policy for the team.</td></tr><tr><td>Modify Policy</td><td>Allows modifying, enabling, and disabling policy.</td></tr><tr><td>Delete Policy</td><td>Allow deleting policy.</td></tr><tr><td>View Policy Log</td><td>Allows viewing the policy execution log.</td></tr></tbody></table>

### **Automation**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>View</td><td>Allows accessing the automation page.</td></tr><tr><td>Add Rule</td><td>Allows setting up new automation rules.</td></tr><tr><td>Edit Rule</td><td>Allows modifying existing rules.</td></tr><tr><td>Delete Rule</td><td>Allows removing automation rules.</td></tr><tr><td>Execute Rule</td><td>Allows enabling/disabling rules.</td></tr><tr><td>Execution Log</td><td>Allows reviewing rule execution history.</td></tr></tbody></table>

### **AML Query**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>View</td><td>Allows accessing the AML Query page.</td></tr><tr><td>Manual Query</td><td>Allows performing manual AML queries.</td></tr><tr><td>Create Rule</td><td>Allows creating rules for automatic AML queries.</td></tr><tr><td>Edit Rule</td><td>Allows editing rules for automatic AML queries.</td></tr><tr><td>Delete Rule</td><td>Allows deleting rules for automatic AML queries.</td></tr><tr><td>Disable/Enable Rule</td><td>Allows disabling or enabling rules for automatic AML queries.</td></tr></tbody></table>

### **Address Book**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>View</td><td>Allows viewing the team address book.</td></tr><tr><td>Add New Address Book</td><td>Allows adding new addresses to the book.</td></tr><tr><td>Modify Address</td><td>Allows modifying existing addresses.</td></tr><tr><td>Delete Address Book</td><td>Allows removing addresses.</td></tr></tbody></table>

### **Subscription**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>View</td><td>Allows viewing the subscription page. Members without this permission can only see basic benefits.</td></tr><tr><td>Renew Upgrade</td><td>Allows upgrading or renewing the team’s subscription plan.</td></tr><tr><td>Scale Up</td><td>Allows expanding team features.</td></tr><tr><td>Coin application</td><td>Allows submitting requests for new token listings.</td></tr></tbody></table>

### **Member Management**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>View</td><td>Allows viewing the list of team members and their roles.</td></tr><tr><td>Invite Members</td><td>Allows inviting new members to the team.</td></tr><tr><td>Modify Member</td><td>Allows modifying member roles.</td></tr><tr><td>Remove Member</td><td>Allows removing members from the team.</td></tr></tbody></table>

### **Role Management**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>View</td><td>Allows viewing the Role Management page.</td></tr><tr><td>Add New Role</td><td>Allow adding a new role for the team</td></tr><tr><td>Modify Role</td><td>Allows modifying role permissions.</td></tr><tr><td>Delete Role</td><td>Allows removing roles.</td></tr></tbody></table>

### **Enterprise Verification**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>Start Verification</td><td>Allows initiating enterprise verification</td></tr><tr><td>View Verification Info</td><td>Allows viewing enterprise verification information</td></tr></tbody></table>

### **Marketplace**

<table><thead><tr><th width="239.03125">Permission</th><th>Definition</th></tr></thead><tbody><tr><td>View</td><td>Allows viewing the Application Marketplace</td></tr><tr><td>Manage Applications</td><td>Allows managing permissions for individual applications</td></tr></tbody></table>

Please note that editing permissions for applications within the Application Marketplace needs to be done separately on the[ <mark style="color:green;">**Application Management**</mark> ](../marketplace/manage-applications.md)page.

## **Manual**

### **Adding Role**

You can manage your team’s roles by navigating to <mark style="color:green;">**Manage**</mark> <mark style="color:green;"></mark><mark style="color:green;">→</mark> <mark style="color:green;"></mark><mark style="color:green;">**Role**</mark>. On the role management page, you can add new roles and edit their permissions. Saving changes requires email verification from the team creator and your Google verification.

<figure><img src="../.gitbook/assets/image (926).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (927).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (928).png" alt=""><figcaption></figcaption></figure>

### **Delete Role**

You can delete a role as below. Please note that you need to complete the Google verification to delete a role.

<figure><img src="../.gitbook/assets/image (929).png" alt=""><figcaption></figcaption></figure>

### **Edit Role**

You can enter the role permissions edition page as below:

<figure><img src="../.gitbook/assets/image (930).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (931).png" alt=""><figcaption></figcaption></figure>
