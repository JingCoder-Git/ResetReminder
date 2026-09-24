# ResetReminder

[中文](#中文) · [English](#english)

## 中文

ResetReminder 是一款面向 Codex 用户的 macOS / Windows 桌面工具。它会读取当前 Codex 账号的重置额度信息，在额度即将过期前显示倒计时和系统通知，帮助你及时使用额度，避免它悄悄失效。

### 主要优点

- **到期提醒**：自动按紧急程度整理重置额度，并在临近到期时发送系统通知。
- **隐私优先**：通过 Codex `app-server` 获取额度信息，不读取 Codex 认证文件。
- **支持直连与代理场景**：可直接同步，也可通过本地文件收件箱完成离线交接。
- **轻量常驻**：以托盘 / 菜单栏为中心运行，支持登录时启动和后台定时检查。
- **中英双语**：应用界面可在中文和英文之间切换。
- **本地数据**：“标记已使用”只影响本地记录，不会消耗账号额度。

### 下载与安装

请前往 [Releases](https://github.com/JingCoder-Git/ResetReminder/releases/latest) 下载当前平台的安装包。

> [!IMPORTANT]
> 当前 v0.1.0 未进行 Apple Developer ID 签名、公证或 Windows 代码签名。因此 macOS Gatekeeper 或 Windows SmartScreen 可能显示安全警告。请只从本仓库的 Releases 页面下载，并在继续安装前核对发布页中的 SHA-256 校验值。

#### macOS

1. 下载 `.dmg`，打开后将 ResetReminder 拖入“应用程序”。
2. 如果系统阻止首次打开，请在 Finder 中按住 Control 键点按应用并选择“打开”；或前往“系统设置 → 隐私与安全性”，确认应用来源后选择“仍要打开”。
3. 首次运行时，根据系统提示授予通知权限。

#### Windows

1. 下载并运行 `ResetReminder.Setup.0.1.0.exe`。
2. 如果 Microsoft Defender SmartScreen 显示“Windows 已保护你的电脑”，请先确认文件来自本仓库的 Release 且校验值一致，再选择“更多信息 → 仍要运行”。
3. 首次运行时，根据系统提示允许通知。

### 使用要求

- 已安装当前版本的 Codex Desktop 或 Codex CLI。
- Codex 已登录 ChatGPT 账号。
- 在线读取需要能够访问 `https://chatgpt.com/`；代理不常驻时可使用应用内的本地收件箱同步功能。

---

## English

ResetReminder is a macOS and Windows desktop companion for Codex users. It reads reset-credit information for the current Codex account, shows a clear expiry countdown, and sends system notifications before credits expire.

### Why ResetReminder

- **Expiry alerts**: Organizes reset credits by urgency and sends notifications as expiration approaches.
- **Privacy first**: Reads credit information through Codex `app-server` without accessing Codex authentication files.
- **Direct and proxy-friendly**: Supports direct sync as well as a local file inbox for offline handoff workflows.
- **Tray-first and lightweight**: Runs from the system tray / menu bar, with launch-at-login and quiet background checks.
- **Bilingual UI**: Switch between Chinese and English in the app.
- **Local data**: “Mark used” is local tracking only and never consumes account credits.

### Download and install

Download the installer for your platform from [Releases](https://github.com/JingCoder-Git/ResetReminder/releases/latest).

> [!IMPORTANT]
> Version 0.1.0 is not signed, notarized with Apple, or Windows code-signed. macOS Gatekeeper or Windows SmartScreen may therefore show a security warning. Download only from this repository’s Releases page and verify the SHA-256 checksum shown in the release notes before installing.

#### macOS

1. Download the `.dmg`, open it, and drag ResetReminder into Applications.
2. If macOS blocks the first launch, Control-click the app in Finder and choose **Open**. Alternatively, review it under **System Settings → Privacy & Security** and choose **Open Anyway** only after confirming the source.
3. Allow notifications when macOS asks.

#### Windows

1. Download and run `ResetReminder.Setup.0.1.0.exe`.
2. If Microsoft Defender SmartScreen shows “Windows protected your PC,” first confirm that the file came from this repository’s Release and that its checksum matches. Then choose **More info → Run anyway**.
3. Allow notifications when Windows asks.

### Requirements

- A current Codex Desktop or Codex CLI installation.
- Codex signed in to a ChatGPT account.
- Online reads require access to `https://chatgpt.com/`. If a proxy is not always available, use the app’s local file-inbox sync workflow.
