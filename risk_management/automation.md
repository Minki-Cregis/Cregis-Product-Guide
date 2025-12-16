# 自动归集／签名

## 什么是自动归集／签名？

这项自动化功能让用户可以根据预设的规则进行自动资金归集和交易签名，无需企业安排人手进行持续监控。一旦设置好规则，系统便可24小时不间断地按照设定规则运行，大幅减少人工干预。例如，过去企业可能需要每天手动进行资金归集，但有了自动化功能，用户可以设定每隔多长时间自动归集资金。此外，还可以根据特定的币种且达到某个金额数值后再启动归集流程。目前，自动签名功能仅限于API出金操作，并只对单签钱包开放。另外，这些自动化功能全部都是本地化进行﹐无需有任何托管分片的动作，用户只需要保持在线状态便可以执行，这既保证了系统的安全性，也为需要频繁交易的企业带来了极大的运营效率提升。

<figure><img src="../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

## 收费表及开通流程

* 目前自动化功能只开放于月费用户，并需每月额外支付 USD $500才可以使用此功能。如需开通可到以下帐户介面，点击「开通」。

<figure><img src="../.gitbook/assets/image (359).png" alt=""><figcaption></figcaption></figure>

* 点击后会有视窗弹出，用户可以选择所需的月份并按提交。

<figure><img src="../.gitbook/assets/image (360).png" alt=""><figcaption></figcaption></figure>

* 提交订单后可以立即支付，支付成功后便可开通。

<figure><img src="../.gitbook/assets/image (361).png" alt=""><figcaption></figcaption></figure>

## 操作手册

请于操作前先确认你已开通自动化功能

1. 进入自动化功能页面，并点击「**创建规则**」

<figure><img src="../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

2. ### 创建自动归集规则

点击「**创建规则**」后，右边有栏目弹出可以开始设定。

<figure><img src="../.gitbook/assets/image (363).png" alt=""><figcaption></figcaption></figure>

**基础设置** \
创建规则时先设置名称及类型，选择「自动归集」类型后，便会有栏目弹出需选择归集类型和WaaS项目

<figure><img src="../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

归集类型分为系统归集和API归集，系统归集是指根据您设定的规则，系统自动归集符合条件的子地址资金；API归集是指根据您设定的规则，归集由API发起的归集请求

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=NzEzZDkxNTM2NDE1Y2IzYzkwOGU0Yjk2NWFhYzMwN2RfaW1NUWlGcUdYdXdERFdpcERmSGVPRm8ya0FrcWw5ZVFfVG9rZW46WENXcGJ0WGh5b05mRFF4RkEzamxOV2FXZ3ZiXzE3NjA5NDc3MDk6MTc2MDk1MTMwOV9WNA" alt="" width="375"><figcaption></figcaption></figure>

**触发条件**\
触发规则中需要设定币种、归集时间及收款地址条件

*   币种 \
    每个规则中只允许设定一种币种，按添加时会显示你所选的项目预设钱包内已设定的币种。设定币种后需设立触发自动归集的金额，大于及小于的条件可以同时符合。如想设定$100-$200时，可设定大于等于100及小于等于200。 \
    <mark style="color:green;">**请注意如果设定条件不合理时将无法成功创建规则，例如小于等于50及大于等于51**</mark><br>

    <figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=YjNjOGVlNjkwOWU0MGFiZDY5Mjg0MzUzMmZiNWFjY2JfSzJUbGdXNW1RTkJ0cENPV3FscGt3MHhEYmRpTXpBbzRfVG9rZW46RFQwbmJKMFdtb21maGV4NnhEQ2xEaEVoZ05lXzE3NjA5NDc4MTU6MTc2MDk1MTQxNV9WNA" alt="" width="375"><figcaption></figcaption></figure>
* 执行动作 \
  用户可选择每隔一段时间执行或是每天于特定的时间点进行自动归集。<mark style="color:green;">**这里的时间目前以UTC+8为准。**</mark>

<figure><img src="../.gitbook/assets/image (369).png" alt=""><figcaption></figcaption></figure>

*   收款地址 \
    收款地址目前只支持选择当前项目钱包的地址进行收款，所以系统会默认设定该钱包的预设收款地址。

    <figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=NmI0ZTI4NWRhYmUwZDFlYWE1M2Q5Nzk3ZjM0OTg2OThfdW5WNGVKR1R1d2lBVWJ4V2JSSkhWQktDZUF3VDB1TTFfVG9rZW46TVRhb2JoTXJUbzVxdVB4azN0WGxIWlFKZ1ViXzE3NjA5NDc4NzA6MTc2MDk1MTQ3MF9WNA" alt="" width="375"><figcaption></figcaption></figure>
*   完成后点击提交，提交后需进行身份认证，认证成功即创建完成。<br>

    <figure><img src="../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>
*   创建后需启用规则才会生效，启用时需进行密码及Google双重验证，验证成功后正式开始使用。<br>

    <figure><img src="../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>
* 归集成功后可到项目地址页面，上面会显示「自动归集中」。请注意自动归集进行中必须保持客户端处于在线状态，否则自动归集会中断。

<figure><img src="../.gitbook/assets/image (373).png" alt=""><figcaption></figcaption></figure>

3. ### 创建自动签名规则

点击「**创建规则**」后，右边有栏目弹出可以开始设定。

<figure><img src="../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

