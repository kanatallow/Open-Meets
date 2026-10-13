<p align="center">
  <img src="https://github.com/kanatallow/Open-Meets/releases/download/v0.16.0/Open-Meets-icon.png" width="180" alt="Open Meets">
</p>

<h1 align="center">Open Meets</h1>

<p align="center">把 Meets / On 装进口袋。<br>Take your Meets / On with you.</p>

<p align="center">
  <a href="https://github.com/kanatallow/Open-Meets/releases/latest">下载最新版 · Download</a> ·
  <a href="#english">English</a> ·
  <a href="https://github.com/kanatallow/Open-Meets/issues">问题反馈 · Feedback</a>
</p>

Open Meets 是面向 Android 手机和平板的 Tamagotchi Meets / On 模拟器。导入自己的 ROM，在手机上继续养育、保存进度、切换版本，也可以通过 WebMeets 接收礼物。

**免费使用 · Android 8.0+ · ARM64 · 正式版 0.3.0**

**支持简体中文和英文界面。English UI is supported.** Choose **English** on the welcome screen or under **⋯ → 语言 / Language**. Menus, help and notifications are available in English; game text follows your ROM.

本版修复游戏内相机无法使用的问题，为智能手表和折叠屏外屏新增小屏模式，并支持一键截屏，记录宝宝的精彩瞬间。保留完整的 64 位 Mixing Meets 客户端。

**强烈建议华为鸿蒙用户关闭后台驻留，采用普通模式，确保关闭程序后养育时间仍与现实时间同步，宠物正常成长。**

本仓库用于发布安装包、更新说明和使用指南，不公开应用源代码。安装包不附带 ROM 或测试存档。

## 下载与安装

当前正式版：**Open Meets 0.3.0**。

