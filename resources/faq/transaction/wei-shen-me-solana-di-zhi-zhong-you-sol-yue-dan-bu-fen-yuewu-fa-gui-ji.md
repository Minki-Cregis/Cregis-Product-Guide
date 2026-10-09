# 为什么 Solana 地址中有 SOL 余额，但部分余额无法归集？

Solana 链上账户需要根据账户数据大小维持一定的最低 SOL 余额，以满足链上存储要求。这部分余额通常称为 _Rent-exempt minimum balance_（免租最低余额），可以理解为可退还的账户存储押金，而非持续扣除的网络租金。Cregis 会根据相关预留规则，将部分 SOL 排除在可归集余额之外（当前预留金额为 0.00089088 SOL）。

如需了解详细信息，请参考 Solana 官方文档：

* [账户结构与存储余额说明](https://solana.com/zh/docs/core/accounts/account-structure)
* [账户基础知识](https://solana.com/zh/docs/core/accounts)

