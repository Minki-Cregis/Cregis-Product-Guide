# Table of contents

## 欢迎使用CREGIS <a href="#welcome" id="welcome"></a>

* [产品概览](README.md)
* [支持的链及加密货币](welcome/tokensandprotocols.md)

## 新手入门 <a href="#gettingstarted" id="gettingstarted"></a>

* [下载及安装](gettingstarted/download.md)
* [帐号注册及登录](gettingstarted/registration.md)

## 帐户管理 <a href="#accountmanagement" id="accountmanagement"></a>

* [个人空间及团队空间](accountmanagement/space.md)
* [帐单及付款](accountmanagement/bill_and_payment/README.md)
  * [管理团队版本](accountmanagement/bill_and_payment/pricing_plan.md)
  * [开通收费功能](accountmanagement/bill_and_payment/feature_activation.md)
  * [帐单管理](accountmanagement/bill_and_payment/manage_your_bill.md)
  * [充值团队帐户](accountmanagement/bill_and_payment/recharge_your_account.md)
* [帐户安全](accountmanagement/security.md)
* [帐户设定](accountmanagement/settings.md)

## 团队 <a href="#team" id="team"></a>

* [团队管理](team/management.md)
* [成员](team/members.md)
* [权限](team/permission.md)
* [团队协作](team/teamwork/README.md)
  * [发起交易申请](team/teamwork/initiate_send_request.md)
  * [审批流](team/teamwork/approval.md)
  * [交易签名](team/teamwork/transaction_signing.md)

## 钱包及交易 <a href="#wallet_and_transaction" id="wallet_and_transaction"></a>

* [钱包](wallet_and_transaction/wallet/README.md)
  * [创建钱包](wallet_and_transaction/wallet/creation.md)
  * [钱包成员管理](wallet_and_transaction/wallet/members.md)
  * [重新命名钱包](wallet_and_transaction/wallet/rename.md)
  * [隐藏钱包](wallet_and_transaction/wallet/hide_your_wallet.md)
  * [信息签名](wallet_and_transaction/wallet/message_signature.md)
* [币种](wallet_and_transaction/token_management.md)
* [地址](wallet_and_transaction/address.md)
* [分片管理](wallet_and_transaction/shard/README.md)
  * [检查分片状态](wallet_and_transaction/shard/shard_status.md)
  * [授权分片](wallet_and_transaction/shard/authorization.md)
  * [删除分片](wallet_and_transaction/shard/delete.md)
  * [恢復分片](wallet_and_transaction/shard/recovery.md)
  * [重置分片](wallet_and_transaction/shard/reset.md)
* [交易](wallet_and_transaction/transaction/README.md)
  * [发送及接收](wallet_and_transaction/transaction/transfer_and_receive.md)
  * [交易加速及取消](wallet_and_transaction/transaction/speed_up_and_cancel.md)
  * [交易重发](wallet_and_transaction/transaction/resend.md)
  * [交易记录](wallet_and_transaction/transaction/dashboard.md)
  * [地址簿](wallet_and_transaction/transaction/address_book.md)
  * [Tron能量模式](wallet_and_transaction/transaction/tron_energy_mode.md)

## 风险管理 <a href="#risk_management" id="risk_management"></a>

* [策略中心](risk_management/policy_engine.md)
* [Copy of 策略中心](risk_management/policy_engine-1.md)
* [自动归集／签名](risk_management/automation.md)
* [AML查询功能](risk_management/aml_query.md)

## API

* [API操作手册](api/manual/README.md)
  * [创建项目](api/manual/creation.md)
  * [配置IP白名单](api/manual/configuration.md)
  * [查询API接入信息](api/manual/access_information.md)
  * [生成地址](api/manual/wallet_address_creation.md)
  * [查询交易记录](api/manual/transaction.md)
  * [归集](api/manual/collection.md)
  * [回调查询](api/manual/callback_query.md)
  * [回调设置](api/manual/callback_setting.md)
  * [通知设置](api/manual/notification.md)
  * [禁用及删除项目](api/manual/disable_and_delete.md)
  * [开发者API中心](api/manual/developer.md)
  * [于API接入TON链](api/manual/ton.md)
* [接口种类](api/type.md)