**[下载 Open-Meets-0.3.0-arm64.apk · 86.6 MiB](https://github.com/kanatallow/Open-Meets/releases/download/v0.3.0/Open-Meets-0.3.0-arm64.apk)**

包含日常养育、后台提醒、存档管理、WebMeets 收礼与内置 Mixing Meets 客户端。

1. 下载 APK，传到 Android 设备并安装。仅在安装时按系统提示允许所用浏览器或文件管理器安装应用。
2. 打开 **Open Meets**，导入自己的 ROM 或未加密 ZIP。ZIP 中的受支持 `.bin` 文件会自动识别，可一次导入多个版本。
3. 允许通知和系统的“闹钟与提醒”，在 **⋯ → 后台养育与提醒** 中选择养育模式。

**升级请直接覆盖安装，先导出存档备份，不要卸载旧版。** 沿用原应用 ID 和签名，保留本地 ROM 与进度。

## 功能

- **ROM / ZIP 导入与版本切换**：导入后保存在应用内的 ROMs 列表，各版本分别保存进度。
- **即时存档**：运行时每 30 秒自动保存，支持手动保存、导出备份和导入同版本 `.t18s` 存档。
- **普通模式**：系统预先安排照料通知；关闭程序后的养育时间与现实时间同步，重新打开时同步离线成长。
- **增强模式（后台驻留）**：实时运行，可让部分安卓设备在小窗中持续运行，响应更迅速。自动降为普通模式后，回到前台恢复增强模式；手动选择普通模式则保持不变。
- **统一暂停**：普通和增强模式均暂停成长与提醒，重新打开仍保持暂停，恢复时不补算暂停时长。
- **三种外观**：真机蛋形外壳、极简大屏与小屏模式，共享同一份进度。小屏模式读取当前窗口尺寸与屏幕形状，支持双指捏合调整并保存画面大小。
- **游戏内相机修复**：相机动画正常播放，不再误触发蓝牙连接。
- **一键截屏**：在设置中开启“截图”，只保存游戏画面至 `Pictures/Open Meets` 独立相册，搭配无声的闪白动画。
- **删除当前存档**：在进度管理中二次确认后删除当前 ROM 的存档并重置，其他 ROM 的进度保留。
- **中文 / English 界面**：菜单、帮助和通知可切换语言；游戏文字由 ROM 决定。
- **手机与平板适配**：横竖屏、圆形 A/B/C 按键、多点触控 A+C。
- **WebMeets 收礼**：通过蓝牙从另一台设备上的 WebMeets 接收物品。
- **内置 Mixing Meets**：从游戏内 App 的“去玩 / Visit”或“接收礼物 / Present”进入内置客户端。

## 快速上手

**操作**：A 选择，B 确认，C 返回。支持长按和 A+C 同时按下；游戏屏幕休眠后按任意键唤醒。

**切换 ROM**：打开 **⋯ → 切换 ROM**，直接点选已导入的版本，也可继续导入 ROM 或 ZIP。只有当前版本继续养育，其他版本在重新打开时只同步时钟。

**保存与恢复**：在设置中导出 `.t18s` 备份；导入时使用与当前 ROM 版本匹配的存档。卸载应用会删除本地 ROM 和进度。

**养育模式**：设置中提供“是否开启后台驻留”开关。新用户默认开启，升级保留原设置；关闭即使用普通模式。保持 ROM 内的声音开启以检测呼叫，应用菜单静音仍保留安静通知。请允许通知和“闹钟与提醒”；未允许精确闹钟时通知可能延迟。系统设置中的“强行停止”会阻止通知，重新打开应用后恢复。长时间离线后可能需要等待成长同步完成。

## 小屏模式与截图

在 **设置 → 外观 → 小屏模式** 中开启。首次进入时双指捏合预览、调整大小并保存；之后切换模式会沿用已保存的大小。需要重新调整时，点小屏模式下方的 **调整大小**。

小屏操作：左侧为 A，中间为 B，右侧下方三分之二为 C。**长按右上方三分之一约一秒，返回极简模式**。支持 A+C 双指组合。

在设置中开启 **截图** 后：

- **极简模式**：点击游戏屏幕上方的相机快门。
- **真机模式**：点击外壳上的蝴蝶结。
- **小屏模式**：双击中间上方三分之一区域；B 键使用中间下方三分之二。

图片仅包含原始游戏画面，保存到 `Pictures/Open Meets` 独立相册。截图时画面从上到下闪白，不播放快门声。

## WebMeets 与 Mixing Meets

### WebMeets 蓝牙收礼

1. 在游戏内选择 **连接 → 下载 / ダウンロード / Download**。
2. 开启蓝牙，允许应用请求的“附近的设备”权限。
3. 在 **Mac 或另一台 Android 设备的 Chrome** 中打开 [WebMeets](https://tamagotchicenter.com/webmeets/items)。
4. 选择物品，连接蓝牙设备 **TMGC_meets**，完成发送。

接收设备需支持 BLE 外设广播。接收时蓝牙名称会临时改为 `TMGC_meets`，结束后恢复。成功后自动保存，取消或中断会恢复连接前的进度。

### 内置 Mixing Meets

从游戏内 **App → 去玩 / Visit** 或 **接收礼物 / Present** 进入。客户端已适配 ARM64，在线功能依赖 Mixing Meets 社区服务。可通过 [Mixing Meets 支持页面](https://mixing-meets.com/support)支持社区运营。

WebMeets 收礼和 Mixing Meets 往返已完成 Android 模拟器链路验证；实体设备的蓝牙与系统兼容性仍需进一步验证。当前不支持红外或与实体玩具直连，Mixing Meets 婚配尚未完成验证。

## 支持的 ROM

| 系列 | 版本 |
| --- | --- |
| Tamagotchi ON（英文） | Fairy、Magic、Wonder Garden |
| Tamagotchi MEETS（日文） | Fairy、Magical、Pastel、Sanrio、Sweets、Fantasy |

暂不支持 Tamagotchi SOME（韩文）。ROM 由用户自行提供。

## 版本显示

发行版本与 Android 应用信息均为 **0.3.0**，内部版本号为 **21**。可直接覆盖此前 build 20 的正式版。

## 反馈与致谢

遇到问题请[提交 Issue](https://github.com/kanatallow/Open-Meets/issues)，附上设备型号、Android 版本、版本和复现步骤。请勿附带 ROM、个人存档或账号凭据。

模拟器基于 [oreo-fox/tg18-emu](https://github.com/oreo-fox/tg18-emu)，感谢上游作者、WebMeets 和 Mixing Meets 社区。上游 MIT 许可及其他组件许可保留在应用中。

Open Meets 免费提供，仅供非商业使用，禁止倒卖、收费分发、付费激活、广告变现及商业捆绑。许可全文见应用内许可页面。本项目与 Bandai 无隶属或认可关系；Tamagotchi 为其相关权利人的商标。

<p align="center"><em>Designed by Kanata with Pride and Joy</em></p>

---

## English

**Open Meets** brings Tamagotchi Meets / On to Android phones and tablets. Import your own ROM, care for your pet, keep separate progress for each version, receive gifts through WebMeets, and use the built-in ARM64 Mixing Meets client.

**English UI is fully supported:** menus, settings, help and notifications are available in English. Select **English** on the welcome screen or under **Settings → Language**. Game text depends on your ROM; English ON ROMs are supported.

This repository hosts downloads, release notes and user documentation. Application source code is not published here. No ROMs or sample saves are included.

### Download

**Android 8.0 or later · ARM64 · Stable release 0.3.0**

**[Download Open-Meets-0.3.0-arm64.apk — 86.6 MiB](https://github.com/kanatallow/Open-Meets/releases/download/v0.3.0/Open-Meets-0.3.0-arm64.apk)**

Includes the emulator, background care, notifications, save management, WebMeets BLE reception and the embedded ARM64 Mixing Meets client.

Install the APK, open **Open Meets**, and import your own ROM or an unencrypted ZIP. Choose **English** on the welcome screen or under **⋯ → 语言 / Language**.

**Back up your save and update over the existing installation. Do not uninstall first.** The app keeps the existing app identity and signing certificate to preserve local ROMs and progress.

### Everyday use

- **Controls:** A selects, B confirms, C goes back. Hold A+C together when needed; press any button to wake the display.
- **Appearance:** choose Device, Minimal or Small screen in Settings without changing your progress. Small screen uses the current window size and screen shape, with a saved pinch-to-resize adjustment.
- **In-game camera:** the photo animation now plays normally without triggering an unrelated Bluetooth connection.
- **Screenshots:** enable Screenshots in Settings to save just the game image to the dedicated `Pictures/Open Meets` album, with a silent white sweep animation.
- **Delete current save:** confirm the red option in save management to remove the current ROM’s save and reset it. Other ROMs keep their progress.
- **ROM library:** import individual ROMs or ZIPs, then switch from the saved ROMs list. Each version keeps separate progress; only the selected version continues care.
- **Saves:** autosave runs every 30 seconds. Export a `.t18s` backup or import one matching the current ROM version from Settings.
- **Normal mode:** turn off background residence to schedule care reminders and keep raising time synchronized after the app closes. Offline growth is synchronized when you return.
- **Enhanced mode (background residence):** supports continuous small-window operation and faster responses on some Android devices. Detected interruptions fall back to normal mode; returning to the foreground restores enhanced mode. Manually selected normal mode stays selected.
- **Pause:** stops growth and reminders in both modes, remains paused after reopening, and excludes paused time when resumed.
- **Preferences:** the residence switch appears in Settings. New users default to on; upgrades preserve their choice.
- **Reminders:** allow notifications and Alarms & reminders. Keep sound enabled inside the game for call detection; app-level mute still allows silent notifications. Without exact-alarm permission, alerts may be delayed. Android Force stop blocks notifications until the app is reopened. Long absences may require time to synchronize growth.

**Huawei HarmonyOS users are strongly advised to use normal mode so raising time remains synchronized with real time and pets continue growing after the app closes.**

### Small screen and screenshots

Select **Settings → Appearance → Small screen**. On first use, pinch the preview to adjust the game size and save it. Later mode changes keep your saved size. Use **Resize** below Small screen to adjust it again.

Tap the left third for A, the middle for B, and the lower two thirds of the right side for C. **Hold the upper-right third for about one second to return to Minimal.** A+C supports two-finger input.

Enable **Screenshots** in Settings, then:

- **Minimal:** tap the camera shutter above the game screen.
- **Device:** tap the bow on the shell.
- **Small screen:** double-tap the upper third of the middle column. B uses the lower two thirds of that column.

Only the original game image is saved, in the dedicated `Pictures/Open Meets` album. A silent white sweep runs from top to bottom when capturing.

### Connections

For **WebMeets**, choose **Connection → Download** in the game, enable Bluetooth and allow Nearby devices. Open [WebMeets](https://tamagotchicenter.com/webmeets/items) in Chrome on a Mac or another Android device, select an item and connect to **TMGC_meets**. The receiving device must support BLE peripheral advertising. Its Bluetooth name changes temporarily during reception and is restored afterward.

**App → Visit** and **App → Present** open the embedded Mixing Meets client. Online features depend on the Mixing Meets community service; [support the community here](https://mixing-meets.com/support).

WebMeets gift reception and Mixing Meets visit/return have been checked through Android emulator integration tests. Physical-device Bluetooth and compatibility need further testing. Infrared and direct links to physical toys are unsupported; Mixing Meets marriage has not yet been validated.

Supported ROMs: **ON** Fairy, Magic and Wonder Garden (English); **MEETS** Fairy, Magical, Pastel, Sanrio, Sweets and Fantasy (Japanese). Korean **SOME** ROMs are not supported.

### Version shown by Android

The release and Android app version are both **0.3.0**, with internal version code **21**. Install directly over the previous build 20 release.

### Feedback and credits

[Report an issue](https://github.com/kanatallow/Open-Meets/issues) with your device, Android version, edition and reproduction steps. Do not attach ROMs, personal saves or account credentials.

Based on [tg18-emu by oreo-fox](https://github.com/oreo-fox/tg18-emu), with thanks to the WebMeets and Mixing Meets communities. Upstream and third-party license notices are included in the app.

Free for noncommercial use. No resale, paid distribution, activation fees, advertising monetization or commercial bundling. See the in-app license page for the terms. This project is not affiliated with or endorsed by Bandai.
