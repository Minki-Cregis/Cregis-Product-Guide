# Team Member Removal Risk Notice & Guidelines

To ensure the security of your team's assets and business continuity, please carefully review the following risk warnings and complete all required configuration checks and cleanups before removing a team member on Cregis.

## Assets and Wallet Security

* Single-Sig Wallet Access Transfer
  * If the member to be removed is the creator of a single-signature wallet, removing them will cause the team to <mark style="color:$danger;">**permanently lose**</mark> all administrative access to that wallet.
  * Recommendation: Prior to removal, transfer all assets from the wallet to another secure team wallet.

## Tasks and Approval Workflows

* Pending Approval Data
  * If the member has pending/unresolved approval data in the "Collaboration" module, the system will block the removal operation.
  * Recommendation: Clear, revoke, or complete all approval processes associated with this member before attempting removal again.
* Impact on Risk Control Policies
  * If the member is the sole designated approver or signer for a specific Risk Control policy:
    * The policy will remain active after the member is removed.
    * However, any subsequent transactions triggering this policy will fail to process due to the missing approver/signer.
  * Recommendation: Check your risk control policies before removal to ensure alternative approvers or signers are assigned.

## System Automation and Risk Monitoring

* Interruption of Automation Rules
  * If the member is actively running any "Automation" tasks, those tasks will <mark style="color:$danger;">**stop immediately**</mark> upon the member's removal.
  * Recommendation: Review the status of automated tasks prior to removal, and ensure another active team member restarts or takes over the workflow.
* AML Alert Recipients
  * If the member is set as the sole recipient for AML auto-scanning risk alerts, the system will block the removal operation.
  * Recommendation: Assign another risk alert recipient to the AML auto-scanning rule and save the configuration before proceeding.

## Automatic Disabling of Notification Settings

* If the member being removed is the sole recipient of any of the following critical business notifications, the system will <mark style="color:$danger;">**automatically turn off those notification settings**</mark>, which may result in missed critical alerts:
  * WaaS Project Notifications
    * Callback failure alerts
    * Enable or disable project alerts
    * API Key reset alerts
    * Insufficient team balance to cover service charges alerts
    * Payment exception notifiaiton
  * Payment Engine Notifications
    * Callback failure alerts
    * Enable or disable project alerts
    * API Key reset alerts
    * Payment exception notifiaiton
  * Team Account Notification
    * Insufficient team balance alerts
* Recommendation: Before removing a member, review the notification settings across "WaaS Projects," "Payment Engine," and "Team Account," and reassign alternative team members to avoid operational disruptions or security risks.
