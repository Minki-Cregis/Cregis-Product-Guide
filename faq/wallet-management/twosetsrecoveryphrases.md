# Why are there two sets of recovery phrases (ed25519 and secp256k1)?

Your wallet automatically generates two sets of recovery phrases because different blockchains use different cryptographic standards. To ensure the security and full compatibility of your assets, we employ a dual-recovery-phrase design.

**Here are the specific reasons:**

* **Technical Necessity**
  * Different blockchains use different encryption standards.&#x20;
  * **First recovery phrase (ed25519):** Supports high-performance blockchains like Solana (SOL), Sui (SUI), Ton (TON), Aptos (APT), and Cardano (ADA).
  * **Second recovery phrase (secp256k1):** Supports Bitcoin (BTC), Ethereum (ETH), and other EVM-compatible chains (e.g., BSC, Polygon).
  * Since the two encryption algorithms (ed25519 and secp256k1) are incompatible, separate recovery phrases are required to manage assets across different chains.
* **Security Design**
  * **Asset isolation reduces risk:** The two recovery phrases are completely independent. Even if one is compromised, the assets managed by the other remain secure.
  * **Prevents asset loss due to derivation errors:** For example, using an ed25519 recovery phrase to restore a secp256k1-based wallet will fail.

**What You Need to Know**

* **Backup both recovery phrases—neither can be omitted.** Losing one may result in irreversible loss of assets on certain chains.
* **When recovering your wallet, you must import both phrases** to regain full access to all assets across supported chains.

**Why Can’t They Be Combined Into One?**\
The blockchain industry has not yet unified cryptographic standards. Our dual-recovery-phrase solution ensures **100% security and compatibility** for your assets. Should industry standards evolve, we will promptly optimize the user experience.

**I Only Use Bitcoin/Ethereum—Why Do I Need to Back Up the ed25519 Phrase?**\
Even if you don’t currently use chains like Solana or Cardano, storing **both phrases** ensures future flexibility. The ed25519 phrase will be essential if you ever wish to interact with these high-performance blockchains.
