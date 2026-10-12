<p align="center">
  <img src="https://github.com/kanatallow/Open-Meets/releases/download/v0.12.3/Open-Meets-icon.png" width="180" alt="Open Meets">
</p>

<h1 align="center">Open Meets</h1>

<p align="center">把 Meets / On 装进口袋。<br>Take your Meets / On with you.</p>

<p align="center">
  <a href="https://github.com/kanatallow/Open-Meets/releases/latest">下载最新版 · Download</a> ·
  <a href="#english">English</a> ·
  <a href="https://github.com/kanatallow/Open-Meets/issues">问题反馈 · Feedback</a>
</p>

Open Meets 是面向 Android 手机和平板的 Tamagotchi Meets / On 模拟器。导入自己的 ROM，在手机上继续养育、保存进度、切换版本，也可以通过 WebMeets 接收礼物。

**免费使用 · Android 8.0+ · ARM64 · 中文 / English**

本仓库用于发布安装包、更新说明和使用指南，不公开应用源代码。安装包不附带 ROM 或测试存档。

## 下载与安装

当前版本：**0.12.3（build 17）**。

| 版本 | 下载 | 适用场景 |
| --- | --- | --- |
| 标准版 | [Open-Meets-0.12.3-arm64.apk](https://github.com/kanatallow/Open-Meets/releases/download/v0.12.3/Open-Meets-0.12.3-arm64.apk) · 1.8 MiB | 日常养育、后台提醒、存档管理、WebMeets 蓝牙收礼 |
| Mixing Meets 合并版 | [Open-Meets-0.12.3-Mixing-arm64.apk](https://github.com/kanatallow/Open-Meets/releases/download/v0.12.3/Open-Meets-0.12.3-Mixing-arm64.apk) · 86.5 MiB | 包含标准版功能，并内置 64 位 Mixing Meets 客户端；实验性版本 |

1. 下载一个 APK，传到 Android 设备并安装。仅在安装时按系统提示允许所用浏览器或文件管理器安装应用。
2. 打开 **Open Meets**，导入自己的 ROM 或未加密 ZIP。ZIP 中的受支持 `.bin` 文件会自动识别，可一次导入多个版本。
3. 允许通知，在 **⋯ → 后台养育与提醒** 中查看本机品牌的后台设置指引。

**升级请直接覆盖安装，先导出存档备份，不要卸载旧版。** 两个版本使用同一应用 ID 和签名，共用本地 ROM 与进度，不能同时作为两个独立应用安装。若设备拒绝切换安装包，请保留现有安装和存档。

合并版在系统应用信息中可能显示 **1.4.3**，这是内置 Mixing Meets 客户端的兼容编号；本次发行对应 **build 17**。

## 功能

- **ROM / ZIP 导入与版本切换**：导入后保存在应用内的 ROMs 列表，各版本分别保存进度。
- **即时存档**：运行时每 30 秒自动保存，支持手动保存、导出备份和导入同版本 `.t18s` 存档。
- **后台养育与呼叫提醒**：锁屏后继续养育，可随时从设置或常驻通知暂停。
- **两种外观**：真机蛋形外壳与极简大屏，共享同一份进度。
- **中文 / English 界面**：菜单、帮助和通知可切换语言；游戏文字由 ROM 决定。
- **手机与平板适配**：横竖屏、圆形 A/B/C 按键、多点触控 A+C。
- **WebMeets 收礼**：通过蓝牙从另一台设备上的 WebMeets 接收物品。
- **可选 Mixing Meets**：合并版从游戏内 App 的“去玩 / Visit”或“接收礼物 / Present”进入内置客户端。

## 快速上手

**操作**：A 选择，B 确认，C 返回。支持长按和 A+C 同时按下；游戏屏幕休眠后按任意键唤醒。

**切换 ROM**：打开 **⋯ → 切换 ROM**，直接点选已导入的版本，也可继续导入 ROM 或 ZIP。只有当前版本继续养育，其他版本在重新打开时只同步时钟。

**保存与恢复**：在设置中导出 `.t18s` 备份；导入时使用与当前 ROM 版本匹配的存档。卸载应用会删除本地 ROM 和进度。

**后台运行**：默认开启后台养育。保持 ROM 内的声音开启以检测呼叫；应用菜单中的静音仍可保留安静通知。暂停、强行停止、重启或系统清理期间不补算养育，重新打开时只补时钟。后台持续运行会增加耗电。

## WebMeets 与 Mixing Meets

### WebMeets 蓝牙收礼

1. 在游戏内选择 **连接 → 下载 / ダウンロード / Download**。
2. 开启蓝牙，允许应用请求的“附近的设备”权限。
3. 在 **Mac 或另一台 Android 设备的 Chrome** 中打开 [WebMeets](https://tamagotchicenter.com/webmeets/items)。
4. 选择物品，连接蓝牙设备 **TMGC_meets**，完成发送。

接收设备需支持 BLE 外设广播。接收时蓝牙名称会临时改为 `TMGC_meets`，结束后恢复。成功后自动保存，取消或中断会恢复连接前的进度。

### 内置 Mixing Meets

安装合并版后，从游戏内 **App → 去玩 / Visit** 或 **接收礼物 / Present** 进入。客户端已适配 ARM64，在线功能依赖 Mixing Meets 社区服务。可通过 [Mixing Meets 支持页面](https://mixing-meets.com/support)支持社区运营。

WebMeets 收礼和 Mixing Meets 往返已完成 Android 模拟器链路验证；实体设备的蓝牙与系统兼容性仍需进一步验证。当前不支持红外或与实体玩具直连，Mixing Meets 婚配尚未完成验证。

## 支持的 ROM

| 系列 | 版本 |
| --- | --- |
| Tamagotchi ON（英文） | Fairy、Magic、Wonder Garden |
| Tamagotchi MEETS（日文） | Fairy、Magical、Pastel、Sanrio、Sweets、Fantasy |

暂不支持 Tamagotchi SOME（韩文）。ROM 由用户自行提供。

## 反馈与致谢

遇到问题请[提交 Issue](https://github.com/kanatallow/Open-Meets/issues)，附上设备型号、Android 版本、安装包版本和复现步骤。请勿附带 ROM、个人存档或账号凭据。

模拟器基于 [oreo-fox/tg18-emu](https://github.com/oreo-fox/tg18-emu)，感谢上游作者、WebMeets 和 Mixing Meets 社区。上游 MIT 许可及其他组件许可保留在应用中。

Open Meets 免费提供，仅供非商业使用，禁止倒卖、收费分发、付费激活、广告变现及商业捆绑。许可全文见应用内许可页面。本项目与 Bandai 无隶属或认可关系；Tamagotchi 为其相关权利人的商标。

<p align="center"><em>Designed by Kanata with Pride and Joy</em></p>

---

## English

**Open Meets** brings Tamagotchi Meets / On to Android phones and tablets. Import your own ROM, care for your pet, keep separate progress for each version, and receive gifts through WebMeets.

This repository hosts downloads, release notes and user documentation. Application source code is not published here. No ROMs or sample saves are included.

### Download

**Android 8.0 or later · ARM64 · Release 0.12.3 / build 17**

- [Standard edition — 1.8 MiB](https://github.com/kanatallow/Open-Meets/releases/download/v0.12.3/Open-Meets-0.12.3-arm64.apk): emulator, background care, notifications, save management and WebMeets BLE reception.
- [Mixing Meets edition — 86.5 MiB](https://github.com/kanatallow/Open-Meets/releases/download/v0.12.3/Open-Meets-0.12.3-Mixing-arm64.apk): includes the standard features and an embedded ARM64 Mixing Meets client. Experimental.

Install one APK, open **Open Meets**, and import your own ROM or an unencrypted ZIP. Choose English on the welcome screen or under **Settings → Language**. Game text follows the ROM language.

**Back up your save and update over the existing installation. Do not uninstall first.** Both editions share the same app identity, signing certificate and local progress. They cannot be installed side by side. If Android rejects an edition switch, keep the current installation and saves. The Mixing edition may display **1.4.3** in system app information for client compatibility; this release is **build 17**.

### Everyday use

- **Controls:** A selects, B confirms, C goes back. Hold A+C together when needed; press any button to wake the display.
- **Appearance:** choose Device or Minimal in Settings without changing your progress.
- **ROM library:** import individual ROMs or ZIPs, then switch from the saved ROMs list. Each version keeps separate progress; only the selected version continues care.
- **Saves:** autosave runs every 30 seconds. Export a `.t18s` backup or import one matching the current ROM version from Settings.
- **Background care:** allow notifications and follow the device guide in Settings. Keep sound enabled inside the game for call detection. Pause from Settings or the persistent notification. Interrupted or paused time advances the clock only, without simulating offline care.

### Connections

For **WebMeets**, choose **Connection → Download** in the game, enable Bluetooth and allow Nearby devices. Open [WebMeets](https://tamagotchicenter.com/webmeets/items) in Chrome on a Mac or another Android device, select an item and connect to **TMGC_meets**. The receiving device must support BLE peripheral advertising. Its Bluetooth name changes temporarily during reception and is restored afterward.

In the **Mixing edition**, **App → Visit** and **App → Present** open the embedded client. Online features depend on the Mixing Meets community service; [support the community here](https://mixing-meets.com/support).

WebMeets gift reception and Mixing Meets visit/return have been checked through Android emulator integration tests. Physical-device Bluetooth and compatibility need further testing. Infrared and direct links to physical toys are unsupported; Mixing Meets marriage has not yet been validated.

Supported ROMs: **ON** Fairy, Magic and Wonder Garden (English); **MEETS** Fairy, Magical, Pastel, Sanrio, Sweets and Fantasy (Japanese). Korean **SOME** ROMs are not supported.

### Feedback and credits

[Report an issue](https://github.com/kanatallow/Open-Meets/issues) with your device, Android version, edition and reproduction steps. Do not attach ROMs, personal saves or account credentials.

Based on [tg18-emu by oreo-fox](https://github.com/oreo-fox/tg18-emu), with thanks to the WebMeets and Mixing Meets communities. Upstream and third-party license notices are included in the app.

Free for noncommercial use. No resale, paid distribution, activation fees, advertising monetization or commercial bundling. See the in-app license page for the terms. This project is not affiliated with or endorsed by Bandai.
