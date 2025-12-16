# 为什么BTC地址有不同的格式？

## **为什么BTC有不同地址格式**

比特币地址格式的多样性源于技术升级，旨在解决早期网络的限制，如交易处理速度、手续费和可扩展性问题。这些改进引入了新技术如隔离见证，提升了交易效率、安全性，并支持更多功能，同时保留对旧地址格式的兼容性。地址格式的演变反映了比特币随着需求变化不断发展和优化的过程。&#x20;

### **常见的BTC地址及用途**

| 类型                                        | 地址格式                | 特点                                                                        | 推荐用途                                                                                    |
| ----------------------------------------- | ------------------- | ------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| <p>Legacy（P2PKH/P2SH）传统地址<br></p>         | 以「1」开头              | 最初的比特币地址，功能齐全。与新格式地址相比，交易大小较大和较高的矿工费                                      | 与不支援隔离见证的旧钱包或服务进行交互                                                                     |
| Nested SegWit（P2SH-P2WPKH）：隔离见证（兼容）       | <p>以「3」开头<br></p>   | 在相容传统地址和提高交易效率之间提供了一种折衷方案，它的交易大小较小，费用略低于传统地址                              | 想要与旧钱包或服务相容，但仍希望享受一些隔离见证的好处                                                             |
| <p>Native SegWit（P2WPKH）：隔离见证（原生）<br></p> | <p>以「bc1」开头<br></p> | 提供了最高的交易效率，从而实现了最小的交易大小和最低的矿工费，与其他格式相比，它们还具有改进的安全功能，减少由于比特币块大小的限制而导致的网路拥塞 | 通过重点优化权重，比特币提升了效率，透过最小化区块大小和重构交易资料储存方式，显著提高了网络的可扩展性与交易处理速度，实现更顺畅、更高效的交易体验，并提升区块内的交易吞吐量。 |

## 如何区分和设置默认收款地址？

### PC版

用户可以先进入钱包页面，然后选择币种，再按右方的地址便可以查看到你现有钱包于这个加密货币下生成的地址。

<figure><img src="../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

选择币种就可以查看到你现有钱包于这个加密货币下生成的地址，你可以透过标签分辨哪个地址是你的默认付款及默认收款的地址，目前一共有5种标签：

* 默认收款：此地址为默认收款地址
* 默认付款：此地址为默认付款地址
* 普通地址：此地址为普通的BTC地址
* 隔离见证(兼容)：此地址格式为隔离见证（兼容）
* 隔离见证(原生)：此地址格式为隔离见证（原生）

<figure><img src="../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

如需新增地址可按右上加号，选择隔离见证（兼容）或隔离见证（原生）地址，选择完成后可以输入新地址的别名。

<figure><img src="../../.gitbook/assets/image (498).png" alt=""><figcaption></figcaption></figure>

如需设置默认收款或付款地址，则可以把鼠标放到地址，按「更多」再设定成预计付款／收款地址。

<figure><img src="../../.gitbook/assets/image (499).png" alt=""><figcaption></figcaption></figure>

设置完成后，用户也可在收款的地方看到此地址的格式。

<figure><img src="../../.gitbook/assets/image (500).png" alt=""><figcaption></figcaption></figure>

### 手机版

先于底导航栏转到钱包页面，然后选择你需要查看的货币

<figure><img src="../../.gitbook/assets/image (501).png" alt="" width="188"><figcaption></figcaption></figure>

进入货币页面后点入「地址」进入地址页面

<figure><img src="../../.gitbook/assets/image (502).png" alt="" width="188"><figcaption></figcaption></figure>

按进去后可以查看该币种在此钱包下现有的地址，同时可透过标签辨认地址格式及是否默认收款／付款使用的地址。

* 默认收款：此地址为默认收款地址
* 默认付款：此地址为默认付款地址
* 普通地址：此地址为普通的BTC地址
* 隔离见证(兼容)：此地址格式为隔离见证（兼容）
* 隔离见证(原生)：此地址格式为隔离见证（原生）

<figure><img src="../../.gitbook/assets/image (503).png" alt="" width="137"><figcaption></figcaption></figure>

可点击「新建BTC地址」选择地址格式，然后为新地址输入别名<br>

<figure><img src="../../.gitbook/assets/image (504).png" alt=""><figcaption></figcaption></figure>

如需设置收款／付款地址，则可以点击想要设定的地址，然后于功能表中选择设置为收款／付款地址。

<figure><img src="../../.gitbook/assets/image (505).png" alt="" width="138"><figcaption></figcaption></figure>

设置完成后也可到收款的页面查看地址及其格式。

<figure><img src="../../.gitbook/assets/image (506).png" alt="" width="140"><figcaption></figcaption></figure>
