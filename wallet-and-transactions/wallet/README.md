# Wallet

## About Cregis Wallet

<mark style="color:green;">**Cregis Wallet**</mark> offers a self-custody solution that gives users full control over their private keys and crypto assets. Using advanced Multi-Party Computation (MPC) technology, Cregis splits private keys into shards stored in different locations, ensuring high asset security. Cregis never pre-generates or stores private keys and operates without third-party reliance for transaction verification, providing users with a secure and efficient way to manage their cryptocurrency.



These are the wallets we provided:

<table data-header-hidden><thead><tr><th width="244">Question</th><th width="214">Single-Signature Wallet</th><th>Multi-Signature Wallets</th></tr></thead><tbody><tr><td><br></td><td><strong>single-signature wallet</strong></td><td><strong>multi-signature wallets</strong></td></tr><tr><td><strong>How many shards will be generated?</strong></td><td><ul><li>Two shards will be generated</li><li>The wallet owner will have his own <strong>15 recovery phrases</strong>.</li></ul><p><br></p></td><td><ul><li>Depending on the specific configuration of the multi-signature wallet</li><li>For example, in a 2-of-3 multi-signature setup, three shards are created. All of them have their own <strong>24 recovery phrase</strong>.</li></ul></td></tr><tr><td><strong>Where do Cregis store the shards?</strong></td><td><ul><li>One shard is stored on the user's local device and the other one stored in multiple Trusted Execution Environments (TEE)</li></ul></td><td><ul><li>Shards are stored in the user's local device depending on the wallet setting</li></ul></td></tr><tr><td><strong>How many signatures are required to process the transaction?</strong><br></td><td><ul><li>Only one signature is required</li></ul><p><br></p></td><td><ul><li>Depending on the users specific configuration of the multi-signature wallet</li><li>Users can set conditions based on different scenarios, allowing the original private key to be reassembled to generate a legitimate signature.</li><li>For example, in a 2-of-3 multi-signature setup, three shards are created, and <strong>any two of them are needed</strong> to sign a transaction.</li></ul></td></tr></tbody></table>

