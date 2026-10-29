# IPADownNext

English | [简体中文](#简体中文)

**v1.0.1 — First official release**

IPADownNext is a Windows tool for finding and downloading historical App Store IPA versions and transferring IPA files over a local network.

The app uses Semantic Versioning: increment the patch number for bug fixes, the minor number for compatible features, and the major number for significant breaking changes. Multiple builds in one iteration keep the same product version and use a separate build identity such as `20261029.1`, `20261029.2`. Velopack compares product versions, so builds with the same product version do not auto-update users already on that version.

## Download

Visit the [latest GitHub Releases page](https://github.com/qishouvip/IPADownNext-Releases/releases/latest) and download one of these files:

- **Installer:** `IPADownNext.Desktop-win-Setup.exe`, recommended for most users.
- **Portable:** `IPADownNext.Desktop-win-Portable.zip`, extract and run without installation.
- **Update files:** used by the in-app Velopack updater; most users do not need to download them manually.

The installed Windows version checks for updates at startup. It shows the version and release notes, then downloads and restarts only after you confirm. You can also check for updates from About.

## Features

- Search App Store apps and see available historical versions.
- Use an Apple account to view and download authorized IPA versions.
- Manage local Apple accounts and download tasks.
- Transfer IPA files to a mobile device using a local-network QR code.

## Getting started

1. Download and run the Windows installer.
2. Add and sign in to your Apple account in Accounts.
3. Search for an app and open Version History.
4. Select an available version and download it. Results depend on account authorization, storefront availability, and Apple service status.
5. To transfer an IPA to a device on the same local network, open Device Transfer, select the IPA, and follow the page instructions.

The app supports Simplified Chinese and English. By default, it follows the Windows display language; unsupported languages use English. App Store search follows the interface language by default (China mainland for Chinese and the United States for English). A manually selected storefront is saved.

Sign-in and downloads require access to Apple services. Never include Apple passwords, verification codes, session files, or other account credentials in issue reports.

## FAQ

### Why can't I find an older version?

Whether a version is visible or downloadable depends on Apple's store data, account authorization, and service status. The app cannot guarantee a complete history for every app or bypass Apple's access controls.

### Will the app install updates automatically?

No. The app checks for and shows updates, but asks before downloading and restarting to install them. Portable builds do not support in-app Velopack updates; download and replace the portable archive manually.

### How do users of earlier date-based versions switch to the public update source?

Download and install the latest installer from this page once. Earlier date-based releases cannot be updated in place by the new Semantic Versioning sequence. After installing `v1.0.1` or later, the app can check for higher product versions through the public release repository.

### Where are accounts, sessions, and settings stored?

Data is stored under `%LOCALAPPDATA%\IpaDownNext` for the current Windows user, separately from the application directory. Do not upload the account data folder to a public repository or issue report.

### Can the local-network QR code install an iOS app?

No. It transfers the IPA to the device but does not install it. Wireless iOS installation also requires suitable HTTPS, certificates, signing, and provisioning. An ordinary App Store IPA is not guaranteed to support sideloading.

### How do I report a problem?

Open an issue in the [public release repository](https://github.com/qishouvip/IPADownNext-Releases/issues). Include the app version, reproduction steps, and redacted error details. Do not attach passwords, verification codes, session files, or other account credentials.

## Disclaimer

IPADownNext is an independent third-party tool and is not affiliated with, endorsed by, or partnered with Apple Inc. or the App Store. It is only for viewing and downloading content authorized for the current account. It does not provide purchases, cracking, signing, or access-control circumvention. Apple may change its services, APIs, or account rules, and the developer cannot guarantee that a particular version will remain available. Follow Apple's terms of service and applicable laws.

---

Developer: Alexander Chen · Email: qishouvip@gmail.com

## Security and limitations

The local account folder contains sensitive session data, including cookie caches. Protect it and never share it. A local SHA-256 fingerprint is not proof of source integrity. Download queues are not restored after restarting the app.

---

## 简体中文

**v1.0.1 — 正式首版**

IPADownNext 是一款面向 Windows 的 App Store IPA 历史版本查询、下载与局域网传输工具。

版本号遵循语义化版本：修复问题且不改变现有功能时增加修订号；新增兼容功能时增加次版本号；重大不兼容变更时增加主版本号。同一轮迭代的多次构建保持相同产品版本，构建号单独递增，例如 `20261029.1`、`20261029.2`。Velopack 按产品版本比较更新；相同产品版本的构建不会自动更新已安装同版本的用户。

## 下载

前往 [GitHub Releases 最新版本页](https://github.com/qishouvip/IPADownNext-Releases/releases/latest)，下载：

- **安装版**：`IPADownNext.Desktop-win-Setup.exe`，推荐大多数用户使用。
- **便携版**：`IPADownNext.Desktop-win-Portable.zip`，解压后运行，不执行安装流程。
- **更新文件**：由应用内 Velopack 更新功能使用，普通用户无需手动下载。

Windows 安装版启动时会检查更新。发现新版本后会展示版本和更新说明；只有你确认后，应用才下载并重启安装。也可以在“关于软件”中手动检查更新。

## 主要功能

- 搜索 App Store 应用并查看可用的历史版本。
- 使用 Apple 账号查询并下载获授权的 IPA 版本。
- 管理本机 Apple 账号和下载任务。
- 通过局域网二维码把 IPA 文件传到移动设备。

## 使用方法

1. 下载并运行 Windows 安装版。
2. 在“账号管理”中添加并登录自己的 Apple 账号。
3. 在“软件搜索”中查找应用，打开“历史版本”。
4. 选择可用版本并下载；账号授权、商店可用性和 Apple 服务状态会影响结果。
5. 如需传到同一局域网的设备，打开“设备传输”，选择 IPA 并按页面提示操作。

软件支持简体中文和 English，默认跟随 Windows 首选显示语言，其他系统语言默认使用英文。App Store 搜索地区默认随界面语言选择：中国大陆或美国；手动选择地区会保存。

首次登录和下载需要访问 Apple 服务。请勿把 Apple 密码、验证码、会话文件或其他账号凭据提交到问题反馈中。

## 常见问题

### 为什么查不到某个旧版本？

历史版本是否可见、是否允许当前账号下载由 Apple 的商店数据、账号授权和服务状态决定。本软件不能保证每个应用都存在完整历史记录，也不能绕过 Apple 的访问控制。

### 新版本发布后，应用会自动安装吗？

不会。应用只检查并展示更新；下载和重启安装前会先征求确认。便携版不支持应用内 Velopack 更新，请下载新版便携包手动替换。

### 旧版 2026.10.29 用户如何切换到公开更新源？

请从本页面下载最新版安装包并手动安装一次。旧版使用日期版本号，无法通过新的语义版本号序列原位更新。安装 `v1.0.1` 或更新版本后，应用即可从公开发布仓库检查更高产品版本。

### 账号、会话和设置存在哪里？

数据保存在当前 Windows 用户的 `%LOCALAPPDATA%\IpaDownNext`，与程序安装目录分开。请勿将账号目录上传到公开仓库或问题反馈。

### 局域网二维码能直接安装 iOS 应用吗？

不能。二维码只用于把 IPA 下载到设备，不表示应用已安装。iOS 无线安装还需要符合要求的 HTTPS、证书、签名和描述文件；普通 App Store IPA 不保证可以侧载。

### 如何反馈问题？

请在 [公开仓库 Issues](https://github.com/qishouvip/IPADownNext-Releases/issues) 提交问题。写明应用版本、操作步骤和脱敏后的错误信息，不要附上 Apple 密码、验证码、会话文件或其他账号凭据。

## 免责声明

IPADownNext 是独立的第三方工具，与 Apple Inc. 或 App Store 无隶属、认可或合作关系。软件仅用于查询和下载当前账号获授权的内容，不提供购买、破解、签名或绕过访问控制的功能。Apple 可能调整服务、接口或账号规则；开发者不能保证特定版本持续可用。请遵守 Apple 服务条款及适用法律。

---

开发者：Alexander Chen · 联系邮箱：qishouvip@gmail.com

### 安全与使用边界

本机账号目录包含 Cookie 等敏感会话缓存，请妥善保护，切勿分享。下载后的本地 SHA-256 是文件指纹，不代表来源完整性验证。重启程序后不恢复下载队列。

