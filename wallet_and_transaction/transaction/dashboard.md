# 交易记录

此页面提供完整的钱包交易记录查询，涵盖团队钱包及Waas项目交易，支持企业清晰查阅所有明细。您可根据需要进行筛选，并将数据导出为Excel文件，便于对账或处理其他财务任务。

## 查看记录明细

用户可点击记录想查看的记录明细

<figure><img src="../../.gitbook/assets/image (719).png" alt=""><figcaption></figcaption></figure>

点击后会有视窗弹出展示此交易的详细记录

<figure><img src="../../.gitbook/assets/image (720).png" alt=""><figcaption></figcaption></figure>

## 更改数据时区

用户可以点击交易时间，更改当前数据展示的时区，导出数据时亦会按照当前选择的时区导出。

<figure><img src="../../.gitbook/assets/image (721).png" alt=""><figcaption></figcaption></figure>

## 导出交易记录

点击右上角导出按钮，即可选择导出的日期，注意目前导出的日期范围不可超过12个月，导出的数据会按当前所选择的时区有调整。

<figure><img src="../../.gitbook/assets/image (722).png" alt=""><figcaption></figcaption></figure>

点击“导出”后，系统将开始准备文件，处理时间取决于数据量大小。完成后，您可在“导出历史”中下载。您还可以在此查看并下载团队其他成员的历史导出文件。

请注意：导出的文件为压缩包。由于技术原因，目前“并行转账”类别的交易（通过打包技术上链）会共用同一个交易哈希。因此，这些交易的详细明细将单独生成，并保存在压缩包内一个名字含有 **“batch”** 的文件中。

<figure><img src="../../.gitbook/assets/image (723).png" alt=""><figcaption></figcaption></figure>

## 交易类型说明

<table><thead><tr><th>交易类型</th><th width="107.578125">收支类型</th><th width="306.8515625">定义</th><th width="374.53515625">触发场景</th></tr></thead><tbody><tr><td>钱包人工转出<br></td><td>转出<br></td><td><ul><li>由客户端发起的钱包出款</li></ul><p><br></p></td><td><ul><li>从钱包点击发送</li><li>团队成员发起付款申请</li><li>通过链上交易进行的充值(团队、加密卡)</li></ul></td></tr><tr><td>API申请转出<br></td><td>转出<br></td><td><ul><li>由API请求的转出申请</li></ul><p><br></p></td><td><ul><li>API申请发送的交易，包含所有主地址及地址转出</li></ul></td></tr><tr><td>归集转出<br></td><td>转出<br></td><td><ul><li>项目子地址归集出款</li></ul><p><br></p></td><td><ul><li>项目归集时触发由子地址转出</li><li>API触发归集</li><li>每次同时出现转出及转入</li></ul></td></tr><tr><td>归集转入</td><td>转入</td><td><ul><li>项目归集转入至钱包</li></ul></td><td><p></p><ul><li>项目归集时触发由子地址转入钱包</li><li>API触发归集</li><li>每次同时出现转出及转入</li></ul></td></tr><tr><td>矿工费(归集)转出</td><td>转出</td><td><ul><li>主钱包出款用于支付归集矿工费的资金</li></ul></td><td><ul><li>归集需要支付矿工费时</li><li>每次同时出现转出及转入</li></ul></td></tr><tr><td>矿工费(归集)转入</td><td>转入</td><td><ul><li>项目子地址收到用于支付归集矿工费的资金</li></ul></td><td><p></p><ul><li>归集需要支付矿工费时</li><li>每次同时出现转出及转入</li></ul></td></tr><tr><td>普通转入</td><td>转入</td><td><ul><li>地址收到资金转入时</li></ul></td><td><ul><li>包含所有主地址及子地址收款</li></ul></td></tr><tr><td>并行转出</td><td>转出</td><td><ul><li>交易用打包形式转出的交易 (由于现时没法拆分，先归成一个交易类型)</li></ul></td><td><ul><li>用户同时有多条相同系列的交易以打包形式上链</li></ul></td></tr></tbody></table>
