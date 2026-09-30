# Recall FC 官方项目

本仓库是 Recall FC（足一把）的官方公开项目与 Android 发行地址，用于集中提供官方网站入口、正式安装包、版本说明、文件校验信息和 App 更新状态。

[![在线游玩](https://img.shields.io/badge/在线游玩-playzuyiba.com-C9FF4A?style=for-the-badge&labelColor=111411)](https://playzuyiba.com)
[![下载 Android](https://img.shields.io/badge/下载-Android_v0.16.0-C9FF4A?style=for-the-badge&logo=android&logoColor=111411&labelColor=111411)](https://github.com/shenshiaba/recall-fc/releases/latest/download/Recall-FC-Android.apk)

Recall FC 是一款足球球员猜谜游戏，目前提供每日挑战、练习和在线对战。产品功能请以官方网站及应用内实际页面为准。

## 产品能力

- **每日挑战与练习**：围绕真实足球球员资料设计持续更新的猜谜内容。
- **多语言检索**：支持中英文球员搜索与输入提示，降低不同用户的检索成本。
- **实时在线对战**：提供大厅匹配、房间邀请、断线重连、观战与对局回看。
- **竞技系统**：包含排位积分、赛季排行、个人战绩与账号统计。
- **跨端体验**：Web 端可直接游玩，Android 客户端提供原生分享、触感反馈和网络状态提示。

## 工程与交付

产品使用 React、TypeScript、Cloudflare Workers、D1 和 Drizzle ORM 构建 Web 与服务端能力，并通过 Capacitor 封装 Android/iOS 客户端。生产交付覆盖数据库迁移、正式包签名、版本校验、GitHub Releases 和 Android 签名差分更新。

## Web 与 Android

| 版本 | 地址 | 说明 |
| --- | --- | --- |
| Web | [playzuyiba.com](https://playzuyiba.com) | 无需安装，浏览器直接游玩 |
| Android | [最新正式 APK](https://github.com/shenshiaba/recall-fc/releases/latest/download/Recall-FC-Android.apk) | 官方上传证书签名版本 |

### Android v0.16.0

- 包名：`com.recallfc.app`
- 最低系统：Android 7.0
- 版本代码：`16`
- APK SHA-256：`f1d4be3584371e41268734252762f5da68f5f00cdd82f2a7afba432a5acb1443`
- APK 签名：Signature Scheme v2 / v3

安装时，Android 可能要求允许浏览器安装来自此来源的应用。请只从本仓库 Releases 或 Recall FC 官网下载安装包。

## App 更新

Android App 已启用签名差分更新：普通界面和游戏资源更新可以只下载发生变化的文件；涉及 Android 原生代码、权限或插件的变化仍通过新的正式 APK 发布。

- 当前生产更新状态：[production.json](https://playzuyiba.com/app-updates/android/production.json)
- 正式版本与更新记录：[GitHub Releases](https://github.com/shenshiaba/recall-fc/releases)

## 仓库用途与公开范围

本仓库主要公开：

- 产品介绍和官方入口
- Android 正式安装包
- 版本说明与更新记录
- App 线上更新状态
- 安全反馈说明

Web/App 业务源码、服务端配置、账号配置、签名私钥和内部运营资料不在公开范围内。

## 授权说明

本仓库未附带开源许可证。公开展示不代表 Recall FC 的代码、名称、标志、视觉资产或内容被授权复制、修改、重新打包或再发行。

## 安全问题

请阅读 [SECURITY.md](SECURITY.md)。请勿在公开 Issue 中提交账号、验证码、访问令牌、私钥或其他敏感信息。
