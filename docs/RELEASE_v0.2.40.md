# 有余记账 v0.2.40

> 银行识别场景合并为一张卡片

**开发体验版** · Android 8.0+ · 上一版 v0.2.39。建议先导出本地备份，再同签名覆盖安装。

[下载 youyu-v0.2.40.apk](https://github.com/lyq-05/youyu-ledger/releases/download/v0.2.40/youyu-v0.2.40.apk)

安装包：140.8 MB。

## 本次更新

- 识别场景中的 48 张银行卡片合并为一张“银行”卡片，统一说明只显示一次，卡片内集中列出已支持的银行及农信应用名称。
- 银行卡片位于京东金融之后，减少查找距离。
- 各银行独立开关保留，默认收起，点击“管理银行渠道开关”展开；已有选择继续生效。

## 界面

独立指南应用截图，仅使用虚构测试数据：

<img src="https://raw.githubusercontent.com/lyq-05/youyu-ledger/main/docs/screenshots/07-bank-channels.png" width="320" alt="银行统一卡片及支持名单">

## 验证与范围

编译与安装包身份检查通过；在独立指南应用检查完整名单排版、开关展开／收起及选择保存。本次只调整界面组织，通知解析、已接入来源和去重逻辑未变。

已登记来源不代表真实通知格式已逐家实测，仍需银行发送可读取且匹配模板的扣款通知。[来源名单](https://github.com/lyq-05/youyu-ledger/blob/main/docs/BANK_NOTIFICATION_SOURCES.md)。

[上一版](https://github.com/lyq-05/youyu-ledger/releases/tag/v0.2.39)
