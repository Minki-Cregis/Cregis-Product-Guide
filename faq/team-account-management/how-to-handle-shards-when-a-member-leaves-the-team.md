# How to Handle Shards When a Member Leaves the Team?

If the departing member is the wallet creator, it is recommended to replace the wallet for asset management. During wallet creation, Cregis displays the recovery phrase once, which poses a risk of phrase leakage.

If the departing member is not the wallet creator and their shard was authorized to them, the following steps can ensure asset security:

1.  **Remove Shards from Specific Devices**\
    Use the wallet's shard management feature to delete all device shards associated with the departing member. This ensures the shards are not exposed.



    <figure><img src="../../.gitbook/assets/image (349).png" alt=""><figcaption></figcaption></figure>
2.  **Reset Shards**\
    Resetting wallet shards is another option. However, this will require all shard holders of the wallet to be reauthorized, and it involves the use of the recovery phrase, making it a less optimal solution.\
    Only the wallet creator has the authority to reset shards. The entry point for this operation is shown below:

    <figure><img src="../../.gitbook/assets/image (350).png" alt=""><figcaption></figcaption></figure>

    Resetting shards requires entering the recovery phrase. Once completed, all related shards of the wallet will be invalidated and must be reauthorized.

    <figure><img src="../../.gitbook/assets/image (351).png" alt=""><figcaption></figcaption></figure>