**基础设置** \
创建规则时先设置名称及类型，选择「自动签名」类型后，便会有栏目弹出需选择提币类型和出款钱包，**请注意 目前只支持单签钱包并使用预设付款地址进行签名出款。**

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=ZGU3OThlNDI3MzYxNjRlYjM4ZDkyZDExNWM2ZjBlNWVfRHZldDlPQ1V4alh0NEJXdExab1c0RnZOQ2l3MmJqa01fVG9rZW46UjRBdGI3QW1wbzRpWTN4dkdTMGxGMVdBZ1hjXzE3NjA5NDc5NzY6MTc2MDk1MTU3Nl9WNA" alt=""><figcaption></figcaption></figure>

提币类型分为提币和子地址API出款，提币是指根据您设定的规则，系统自动签名符合条件的API提币申请；子地址API出款是指根据您设定的规则，系统自动签名符合条件的子地址API出款申请

<figure><img src="https://0xcregis.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=MTZjNmM5MWJhMTk3MGYyNzM4MzNlZWE0MWJmNzEzYTlfOG1Da3RxeDlXWmtFWjlpMkZIRlgxM1ZadVdXQllUdXVfVG9rZW46VUp5c2JHbDEzb3J6ZFl4MHBNVWxoQWFQZ2hoXzE3NjA5NDgwMDY6MTc2MDk1MTYwNl9WNA" alt="" width="375"><figcaption></figcaption></figure>

**触发規則**\
触发规则中需要设定币种、出金类型及执行动作条件

*   币种 \
    每个规则中只允许设定一种币种，按添加时会显示你所选的出款钱包内已设定的币种。设定币种后需设立触发自动签名的金额，大于及小于的条件可以同时符合。如想设定$100-$200时，可设定大于等于100及小于等于200。 <mark style="color:green;">**请注意如果设定条件不合理时将无法成功创建规则，例如小于等于50及大于等于51。**</mark><br>

    <figure><img src="../.gitbook/assets/image (35).png" alt="" width="290"><figcaption></figcaption></figure>
*   出金类型 \
    由于目前只支持API出金，所以在此部份需要选择你需要进行出金的API。<br>

    <figure><img src="../.gitbook/assets/image (36).png" alt="" width="298"><figcaption></figcaption></figure>
* 执行动作 \
  这里可以进行定时签名的设定，这里的时间目前以UTC+8为准。另外用户需户需设置每隔多少分钟进行一次签名，触发时如多于一笔会以打包形式上链，于某些链可以为用户节省矿工费。

<figure><img src="../.gitbook/assets/image (378).png" alt="" width="304"><figcaption></figcaption></figure>

* 完成后点击提交，提交后需进行身份认证，认证成功即创建完成。

<figure><img src="../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

* 启用后可到协作页面，右下会显示自动签名进行中。<mark style="color:green;">**请注意自动签名进行中必须保持上线状态，否则自动签名会中断。**</mark>

<figure><img src="../.gitbook/assets/image (381).png" alt=""><figcaption></figcaption></figure>

4. ### 编辑及删除自动化规则

* 编辑规则

已创建的规则可以在规则配置页面进行编辑，进行编辑前必须先禁用规则，禁用时需要进行身份验证。

<figure><img src="../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

* 删除规则&#x20;

删除已创建的规则可以在规则配置页面中进行，删除前必须先禁用规则，禁用时需要进行身份验证。

<figure><img src="../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

5. ### 查看自动化日志

进入执行日志可以看到每一个规则的动向，包括日期时间、操作人员及动作。

<figure><img src="../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

在此页面用户亦可根据操作日期、操作人或日志类型进行筛选

<figure><img src="../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

同时搜寻栏亦支持使用日志名称及编号去搜寻相关记录。

<figure><img src="../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure>

6. ### 触发自动归集

如触发自动归集的规则条件，系统便会进行自动归集，用户可到项目地址查看自动归集详情

<figure><img src="../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

* 详情中会显示运行时长、开放时间及已归集的笔数及金额，另外交易记录亦有列明每笔归集的记录

<figure><img src="../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

* 如果因矿工费不足导致自动归集暂停，有提示显示需要充值，用户可直接于此页面按「**充值**」，然后可通过充值弹窗的地址及 QR 码进行充值，充值后会在下一个触发点再执行动作。

<figure><img src="../.gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

7. ### 触发自动签名

* 如触发自动签名的规则条件，系统便会进行自动签名，用户可到协作看自动签详情，右下会出现「自动签名运行中」的图标。

<figure><img src="../.gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure>

* 详情中会显示运行时长、开启时间、已签名的笔数、金额及签名所用的矿工费，另外交易记录有显示每笔归集的记录。如果因矿工费不足导致自动签名暂停，有提示显示需要充值，用户可直接于此页面按「**充值**」，然后可通过弹窗的地址及 QR 码进行充值，充值后会在下一个触发点再执行动作。

<figure><img src="../.gitbook/assets/image (394).png" alt=""><figcaption></figcaption></figure>

## 实际使用场景

实际的设置需根据用户自身需求进行，以下是一些场照的自动归集／签名设置。

**场景一：我想每天定期为项目子地址中的USDT进行归集**\
这种情况下只要项目内地址有USDT都会触发条件，而用户只需要设定币种及自定义每天归集时间，例如每天的12:00分时进行。

<figure><img src="../.gitbook/assets/image (395).png" alt="" width="294"><figcaption></figcaption></figure>

**场景二：周末时只要项目内的出金金额少于USDT $100可自动签名**\
这种情况下需要设定币种及定时签名的日子，同时也要列明隔多久才签一次。

<figure><img src="../.gitbook/assets/image (396).png" alt="" width="292"><figcaption></figcaption></figure>
