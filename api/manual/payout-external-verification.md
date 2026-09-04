# 提币外部验证

提币外部验证用于在提币申请（钱包提币和子地址提币）进入Cregis审批流程前，增加一层由客户业务系统控制的审核环节。\
开启该功能后，当用户发起提币申请时，系统不会立即执行提币审批/签名，而是先将提币申请通过回调接口发送至客户配置的外部验证系统。客户可结合自身的业务规则、风控策略或审批流程对提币申请进行审核，并将审核结果返回至 Cregis。

Cregis将根据审核结果继续处理提币申请：

* **审核通过（ok）**：继续执行后续提币流程。
* **审核拒绝（deny）**：终止本次提币申请，不再进行签名和链上广播。

通过提币外部验证，企业可将 Cregis WaaS 与内部审批、风控或合规系统集成，实现提币业务的自定义审核流程，进一步提升资金安全性和风险管控能力。

## **开启提币外部验证**

登录Cregis 客户端进入WaaS项目 > 设置 > 回调设置页面，点击提币外部验证「开启」按钮

<figure><img src="../../.gitbook/assets/image (1072).png" alt=""><figcaption></figcaption></figure>

\
弹出开启提币外部验证提示弹窗，点击「确定」

<figure><img src="../../.gitbook/assets/image (1073).png" alt=""><figcaption></figcaption></figure>

按钮进入配置回调URL页面，输入或粘贴要接收提币回调的URL，然后点击「测试连接」按钮

<figure><img src="../../.gitbook/assets/image (1074).png" alt=""><figcaption></figcaption></figure>

系统将会尝试与您的URL地址进行通信测试，测试成功则提示“测试成功，服务器响应正常。”，然后点击「确定」按钮

<figure><img src="../../.gitbook/assets/image (1075).png" alt=""><figcaption></figcaption></figure>

完成身份验证，则开启成功

<figure><img src="../../.gitbook/assets/image (1076).png" alt=""><figcaption></figcaption></figure>

## **修改回调URL**

登录Cregis 客户端进入WaaS项目 > 设置 > 回调设置页面，点击提币外部验证「编辑」按钮

<figure><img src="../../.gitbook/assets/image (1077).png" alt=""><figcaption></figcaption></figure>

进入配置回调URL页面，输入或粘贴要修改的回调URL，然后点击「测试连接」按钮

<figure><img src="../../.gitbook/assets/image (1078).png" alt=""><figcaption></figcaption></figure>

系统将会尝试与您的URL地址进行通信测试，测试成功则提示“测试成功，服务器响应正常。”，然后点击「确定」按钮

<figure><img src="../../.gitbook/assets/image (1079).png" alt=""><figcaption></figcaption></figure>

完成身份验证，点击「确定」按钮，修改成功

<figure><img src="../../.gitbook/assets/image (1080).png" alt=""><figcaption></figcaption></figure>

## **关闭提币外部验证**

登录Cregis 客户端进入WaaS项目 > 设置 > 回调设置页面，点击提币外部验证「关闭」按钮

<figure><img src="../../.gitbook/assets/image (1081).png" alt=""><figcaption></figcaption></figure>

弹出关闭提币外部验证提示弹窗，点击「确定」按钮

<figure><img src="../../.gitbook/assets/image (1082).png" alt=""><figcaption></figcaption></figure>

完成身份验证，点击「确定」按钮，关闭成功

<figure><img src="../../.gitbook/assets/image (1083).png" alt=""><figcaption></figcaption></figure>

