# 银行通知来源与验证范围

核实日期：2026-10-10。v0.2.39 接入 48 个个人手机银行应用来源，共用人民币扣款模板，不按商户单独适配。

来源核实依据为小米应用商店列出的应用包名和开发者。此处“来源已核实”不等于真实通知格式已逐家实测，也不代表运行时进行了银行签名证书验证；通知来源按系统提供的准确包名匹配，不按应用名称或通知标题模糊匹配。

广东农信已纳入。河源当地农商行若使用广东农信应用，并由该应用发出匹配的扣款通知，可走同一模板；卡片属于哪家支行不影响这一路径。其他省级农信或独立农商行应用分别登记，不推断所有农商行都使用同一应用。

## 使用条件

- 开启自动记账、对应渠道，通知服务已连接；银行应用实际发送新的、内容可读取的扣款通知。
- 模板支持明确支出、消费、扣款以及成功付款中的人民币金额；不把余额、优惠金额当成消费。
- 新渠道默认开启，既有渠道选择保留。识别后直接预填金额，由用户确认入账；不确定是消费还是充值时可取消。
- 银行与微信／支付宝的弱关联仅提示疑似重复，不据此丢弃；明确交易编号的关联规则沿用上一版。
- 没有应用通知、仅发短信、金额隐藏、未知文案或未列出的独立应用，不能承诺自动识别。银行页面、短信、独立信用卡应用不在本次新增范围。

## 已核实应用

以下均为来源登记与通用模板接入，实际设备通知仍待逐项验证。测试使用虚构金额与账户，不代表已使用这些银行付款。

