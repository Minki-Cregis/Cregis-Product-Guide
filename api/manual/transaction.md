# 查询交易记录

在 WaaS 项目中，交易记录用于查看当前项目下所有与资金流转相关的业务记录，帮助用户追踪提币、子地址交易以及归集交易记录。交易记录主要分为以下三类：

* 提币记录
* 交易记录
* 归集记录

## **提币记录**

提币记录用于查看通过 API 发起的提币申请记录。根据提币来源不同，分为：

* 钱包提币：指通过钱包提币接口发起的提币申请记录。
* 子地址提币：指通过子地址提币接口发起的提币申请记录。

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=NDU2MWI1ZDNjNDk1MmJjNjhjM2I3ZTc3ZGRjNzhkMWVfeUI4NXBWY1lEZklhTWZXVUtWSUNkM09XYmhPWlFLRW1fVG9rZW46RHNNdGIzUldub3ZESFF4eGROOGw3ckNXZ0tmXzE3ODAyODIwNTM6MTc4MDI4NTY1M19WNA" alt=""><figcaption></figcaption></figure>

## **交易记录**

交易记录用于查看 WaaS 项目子地址相关的交易记录。包括：

* 接收
* 发送

不包含：

* 归集相关交易 （归集、矿工费充值）

交易记录分为：

* 历史记录：显示最终状态（成功、失败、已取消）的交易记录，
* 处理中：显示当前仍在链上待确认的交易记录。

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=MmVmZWUzMTY5M2FmNGE0ZDZiZDBjZjA1MWY2NmJmMzJfdkNZZGR0dm00a0E3UmlsMVJQbUdoT2FsMGc0bU5yQTRfVG9rZW46RFBXMWJEU1k2b1VvTVJ4aHNkVmw2VGFiZ2llXzE3ODAyODIxNTc6MTc4MDI4NTc1N19WNA" alt=""><figcaption></figcaption></figure>

**归集记录**归集记录用于查看 WaaS 项目子地址归集相关的交易记录。包括：

* 归集 （手动归集、自动归集）
* 矿工费充值

归集记录分为：

* 历史记录：显示最终状态（成功、失败、已取消）的归集交易记录。
* 处理中：显示当前仍在链上待确认的归集交易记录。

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=NDg3NzA5OGE0YmMzNWNiNWM2ODA3YTJiZmVlNjQ3OTJfQnRKVm9rQkUzaWhaSnQyV1ZvN0NPQ3RZWm5Cd2p0ZGVfVG9rZW46UVFRbmJrVHkzb1g1NEZ4QUdwcmxPVThNZ1hjXzE3ODAyODIxNzU6MTc4MDI4NTc3NV9WNA" alt=""><figcaption></figcaption></figure>





