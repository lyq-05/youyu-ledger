# 有余记账 v0.2.77

> 周期记账、图片备注与存钱计划升级

**开发体验版** · 2026-10-16 · Android 8.0+ · 上一版 v0.2.76。

## 下载与升级

[下载 youyu-v0.2.77.apk](https://github.com/lyq-05/youyu-ledger/releases/download/v0.2.77/youyu-v0.2.77.apk)（73.4 MiB）。同签名体验版可覆盖安装，升级前请在设置中导出完整备份；签名冲突时不要直接卸载。新版备份包含新增计划与图片，旧版应用不支持恢复新版备份。

## 本次更新

- 新增周期记账：支持房租、工资等按周、月、年生成待确认账单，金额可留空；支持暂停、跳过与结束，确认后才计入收支。
- 新增图片备注：每笔最多 3 张，压缩后保存在本机并纳入完整备份；入口位于备注旁，手动、自动与悬浮核对面板均可使用。
- 新增账本统计月起始日设置，月度流水、统计、日历、预算和桌面组件按同一周期展示。
- 存钱计划支持自由攒钱、定额攒钱和按期达标，设置目标、日期与日/周/月频率，显示建议存入金额；记录存入不自动记作收入或支出。
- 小荷包仅提供文字路径：支付宝 → 支付宝小荷包 → 新建荷包 → 命名 → 自定义存钱计划。尚未绑定，不会同步余额或真实划款。
- 收紧记账分类与周期计划表单间距，更新操作指南至 11 个主题、41 个图文页面。
- 京东白条成功页优先识别“白条付款”金额，避免自动还款推广与推荐商品价格干扰。
- 修复悬浮核对保存时后台计划调度可能引起数据库锁冲突的问题。

## 界面

| 存钱方式 | 周期计划 | 图片备注 |
| --- | --- | --- |
| ![存钱方式](https://raw.githubusercontent.com/lyq-05/youyu-ledger/main/docs/screenshots/04-saving-modes.webp) | ![周期计划](https://raw.githubusercontent.com/lyq-05/youyu-ledger/main/docs/screenshots/05-recurring.webp) | ![图片备注](https://raw.githubusercontent.com/lyq-05/youyu-ledger/main/docs/screenshots/06-photo-entry.webp) |

## 验证与限制

- 89 项核心测试通过；已完成周期计划、存钱计划、图片与备份迁移、悬浮核对的针对性模拟器检查，并非全量回归测试。
- Release 构建完成，测试工具关闭，包名与上一版签名一致。
- 京东白条规则尚待真机支付验证；重新进入旧成功页与首次支付成功分别验收，不能视为同一测试。
- 图片完整备份仍受 20 MiB 文件上限约束。周期账单不代表真实扣款，系统后台限制可能影响生成时机，进入应用会补查。

## 相关链接

[项目首页](https://github.com/lyq-05/youyu-ledger) · [版本历史](https://github.com/lyq-05/youyu-ledger/blob/main/CHANGELOG.md) · [上一版本](https://github.com/lyq-05/youyu-ledger/releases/tag/v0.2.76)