## 支付引擎 <a href="#payment_engine" id="payment_engine"></a>

* [简介](payment_engine/introduction.md)
* [创建支付引擎](payment_engine/creation.md)
* [修改支付引擎配置](payment_engine/configuration.md)
* [查询订单相关记录](payment_engine/records.md)
* [订单逻辑](payment_engine/additional_payment_and_refund_processes.md)
* [支付链结（收银台）](payment_engine/checkout_page.md)

## 汇款 <a href="#remittance" id="remittance"></a>

* [發起匯款單](remittance/records.md)
* [常用收款人](remittance/recipient_list.md)

## FAQ

* [钱包相关](faq/wallet/README.md)
  * [什么是非托管钱包？](faq/wallet/what_is_a_non_custodial_wallet.md)
  * [为什么我看不到团队的钱包？](faq/wallet/why_cant_i_see_the_team_wallet.md)
  * [为什么BTC地址有不同的格式？](faq/wallet/btc_address_format.md)
  * [我可以在一个钱包内创建多个地址吗？](faq/wallet/can_i_create_multiple_addresses_within_a_single_wallet.md)
  * [为什么会出现分片不支持添加币种？](faq/wallet/why_does_the_shard_not_support_adding_tokens.md)
  * [为什么我的钱包数据无法载入？](faq/wallet/why_cant_my_wallet_data_load.md)
  * [为什么我的 MATIC 币不见了？](faq/wallet/matic_missing.md)
  * [为什么我想授权分片给成员时成员没有导入的选项？](faq/wallet/shard_authorizing.md)
  * [为什么有ed25519和secp256k1两组助记词？](faq/wallet/twosetsrecoveryphrases.md)
* [交易相关](faq/transaction/README.md)
  * [为什么多签需要同时在线？](faq/transaction/multi_signing.md)
  * [为什么我的协作里没有签名？](faq/transaction/teamwork_signing.md)
  * [为什么交易状态一直在确认中？](faq/transaction/transaction_confirmation.md)
  * [如果两条策略权重相同且同时命中，系统会优先执行哪一条？](faq/transaction/policy_prioritization.md)
  * [为什么发送交易时显示请先导入分片？](faq/transaction/shard.md)
  * [如果我的钱包收到黑U，应该如何处理？](faq/transaction/blacku.md)
  * [为什么有些地址需要有激活费？](faq/transaction/activation_fee.md)
  * [关闭了客户端后仍可自动签名吗？](faq/transaction/auto-signing.md)
  * [高级模式及普通模式的矿工费设置有什么分别？](faq/transaction/gas_fee_setting.md)
  * [什么是Tron能量模式？](faq/transaction/shen-me-shi-tron-neng-liang-mo-shi.md)
  * [我可以使用团队账户余额支付矿工费吗？](faq/transaction/wo-ke-yi-shi-yong-tuan-dui-zhang-hu-yuezhi-fu-kuang-gong-fei-ma.md)
  * [我可以授权给我的员工签名吗？](faq/transaction/wo-ke-yi-shou-quan-gei-wo-de-yuan-gong-qian-ming-ma.md)
* [API相关](faq/api/README.md)
  * [API 项目创建后还可以编辑类型吗？](faq/api/waas-type-edition.md)
  * [为什么我找不到订单收款的项目创建？](faq/api/wei-shen-me-wo-zhao-bu-dao-ding-dan-shou-kuan-de-xiang-mu-chuang-jian.md)
  * [API次数用完后系统会立即停止吗？](faq/api/api-ci-shu-yong-wan-hou-xi-tong-hui-li-ji-ting-zhi-ma.md)
  * [我可以直接通过 API 发出出款指令吗？](faq/api/wo-ke-yi-zhi-jie-tong-guo-api-fa-chu-chu-kuan-zhi-ling-ma.md)
  * [出现异常回调应该如何操作？](faq/api/error-callback.md)
  * [为什么接入 TON 币种时 API 返回不支持币种？](faq/api/wei-shen-me-jie-ru-ton-bi-zhong-shi-api-fan-hui-bu-zhi-chi-bi-zhong.md)
  * [我的项目已经停止，但仍有用户不小心转账到项目地址，应如何处理？](faq/api/project-name-defunct-how-to-recover-funds.md)
  * [我团队版本到期后项目无法进行归集，应如何处理？](faq/api/wo-tuan-dui-ban-ben-dao-qi-hou-xiang-mu-wu-fa-jin-xing-gui-ji-ying-ru-he-chu-li.md)
  * [每次归集有笔数的限制吗？](faq/api/mei-ci-gui-ji-you-bi-shu-de-xian-zhi-ma.md)
