# 地址簿

地址簿用于集中管理链上地址的风险属性，支持维护 白名单 和 黑名单 两类地址。

* 白名单：用于记录可信地址，可作为风控放行、地址识别、内部常用地址管理的依据，并且可在发送交易时快速选择。
* 黑名单：用于记录风险地址、禁止交易地址或需重点拦截的地址。

用户可在客户端中对地址进行新增、编辑、删除、筛选和批量导入，便于风控团队统一维护地址数据。功能入口：风控 → 地址簿 → 白名单 / 黑名单

## **新增白名单地址**

点击白名单页面的「新增」按钮并选择币种。

<figure><img src="../.gitbook/assets/image (1003).png" alt=""><figcaption></figcaption></figure>

进入新增页面后，可直接在表格中填写地址信息，如需新增多条地址，可点击表格左下角的「+」添加新行，或点击页面右上角的「上传表单」批量导入地址。

<figure><img src="../.gitbook/assets/image (1004).png" alt=""><figcaption></figcaption></figure>

确认无误后，点击界面左下角的「保存」按钮。

<figure><img src="../.gitbook/assets/image (1005).png" alt=""><figcaption></figcaption></figure>

完成身份验证，则添加白名单地址成功。

<figure><img src="../.gitbook/assets/image (1006).png" alt=""><figcaption></figcaption></figure>

## **编辑白名单地址**

在白名单列表中找到目标地址，点击「编辑」按钮。

<figure><img src="../.gitbook/assets/image (1007).png" alt=""><figcaption></figcaption></figure>

进入白名单编辑页面，修改币种、别名、地址相关信息。

<figure><img src="../.gitbook/assets/image (1008).png" alt=""><figcaption></figcaption></figure>

确认修改后，点击「保存」按钮，完成身份验证，则编辑成功。

<figure><img src="../.gitbook/assets/image (1009).png" alt=""><figcaption></figcaption></figure>

## **删除白名单地址**

在白名单列表中找到目标地址，点击「删除」按钮。

<figure><img src="../.gitbook/assets/image (1010).png" alt=""><figcaption></figcaption></figure>

点击删除白名单地址确认弹窗的「确定」按钮，完成身份验证，则删除成功。

<figure><img src="../.gitbook/assets/image (1011).png" alt=""><figcaption></figcaption></figure>

## **开启/关闭白名单校验**

开启后，仅允许向已添加至白名单的地址发送交易，未加入白名单的地址将无法发起交易，白名单校验仅对客户端手动发起的交易生效，通过 API 发起的提币请求，不校验白名单。

功能入口：管理 → 团队安全 → 白名单校验

<figure><img src="../.gitbook/assets/image (1012).png" alt=""><figcaption></figcaption></figure>

## **新增黑名单地址**

点击黑名单页面的「新增」按钮。

<figure><img src="../.gitbook/assets/image (1013).png" alt=""><figcaption></figcaption></figure>

进入新增页面后，可直接在表格中填写地址信息，如需新增多条地址，可点击表格左下角的「+」添加新行，或点击页面右上角的「上传表单」批量导入地址。

<figure><img src="../.gitbook/assets/image (1014).png" alt=""><figcaption></figcaption></figure>

确认无误后，点击界面左下角的「保存」按钮，则添加黑名单地址成功。

<figure><img src="../.gitbook/assets/image (1015).png" alt=""><figcaption></figcaption></figure>

## **编辑黑名单地址**

在黑名单列表中找到目标地址，点击「编辑」按钮。

<figure><img src="../.gitbook/assets/image (1016).png" alt=""><figcaption></figcaption></figure>

进入黑名单编辑页面，修改别名、地址相关信息。

<figure><img src="../.gitbook/assets/image (1017).png" alt=""><figcaption></figcaption></figure>

确认修改后，点击「保存」按钮，完成身份验证，则编辑成功。

<figure><img src="../.gitbook/assets/image (1018).png" alt=""><figcaption></figcaption></figure>

## **删除黑名单地址**

在黑名单列表中找到目标地址，点击「删除」按钮。

<figure><img src="../.gitbook/assets/image (1019).png" alt=""><figcaption></figcaption></figure>

点击删除黑名单地址确认弹窗的「确定」按钮，完成身份验证，则删除成功。

<figure><img src="../.gitbook/assets/image (1020).png" alt=""><figcaption></figcaption></figure>

