# 权限

团队成员可使用的功能由其分配的角色决定。Cregis支持创建、编辑和删除角色，允许精确管理每个成员在团队中的权限。每个角色的权限范围可以根据具体需求进行细致调整。包含所有权限的超级管理员角色无法编辑或删除。

## 权限说明

以下为各项权限的功能定义，请根据团队角色进行配置。

### 成员管理

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>查看</td><td>允许查看团队成员名单及其角色。</td></tr><tr><td>邀请成员</td><td>允许邀请新成员。</td></tr><tr><td>修改成员</td><td>允许修改成员角色。</td></tr><tr><td>删除成员</td><td>允许删除成员。</td></tr></tbody></table>

### 项目

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>查看</td><td>允许查看项目页面的所有项目。</td></tr><tr><td>创建项目</td><td>允许为团队创建新项目。</td></tr><tr><td>回调处理</td><td>允许处理回调记录，包括重推或忽略。</td></tr><tr><td>API接入</td><td>允许用户可查看API Key及网关服务器。</td></tr><tr><td>归集</td><td>允许为项目子地址进行归集。</td></tr><tr><td>重置API Key</td><td>允许重置API Key。</td></tr><tr><td>创建地址</td><td>允许为项目手动创建地址。</td></tr><tr><td>发送交易</td><td>允许发起项目子地址的发送交易流程。</td></tr><tr><td>地址禁用</td><td>允许禁用或启用项目子地址。</td></tr><tr><td>通知配置</td><td>允许修改项目内的通知配置。</td></tr></tbody></table>

### 订阅

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>查看</td><td>允许查看团队订阅介面，没有此权限的成员只能看到基本权益。。</td></tr><tr><td>续费升级</td><td>允许团队订阅版本进行升级或续费。</td></tr><tr><td>扩容</td><td>允许为团队进行功能扩容。</td></tr><tr><td>上币申请</td><td>允许申请上币。</td></tr></tbody></table>

### 加密卡

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>查看</td><td>允许查看加密卡介面。</td></tr><tr><td>查看所有卡</td><td>允许查看所有团队创建的加密卡。</td></tr><tr><td>充值</td><td>允许为加密卡进行充值功能。</td></tr><tr><td>加密卡设置</td><td>允许编辑加密卡名称，此名称只适用于内部。</td></tr><tr><td>安全码</td><td>允许查看安全码。</td></tr><tr><td>创建加密卡</td><td>允许创建加密卡。</td></tr></tbody></table>

&#x20;<mark style="color:green;">**请注意以上充值、加密卡设置及安全码功能只适用于该用户能查看的卡。**</mark>

### AML查询

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>查看</td><td>允许查看AML查询页面。</td></tr><tr><td>AML查询</td><td>允许进行AML查询。</td></tr></tbody></table>

### 支付引擎

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>查看</td><td>允许查看支付引擎页面。</td></tr><tr><td>创建项目</td><td>允许创建新的支付引擎项目。</td></tr><tr><td>编辑项目</td><td>允许编辑项目名称、通知配置。</td></tr><tr><td>API接入</td><td>允许成员可查看该支付引擎项目的API Key及网关服务器。</td></tr><tr><td>重置API Key</td><td>允许成员可重置API Key。</td></tr><tr><td>结算配置</td><td>允许成员可以编辑该支付引擎项目的结算配置。</td></tr></tbody></table>

### 角色管理

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>查看</td><td>允许查看角色管理页面。</td></tr><tr><td>新增角色</td><td>允许为团队新增角色。</td></tr><tr><td>修改角色</td><td>允许修改角色权限。</td></tr><tr><td>删除角色</td><td>允许删除角色。</td></tr></tbody></table>

### 地址簿

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>查看</td><td>允许查看团队地址簿。</td></tr><tr><td>新增地址簿</td><td>允许于地址簿新增地址。</td></tr><tr><td>修改地址簿</td><td>允许修改地址簿内地址。</td></tr><tr><td>删除地址簿</td><td>允许删除地址簿内地址。</td></tr></tbody></table>

### 协作

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>审批</td><td>允许处理指定审批人是本人的流程。</td></tr><tr><td>查看所有协作数据</td><td>允许查看所有团队协作数据，包括申请、审批及签名。</td></tr><tr><td>付款申请</td><td>允许提出付款申请。</td></tr><tr><td>签名</td><td>允许处理指定签名人是本人或未有指定签名人的流程。</td></tr></tbody></table>

<mark style="color:green;">**请注意审批及签名只是开放操作权限，但实则视乎流程是否需要该成员审批以及该成员是否有分片进行签名。**</mark>

### 钱包

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>创建钱包</td><td>允许创建钱包。</td></tr></tbody></table>

<mark style="color:green;">**请注意钱包有独立的权限设置，详情可参考**</mark>[<mark style="color:blue;">**钱包成员管理**</mark>](../wallet_and_transaction/wallet/members.md)<mark style="color:green;">**。**</mark>

### 账单

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>查看</td><td>允许查看团队账单，包括所有钱包的出入金。</td></tr><tr><td>导出</td><td>允许导出账单记录。</td></tr></tbody></table>

### 策略

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>查看</td><td>允许查看团队策略页面。</td></tr><tr><td>新增策略</td><td>允许新增策略。</td></tr><tr><td>修改策略</td><td>允许修改、启用及停用策略。</td></tr><tr><td>删除策略</td><td>允许删除策略。</td></tr><tr><td>策略日志</td><td>允许查看团队策略日志。</td></tr></tbody></table>

### 自动化

<table><thead><tr><th width="239.03125">权限</th><th>定义</th></tr></thead><tbody><tr><td>查看</td><td>允许查看团队自动化页面。</td></tr><tr><td>新增规则</td><td>允许新增规则。</td></tr><tr><td>修改规则</td><td>允许修改规则。</td></tr><tr><td>删除规则</td><td>允许删除规则。</td></tr><tr><td>运行规则</td><td>允许启用或停用规则。</td></tr><tr><td>执行日志</td><td>允许查看团队自动化执行日志。</td></tr></tbody></table>

## 操作流程

### 新增角色

您可以通过导航至“管理” → “角色”来管理团队的角色。在角色管理页面，您可以添加新角色并编辑其权限。

<figure><img src="../.gitbook/assets/image (310).png" alt=""><figcaption></figcaption></figure>

### 删除角色

您可以按照下方步骤删除角色。请注意，删除角色时需要完成Google验证。

<figure><img src="../.gitbook/assets/image (311).png" alt=""><figcaption></figcaption></figure>

### 编辑角色

您可以根据以下步骤为角色进编辑。

<figure><img src="../.gitbook/assets/image (312).png" alt=""><figcaption></figcaption></figure>
