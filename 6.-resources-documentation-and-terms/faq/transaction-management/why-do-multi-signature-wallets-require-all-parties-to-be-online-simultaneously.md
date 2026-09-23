# Why Do Multi-Signature Wallets Require All Parties to Be Online Simultaneously?

Other wallets implement multi-sig through a separate signing approach. After one party completes their signature, the platform stores that party's key share in the cloud and then waits for the other party to sign. However, this approach is equivalent to the platform temporarily holding the complete private key, which poses a significant security risk.

To safeguard user assets, Cregis adopts a more rigorous security design to avoid such practices. Cregis's multi-sig feature is based on MPC (Multi-Party Computation) technology, where the user's private key never exists in its complete form. During the signing process, each party's key share interacts in real time through cryptographic protocols to complete the signature, without any party needing to store their share in the cloud. This ensures the absolute security of the private key while eliminating the potential risks associated with centralized storage.

Therefore, Cregis's multi-sig requires all parties to be online simultaneously in order to complete the signature through real-time interaction, preventing any party's key share from being stored in the cloud and thereby ensuring the private key remains secure at all times.
