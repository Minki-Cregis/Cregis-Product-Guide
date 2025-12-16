---
hidden: true
---

# 恢復分片

恢复分片功能主要是针对<mark style="color:green;">**多签钱包**</mark>，当有创建人失去分片时，可透过此功能恢复分片。恢复过程需要所有钱包创建人在线参与，并且需要导入助记词，恢复成功后所有创建人的分片将会被重置。

**恢复分片时用户需要注意以下事项：**

* 不支持添加TON、SUI链的钱包：只有一套助记词，可以进行重置和恢复操作
* 线上支持添加TON、SUI链的钱包：需使用有该钱包分片的设备进行重置操作，重置时会为您生成两套助记词，后续可正常使用恢复功能
* 新用户创建钱包时直接有两套助记词，可正常使用重置及恢复分片功能。

## 操作过程

先透过以下入口进入钱包信息页面

<figure><img src="../../.gitbook/assets/image (583).png" alt=""><figcaption></figcaption></figure>

于分片管理下点击恢复

<figure><img src="../../.gitbook/assets/image (584).png" alt=""><figcaption></figcaption></figure>

点击后会有个恢复分片的视窗，然后需要等待其他成员在线\
这里需要注意，其他成员需要把页面<mark style="color:green;">**切换至当前团队**</mark>才会被判定为在线。

<figure><img src="../../.gitbook/assets/image (585).png" alt=""><figcaption></figcaption></figure>

被邀请成员可于钱包通知内查看邀请

<figure><img src="../../.gitbook/assets/image (75).png" alt=""><figcaption></figcaption></figure>

当所有成员都同意加入后，发起人可点击开始

<figure><img src="../../.gitbook/assets/image (586).png" alt=""><figcaption></figcaption></figure>

开始后需要输入助记词，新用户创建多签钱包时会拥有两组助记词，需要先输入第一组secp256k1助记词\
如旧用户的钱包为不支持添加TON、SUI链的钱包，系统会自行判断，用户只需输入一组助记词即可恢复。

<figure><img src="../../.gitbook/assets/image (587).png" alt=""><figcaption></figcaption></figure>

完成输入第一组后，可接著输入第二组ed25519助记词\
如旧用户的钱包为不支持添加TON、SUI链的钱包，系统则会直接跳过这步

<figure><img src="../../.gitbook/assets/image (588).png" alt=""><figcaption></figcaption></figure>

输入完成后需等待所有成员导入助记词

<figure><img src="../../.gitbook/assets/image (589).png" alt=""><figcaption></figcaption></figure>

所有成员导入完成后，发起人点击开始。

<figure><img src="../../.gitbook/assets/image (590).png" alt=""><figcaption></figcaption></figure>

如果每个成员输入的助记词正确，于恢复分片动画完结后便会直接恢复成功，所有成员的分片都会被重置。\
请注意，恢复分片后之前被授权到其他设备的分片也会失效，需要重新授权。

<figure><img src="../../.gitbook/assets/image (591).png" alt=""><figcaption></figcaption></figure>

