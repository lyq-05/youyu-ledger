# 有余记账 v0.2.3

首页微风与小鸟动态更新 · 开发体验版

上一版本：v0.2.2。系统要求：Android 8.0 及以上。

## 下载

| 平台 | 安装包 | 大小 |
| --- | --- | --- |
| Android 8.0 及以上 | [下载 youyu-v0.2.3.apk](https://github.com/lyq-05/youyu-ledger/releases/download/v0.2.3/youyu-v0.2.3.apk) | 91.2 MB |

## 升级说明

本包沿用之前体验版的包名与签名，可覆盖安装。升级前请先在设置中导出备份；不要通过卸载解决签名冲突。

## 较上一版更新

1. 首页加入左上、左下、右下三处同步微风动画。
2. 小鸟随机飞入、落脚与飞出，加入张望、啄笔、整理羽毛和抖羽动作。
3. 设置增加“首页动态 → 减少动态效果”，可切回静态首页。
4. 动画在离开首页、失去窗口焦点或进入后台时暂停；装饰层不拦截按钮点击。
5. 使用异步解码、相邻帧预取和有上限的缓存，减少重复绘制。

## 已完成验证与已知限制

核心测试 17 项通过；完成动画帧解码、动作边界、持久化和入口点击检查，APK 签名验证通过。

这是开发体验版，使用现有体验包签名与包名（app.youyu.ledger.preview），不是应用商店正式版。模拟器仍存在慢帧，真机流畅度、耗电和发热待验证；可在设置中开启“减少动态效果”。支付通知、悬浮识别受权限、渠道页面与系统后台限制影响，仍需实机验证，识别后请核对金额、类型和账户。

## 界面

<img src="https://raw.githubusercontent.com/lyq-05/youyu-ledger/main/docs/screenshots/01-home.png" alt="虚构数据首页" width="360">

## 校验

SHA256（youyu-v0.2.3.apk）：

```text
9b7e84816856984b7ea38d0c02564fa210672a2840e8323018742c1959d5e897
```

[项目首页](https://github.com/lyq-05/youyu-ledger) · [完整变更历史](https://github.com/lyq-05/youyu-ledger/blob/main/CHANGELOG.md)
