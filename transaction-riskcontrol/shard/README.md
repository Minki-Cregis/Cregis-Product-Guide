# 分片管理

Cregis采用先进的<mark style="color:green;">**MPC（多方计算）分片技术**</mark>，通过将私钥分割成多个分片来增强安全性。在<mark style="color:green;">**单签钱包**</mark>中，这些MPC分片安全地存储在本地设备和<mark style="color:green;">**可信执行环境（TEE）**</mark>中，确保没有任何单一实体掌握完整的密钥。对于<mark style="color:green;">**多签钱包**</mark>，分片分布在不同的本地设备上，进一步通过去中心化控制来提升安全性。每次进行交易时，MPC分片会在多个位置进行计算，并与存储在云端的分片结合，确保交易签名过程高度安全且高效。