* [团队帐户相关](faq/team_account/README.md)
  * [为什么我的团队账户无法升级？](faq/team_account/wei-shen-me-wo-de-tuan-dui-zhang-hu-wu-fa-sheng-ji.md)
  * [成员离职后应如何处理分片？](faq/team_account/cheng-yuan-li-zhi-hou-ying-ru-he-chu-li-fen-pian.md)
  * [如何解散团队？](faq/team_account/ru-he-jie-san-tuan-dui.md)
  * [如何邀请团队成员加入？](faq/team_account/ru-he-yao-qing-tuan-dui-cheng-yuan-jia-ru.md)
  * [为什么我完成权限编辑后仍无法进行操作？](faq/team_account/wei-shen-me-wo-wan-cheng-quan-xian-bian-ji-hou-reng-wu-fa-jin-xing-cao-zuo.md)
  * [如何设置审批流程？](faq/team_account/ru-he-she-zhi-shen-pi-liu-cheng.md)
  * [如果我团队版本到期后没有续费的话会停止运作吗？](faq/team_account/ru-guo-wo-tuan-dui-ban-ben-dao-qi-hou-mei-you-xu-fei-de-hua-hui-ting-zhi-yun-zuo-ma.md)
* [安全相关](faq/security/README.md)
  * [什么是MPC？](faq/security/shen-me-shi-mpc.md)
  * [MPC 分片有没有被窃取的风险？](faq/security/mpc-fen-pian-you-mei-you-bei-qie-qu-de-feng-xian.md)
  * [使用 Cregis 时资产存放在哪里？](faq/security/shi-yong-cregis-shi-zi-chan-cun-fang-zai-na-li.md)
  * [什么是TEE环境？](faq/security/shen-me-shi-tee-huan-jing.md)
  * [丢失了助记词应如何安全处理？](faq/security/diu-shi-le-zhu-ji-ci-ying-ru-he-an-quan-chu-li.md)
  * [设备遗失或损毁了如何安全处理？](faq/security/she-bei-yi-shi-huo-sun-hui-le-ru-he-an-quan-chu-li.md)
  * [如何开启及关闭地址簿校验？](faq/security/ru-he-kai-qi-ji-guan-bi-di-zhi-bo-jiao-yan.md)
  * [什么是策略？](faq/security/shen-me-shi-ce-le.md)
* [其他常见问题](faq/others/README.md)
  * [安装客户端异常如何处理？](faq/others/an-zhuang-ke-hu-duan-yi-chang-ru-he-chu-li.md)
  * [Cregis 的钱包可以从哪里重新导入呢？](faq/others/cregis-de-qian-bao-ke-yi-cong-na-li-chong-xin-dao-ru-ne.md)
  * [Cregis 会提供测试环境吗？](faq/others/cregis-hui-ti-gong-ce-shi-huan-jing-ma.md)
  * [KYB/KYC 的审批要多久？](faq/others/kybkyc-de-shen-pi-yao-duo-jiu.md)
  * [为什么我登不进我的测试环境？](faq/others/wei-shen-me-wo-deng-bu-jin-wo-de-ce-shi-huan-jing.md)
  * [如何查看我的Cregis版本？](faq/others/ru-he-cha-kan-wo-de-cregis-ban-ben.md)
  * [忘记了交易密码怎么办？](faq/others/wang-ji-le-jiao-yi-mi-ma-zen-me-ban.md)

## 条款与细则 <a href="#terms_and_conditions" id="terms_and_conditions"></a>

* [服务条款](terms_and_conditions/terms_of_service.md)
* [收集个人资料声明](terms_and_conditions/personal_information_collection_statement.md)

## Cregis Support

* [联系我们](cregis-support/contact_us.md)
