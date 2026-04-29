---
hidden: true
---

# Shard Recovery

The shard recovery feature is designed for <mark style="color:green;">**multisig wallets**</mark>, allowing shard restoration when a creator loses their shard. The recovery process requires all wallet creators to participate online by importing their recovery phrases. Upon successful recovery, all creators' shards will be reset.

**Important notes for shard recovery:**

* Wallets that don't support TON/SUI chains: \
  Only have one set of recovery phrases, can perform reset and recovery functions.
* Wallets that support TON/SUI chains: \
  Need to use a device that has the wallet's shards to perform the reset operation. During reset, two sets of recovery phrases will be generated for you, and you can use the recovery function normally afterward.
* New users creating wallets will directly get two sets of recovery phrases and can use the reset and shard recovery functions normally.

### Recovery Manual:  <a href="#cao-zuo-guo-cheng" id="cao-zuo-guo-cheng"></a>

Enter the wallet information page through the following entry.

<figure><img src="../../.gitbook/assets/image (742).png" alt=""><figcaption></figcaption></figure>

Click "Recover" under Shard Management.

<figure><img src="../../.gitbook/assets/image (743).png" alt=""><figcaption></figcaption></figure>

After clicking, a recovery shard window will appear, then you need to wait for other members to come online.\
Note: Other members need to switch their page to the current team to be recognized as online.

When all members have agreed to join, the initiator can click "Start".

<figure><img src="../../.gitbook/assets/image (755).png" alt=""><figcaption></figcaption></figure>

Invited members can view the invitation in their wallet notifications.

<figure><img src="../../.gitbook/assets/image (762).png" alt=""><figcaption></figcaption></figure>

After starting, you need to enter recovery phrases. New users creating multisig wallets will have two sets of recovery phrases and need to enter the first set of secp256k1 recovery phrases.\
If it's an old user's wallet that doesn't support TON/SUI chains, the system will automatically determine, and the user only needs to enter one set of recovery phrases to recover.

<figure><img src="../../.gitbook/assets/image (756).png" alt=""><figcaption></figcaption></figure>

After completing the first set, you can then enter the second set of ed25519 recovery phrases.\
If it's an old user's wallet that doesn't support TON/SUI chains, the system will skip this step directly.

<figure><img src="../../.gitbook/assets/image (757).png" alt=""><figcaption></figcaption></figure>

You need to wait for all members to import their recovery phrases. After all members have finished importing, the initiator clicks "Start".

<figure><img src="../../.gitbook/assets/image (758).png" alt=""><figcaption></figcaption></figure>

If each member entered the correct recovery phrases, the shards will be successfully recovered immediately after the recovery animation finishes, and all members' shards will be reset.\
Note: After recovering shards, previously authorized shards on other devices will also become invalid and need to be reauthorized.

<figure><img src="../../.gitbook/assets/image (759).png" alt=""><figcaption></figcaption></figure>
