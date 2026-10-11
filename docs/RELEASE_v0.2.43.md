# 有余记账 v0.2.43

> 本地搜索与统计优化，暂停深色主题

**开发体验版 · 功能更新** · 2026-10-11 · Android 8.0+ · 上一版 v0.2.42。

## 下载与升级

[下载 youyu-v0.2.43.apk](https://github.com/lyq-05/youyu-ledger/releases/download/v0.2.43/youyu-v0.2.43.apk) · **134.3 MiB**。

建议先在设置中导出本地备份，再同签名覆盖安装。无需卸载；本版统一恢复浅色主题。

## 本次更新

- **流水搜索**：默认搜索当前账本全部日期，支持备注、分类、账户与精确金额；可组合日期、金额范围、账户、分类及收支类型筛选。搜索结果显示数量和收支汇总，退出后恢复原浏览位置。
- **设置搜索**：输入“字体”“通知”“OCR”“备份”等名称或常用词，点击结果跳转到对应区域并短暂突出目标。
- **统计优化**：新增周统计、每日或每月收支趋势、分类占比；无记录日期补零，退款按原有规则冲减支出。
- **暂停深色主题**：移除开关，夜景图片与恢复参考保存在源码仓库的独立设计归档，不打入普通、测试或指南 APK。安装包比上一版减少约 15.0 MiB。
- 继续本地使用，不新增家庭共享、云同步或网络权限。

## 界面

以下截图来自独立指南应用，数据完全虚构。

| 流水搜索筛选 | 周收支趋势 |
| --- | --- |
| ![流水筛选](https://raw.githubusercontent.com/lyq-05/youyu-ledger/main/docs/screenshots/43-search-filter.png) | ![收支趋势](https://raw.githubusercontent.com/lyq-05/youyu-ledger/main/docs/screenshots/43-spending-trend.png) |

## 验证与已知限制

- 16 项搜索、筛选、设置索引及趋势统计检查通过，37 项核心单元测试通过。
- 模拟器检查搜索、筛选、设置定位和周趋势；核对普通及指南 APK 均不含夜景素材，签名与上一版一致。
- 搜索范围为当前账本已保存的流水，不跨账本，也不搜索原始通知或截图内容。
- 本次不改变自动记账规则。各银行、线下付款及跨渠道去重仍按既有计划等待真机验证，模拟样本不等于实际支付验证。

[项目首页](https://github.com/lyq-05/youyu-ledger) · [版本历史](https://github.com/lyq-05/youyu-ledger/blob/main/CHANGELOG.md) · [上一版](https://github.com/lyq-05/youyu-ledger/releases/tag/v0.2.42)
