# 高级模式及普通模式的矿工费设置有什么分别？

高级模式与普通模式的 Gas 费设置主要区别在于协议基础与费用控制方式。高级模式采用了 EIP-1559 协议，利用新的费用计算方式，让交易确认速度更快，且理论上能减少费用波动，适合需要高优先级确认的用户。在高级模式中，用户可以自定义 Max Fee（最大费用）和 Max Priority Fee（优先费用），达到精确控制。而普通模式基于传统 Gas 费结构，需手动设置 Gas Price 和 Gas Limit，灵活性较低，但适合对 EIP-1559 不熟悉或习惯使用传统设置方式的用户。相比之下，高级模式更能节省费用并提供稳定表现，而普通模式则延续了传统的设置习惯。

<figure><img src="../../.gitbook/assets/image (269).png" alt="" width="375"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (270).png" alt="" width="375"><figcaption></figcaption></figure>
