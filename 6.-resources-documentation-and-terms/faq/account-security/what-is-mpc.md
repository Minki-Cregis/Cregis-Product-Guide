# What is MPC?

MPC (Multi-Party Computation) is short for "secure multi-party computation." It allows two or more parties to jointly compute a result without revealing their individual inputs. For example, MPC enables a group of friends to calculate their average salary securely without disclosing their individual earnings.

In cryptocurrency wallets, MPC facilitates the creation of a secure key management system without a single point of failure. Multiple parties (e.g., remote servers and mobile devices) can collaboratively perform cryptographic functions such as key generation, transaction signing, and verification without exposing their private data. Crucially, MPC ensures that a complete private key is never created, split, or reconstructed during the process, making it superior to traditional single-key models.

By leveraging MPC, consumer-focused wallets and institutional services can design secure on-chain asset management systems, eliminating private key vulnerabilities. This offers a more secure self-custody option, preventing key theft (as there’s no single key to steal) and key loss (as each party can independently back up their encrypted inputs without compromising the system).

## **Advantages of MPC**

* **Easy Recovery**: Ensures asset access even in adverse scenarios.
* **No Single Point of Failure**: Enhances security by eliminating central points of risk.
* **Full User Control**: Users retain full control over their assets.
* **Broad Blockchain Compatibility**: Unlike MultiSigs, which are not supported across all blockchains, MPC can be applied to many.

## **Unique MPC Features in Cregis**

1. **Single-Signature Wallets**:
   * Requires only one member for signing.
   * Cregis’ patented technology generates two shards: one stored on the user’s device and the other managed in Cregis’ cloud TEE (Trusted Execution Environment). Both shards must combine during signing, ensuring security. Even if one shard is compromised, it cannot be used independently, eliminating single-point risks and enabling keyless management.
2. **Multi-Signature Wallets**:
   * Requires multiple members to complete a signature.
   * Shards are generated and managed across client devices, while Cregis’ cloud stores none of them.
   * Multiple devices collaborate using their respective shards for signing. Users can also customize conditions, such as specifying which members must approve and how many approvals are required for signing.
