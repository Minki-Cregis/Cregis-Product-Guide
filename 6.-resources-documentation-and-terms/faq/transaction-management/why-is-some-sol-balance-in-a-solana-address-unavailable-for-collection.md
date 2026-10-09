# Why Is Some SOL Balance in a Solana Address Unavailable for Collection?

Solana on-chain accounts must maintain a minimum SOL balance based on the account data size to meet on-chain storage requirements. This balance is commonly referred to as the **rent-exempt minimum balance** and can be understood as a refundable account storage deposit rather than an ongoing network rent charge. Cregis reserves a portion of SOL according to its applicable reservation rules and excludes it from the collectible balance. (The current reserved amount is 0.00089088 SOL.)

For more information, please refer to the official Solana documentation:

* [Account Structure and Storage Balance](https://solana.com/docs/core/accounts/account-structure)
* [Accounts Overview](https://solana.com/docs/core/accounts)

