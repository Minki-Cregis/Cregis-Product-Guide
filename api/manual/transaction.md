# 查询交易记录

项目内目前有三个页面可查看与项目相关的交易记录：

* 交易记录\
  所有不是从API发起的交易记录都会被记录在这里，包括地址手动转出、接收、矿工费充值及系统归集记录。
* 提币记录\
  这里记录的是通过Payout API发起的记录，经此API发起的提币皆是从**钱包的地址**而非项目地址转出。
* 出款记录\
  这里记录的是通过Withdrawal API发起的记录，经此API发起的提币是从**项目地址**转出。



你可以在WaaS项目中找到此三个交易记录的入口：

<figure><img src="../../.gitbook/assets/image (627).png" alt=""><figcaption></figcaption></figure>

