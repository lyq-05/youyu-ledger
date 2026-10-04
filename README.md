# 有余记账

<p align="center">
  <a href="https://github.com/lyq-05/youyu-ledger/releases"><img alt="版本" src="https://img.shields.io/github/v/release/lyq-05/youyu-ledger?include_prereleases&amp;sort=semver&amp;label=%E7%89%88%E6%9C%AC&amp;color=42684D"></a>
  <a href="https://github.com/lyq-05/youyu-ledger/releases"><img alt="总下载" src="https://img.shields.io/github/downloads/lyq-05/youyu-ledger/total?label=%E6%80%BB%E4%B8%8B%E8%BD%BD&amp;color=brightgreen"></a>
  <a href="https://github.com/lyq-05/youyu-ledger/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/lyq-05/youyu-ledger?style=social"></a>
  <a href="https://github.com/lyq-05/youyu-ledger/commits/main"><img alt="最后提交" src="https://img.shields.io/github/last-commit/lyq-05/youyu-ledger/main?label=%E6%9C%80%E5%90%8E%E6%8F%90%E4%BA%A4"></a>
  <img alt="平台 Android" src="https://img.shields.io/badge/%E5%B9%B3%E5%8F%B0-Android-3DDC84">
  <img alt="Android 8.0 及以上" src="https://img.shields.io/badge/Android-8.0%2B-3DDC84">
  <a href="https://github.com/lyq-05/youyu-ledger/releases/download/v0.2.10/youyu-v0.2.10.apk"><img alt="安装包 87.6 MB" src="https://img.shields.io/badge/%E5%AE%89%E8%A3%85%E5%8C%85-87.6%20MB-orange"></a>
  <img alt="开发体验版" src="https://img.shields.io/badge/%E7%8A%B6%E6%80%81-%E5%BC%80%E5%8F%91%E4%BD%93%E9%AA%8C%E7%89%88-d6a34a">
  <img alt="不联网" src="https://img.shields.io/badge/%E7%BD%91%E7%BB%9C-%E4%B8%8D%E8%81%94%E7%BD%91-lightgrey">
</p>

<p align="center">
  <b>收支有数，生活有余。</b><br>
  让日常账目成为手绘小镇里的一本生活记录。
</p>

Android 本地记账应用：手动入账、通知识别、图片补记与主动悬浮识别，共用“先核对、再入账”的流程。本仓库提供安装包与说明，暂不公开源码。

> 当前版本 **v0.2.10 · 悬浮核对窗口重做**：分类图标、固定保存栏；日期未识别默认今天，账户默认不使用。详见 [本次发布说明](docs/RELEASE_v0.2.10.md)。

---

## 下载

| 平台 | 安装包 | 大小 | 说明 |
| --- | --- | --- | --- |
| Android 8.0+ | **[⬇ youyu-v0.2.10.apk](https://github.com/lyq-05/youyu-ledger/releases/download/v0.2.10/youyu-v0.2.10.apk)** | 87.6 MB | 点击直接下载，无需 root |

[查看 Releases 与历史附件](https://github.com/lyq-05/youyu-ledger/releases)。旧版说明尽量保留，没有可用附件的版本不提供下载链接。

**安装步骤**

1. 下载 APK，在手机文件管理器中打开。
2. 如系统提示，允许当前来源安装应用，再继续安装。
3. 同签名体验版可直接覆盖；升级前请在设置中导出本地备份。若签名冲突，不要直接卸载。
4. 首次进入可查看指南，或跳过后开始手动记账。

---

## 界面

截图来自独立指南应用，仅使用虚构数据。

| 首页 | 操作指南引导 | 权限引导 |
| --- | --- | --- |
| ![首页](docs/screenshots/01-home.png) | ![指南引导](docs/screenshots/02-guide.png) | ![权限引导](docs/screenshots/02-permissions.png) |

## 功能

| 功能 | 说明 |
| --- | --- |
| 日常入账 | 选择账本、收支类型、分类与金额，账户可选 |
| 自动识别 | 按渠道开启通知识别；结果先进入待核对流程 |
| 历史补记 | 主动点击悬浮入口读取账单页，或从图片补记 |
| 流水与统计 | 月、年和自选日期统计，账户筛选与分类预算 |
| 账户与资金 | 转账、还款与退款；退款按退款日冲减支出 |
| 存钱计划 | 本地目标与分配记录，支持归档，不涉及真实划款 |
| 数据管理 | 本地备份恢复、自定义 CSV 导入、回收站恢复 |
| 桌面组件 | 快捷记账、收支预算与存钱愿望，金额默认隐藏 |
| 动态首页 | 静态街区背景与小鸟；可在设置中暂停小鸟 |

## 权限说明

| 权限 | 用途 | 是否必须 |
| --- | --- | --- |
| 通知使用权 | 读取所选渠道的支付通知 | 手动记账不需要 |
| 悬浮窗 | 显示识别入口和相关小窗 | 按需开启 |
| 屏幕共享 | 点击悬浮按钮时截取一帧并在本机识别 | 使用悬浮识别时按系统提示授权 |
| 无障碍服务 | 可选的单次页面文字读取 | 悬浮截图识别不需要 |

首次引导不会自动申请权限。悬浮识别的屏幕共享授权由点击入口触发。点击“现在去设置”后，在权限与识别状态页逐项配置。应用清单移除了联网权限；图片识别在本机进行。账务与备份保存在本机，请妥善保管明文导出文件。

## 常见问题

**不设置权限能记账吗？** 可以，手动入账不依赖通知或无障碍权限，付款／收款账户也可暂不选择。

**为什么没有识别成功？** 检查渠道开关、对应权限和系统后台限制；不是所有通知或页面都包含完整账单字段，可改用图片补记或手动录入。

**首页动态卡顿怎么办？** 在“设置 → 首页动态”开启“减少动态效果”。

**这是正式版吗？** 当前为开发体验版，使用调试签名。真实支付通知、页面读取、厂商后台策略及动画真机流畅度、耗电和温升仍需验证。识别结果需要核对后入账；自定义 CSV 导入不等于兼容支付宝或微信的原始导出文件。

## 版本历史

见 [CHANGELOG.md](CHANGELOG.md)，逐版说明如下：

| 版本 | 主题 |
| --- | --- |
| [v0.2.10](docs/RELEASE_v0.2.10.md) | 悬浮核对窗口重做 |
| [v0.2.9](docs/RELEASE_v0.2.9.md) | 手写字体账单识别修正 |
| [v0.2.8](docs/RELEASE_v0.2.8.md) | 松鼠主角首次接入 |
| [v0.2.7](docs/RELEASE_v0.2.7.md) | 静态首页与小鸟保留 |
| [v0.2.6](docs/RELEASE_v0.2.6.md) | 主动识别字段容错 |
| [v0.2.5](docs/RELEASE_v0.2.5.md) | 悬浮识别与屏幕授权 |
| [v0.2.4](docs/RELEASE_v0.2.4.md) | 首次引导顺序与发布说明 |
| [v0.2.3](docs/RELEASE_v0.2.3.md) | 首页同步微风与小鸟动态 |
| [v0.2.2](docs/RELEASE_v0.2.2.md) | 花草边角与更新说明 |
| [v0.2.1](docs/RELEASE_v0.2.1.md) | 首页标志与版本信息 |
| [v0.2.0-preview](docs/RELEASE_v0.2.0-preview.md) | 本地功能与图文指南完善 |

反馈问题时请遮挡订单号、账号等个人信息，不要将真实账单上传到公开 Issue。