| 显示名称 | 应用包名 | 开发者 | 依据 |
|---|---|---|---|
| 交通银行 | `com.bankcomm.Bankcomm` | 交通银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.bankcomm.Bankcomm) |
| 工商银行 | `com.icbc` | 中国工商银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.icbc) |
| 农业银行 | `com.android.bankabc` | 中国农业银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.android.bankabc) |
| 中国银行 | `com.chinamworld.bocmbci` | 中国银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.chinamworld.bocmbci) |
| 建设银行 | `com.chinamworld.main` | 中国建设银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.chinamworld.main) |
| 招商银行 | `cmb.pb` | 招商银行股份有限公司 | [应用商店](https://app.mi.com/details?id=cmb.pb) |
| 邮储银行 | `com.yitong.mbank.psbc` | 中国邮政储蓄银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.yitong.mbank.psbc) |
| 平安口袋银行 | `com.pingan.paces.ccms` | 平安银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.pingan.paces.ccms) |
| 徽商银行 | `com.hsbank.mobilebank` | 徽商银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.hsbank.mobilebank) |
| 中信银行 | `com.ecitic.bank.mobile` | 中信银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.ecitic.bank.mobile) |
| 浦发银行 | `cn.com.spdb.mobilebank.per` | 上海浦东发展银行股份有限公司 | [应用商店](https://app.mi.com/details?id=cn.com.spdb.mobilebank.per) |
| 民生银行 | `cn.com.cmbc.newmbank` | 中国民生银行股份有限公司 | [应用商店](https://app.mi.com/details?id=cn.com.cmbc.newmbank) |
| 兴业银行 | `com.cib.cibmb` | 兴业银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.cib.cibmb) |
| 威海银行 | `com.iss.weihaibank` | 威海银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.iss.weihaibank) |
| 光大银行 | `com.cebbank.mobile.cemb` | 中国光大银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.cebbank.mobile.cemb) |
| 北京农商银行 | `cn.com.bjns.mbank` | 北京农村商业银行股份有限公司 | [应用商店](https://app.mi.com/details?id=cn.com.bjns.mbank) |
| 广发银行 | `com.cgbchina.xpt` | 广发银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.cgbchina.xpt) |
| 广东农信 | `com.csii.gdnx.mobilebank` | 广东省农村信用社联合社 | [应用商店](https://app.mi.com/details?id=com.csii.gdnx.mobilebank) |
| 福建农信 | `com.yitong.fjnx.mbank.android` | 福建省农村信用社联合社 | [应用商店](https://app.mi.com/details?id=com.yitong.fjnx.mbank.android) |
| 河南农商银行 | `com.hnnx.pmbank` | 河南农村商业银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.hnnx.pmbank) |
| 长沙银行 | `cn.com.csbank` | 长沙银行股份有限公司 | [应用商店](https://app.mi.com/details?id=cn.com.csbank) |
| 山东农信 | `com.android.clock.sd` | 山东省农村信用社联合社 | [应用商店](https://app.mi.com/details?id=com.android.clock.sd) |
| 宁波银行 | `com.nbbank` | 宁波银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.nbbank) |
| 上海银行 | `cn.com.shbank.mper` | 上海银行股份有限公司 | [应用商店](https://app.mi.com/details?id=cn.com.shbank.mper) |
| 四川农信（蜀信e） | `com.nxy.sc` | 四川农村商业联合银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.nxy.sc) |
| 北京银行 | `com.bankofbeijing.mobilebanking` | 北京银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.bankofbeijing.mobilebanking) |
| 浙江农信（丰收互联） | `com.yitong.zjrc.mfs.android` | 浙江农村商业联合银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.yitong.zjrc.mfs.android) |
| 中原银行 | `com.csii.zybk.ui` | 中原银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.csii.zybk.ui) |
| 网商银行 | `com.mybank.android.phone` | 浙江网商银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.mybank.android.phone) |
| 江西农商 | `com.jxnxs.mobile.bank` | 江西省农村信用社联合社 | [应用商店](https://app.mi.com/details?id=com.jxnxs.mobile.bank) |
| 江苏·农商行 | `com.yitong.mbank` | 江苏农村商业联合银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.yitong.mbank) |
| 广西农信 | `com.nxy.mobilebank.gx` | 广西农村商业联合银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.nxy.mobilebank.gx) |
| 吉林农信 | `com.jlnx.mbank` | 吉林省农村信用社联合社 | [应用商店](https://app.mi.com/details?id=com.jlnx.mbank) |
| 湖北农信 | `cn.com.hbnxmbank.Android` | 湖北省农村信用社联合社 | [应用商店](https://app.mi.com/details?id=cn.com.hbnxmbank.Android) |
| 常熟农商银行 | `com.csii.csbank` | 江苏常熟农村商业银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.csii.csbank) |
| 广州农商银行 | `com.gzrcb.mobilebank` | 广州农村商业银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.gzrcb.mobilebank) |
| 华夏银行 | `com.hxb.mobile.client` | 华夏银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.hxb.mobile.client) |
| 浙商银行 | `com.czbank.mbank` | 浙商银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.czbank.mbank) |
| 恒丰银行 | `com.hfbank.mobile` | 恒丰银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.hfbank.mobile) |
| 杭州银行 | `cn.com.hzb.mobilebank.per` | 杭州银行股份有限公司 | [应用商店](https://app.mi.com/details?id=cn.com.hzb.mobilebank.per) |
| 广州银行 | `com.gzbank.mbank.externalpk` | 广州银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.gzbank.mbank.externalpk) |
| 江苏银行 | `cn.jsb.china` | 江苏银行股份有限公司 | [应用商店](https://app.mi.com/details?id=cn.jsb.china) |
| 深圳农商银行 | `com.csii.sns.ui` | 深圳农村商业银行股份有限公司 | [应用商店](https://app.mi.com/details?id=com.csii.sns.ui) |
| 湖南农信 | `com.hnnx.eBank.android` | 湖南省农村信用社联合社 | [应用商店](https://app.mi.com/details?id=com.hnnx.eBank.android) |
| 安徽农金 | `com.ahrcu.mobilebank` | 安徽省农村信用社联合社 | [应用商店](https://app.mi.com/details?id=com.ahrcu.mobilebank) |
| 贵州农信（黔农云） | `csii.com.qny` | 贵州农村商业联合银行股份有限公司 | [应用商店](https://app.mi.com/details?id=csii.com.qny) |
| 陕西信合 | `com.sxnxs.mbank` | 陕西省农村信用社联合社 | [应用商店](https://app.mi.com/details?id=com.sxnxs.mbank) |
| 云南农信 | `com.csii.mobilebank` | 云南省农村信用社科技结算中心 | [应用商店](https://app.mi.com/details?id=com.csii.mobilebank) |
