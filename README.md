# Voice of the Heart Pro Max - 基于 Mineradio 二次开发

Voice of the Heart Pro Max 是一款基于 Mineradio 二次开发的沉浸式音乐可视化播放器，把搜索、播放、歌单、歌词舞台、粒子视觉、封面视觉和桌面氛围整合到一个深色玻璃质感的音乐空间里。它从 Mineradio 的桌面体验演进而来，目标是让音乐不仅能被听见，也能被看见。

当前公开版本：`v1.1.1`，已覆盖 **macOS / Windows / iOS / Android** 四个平台，界面与交互一致。

## 预览

![Voice of the Heart 首页](./docs/assets/readme/voice-home.png)

![Voice of the Heart 搜索结果](./docs/assets/readme/voice-search.png)

![Voice of the Heart 播放器控制台](./docs/assets/readme/voice-player-panel.png)

## 特色功能

- 沉浸式首页：星河背景、玻璃卡片、最近播放、歌单与推荐入口。
- 多平台搜索：支持网易云、Apple Music 试听、本地与播客等入口组合。
- 播放器控制台：播放/暂停、上下首、喜欢、收藏、队列、歌词、音量和沉浸模式。
- 歌词与视觉舞台：歌词层、粒子、封面、照片轮播和音乐律动视觉。
- 歌单与队列：支持当前队列、我的歌单、播客和推荐内容浏览。
- 真实频谱接入：macOS 可配合 BlackHole 等虚拟声卡，让视觉跟随系统音频律动。
- 深色高级质感：以玻璃、暗场、粒子和专辑封面为核心视觉语言。
- 全平台一致：桌面（Mac/Windows）功能最全；iOS 网易云为原生实现；Android 同源 WebView 外壳。

## 下载

请到 [v1.1.1 Release](https://github.com/futuredo/voice-of-the-heart/releases/tag/v1.1.1) 下载对应系统的安装包。

| 设备 / 系统 | 应下载的文件 | 说明 |
| --- | --- | --- |
| Apple 芯片 Mac | `VoiceOfTheHeart-1.1.1-arm64.dmg` | 适用于 M1 / M2 / M3 / M4 等 Apple Silicon |
| Intel 芯片 Mac | `VoiceOfTheHeart-1.1.1-x64.dmg` | 适用于 Intel 处理器 Mac |
| Windows 电脑 | `VoiceOfTheHeart-1.1.1-win-x64-portable.zip` | 便携版，解压后运行 `VoiceOfTheHeart.exe`（本版暂无安装器 .exe） |
| Android 手机 | `VoiceOfTheHeart-Android-1.1.1.apk` | 允许「未知来源」后安装；debug 签名，自用 |
| iPhone | `VoiceOfTheHeart-iOS-1.1.1-TrollStore.ipa` | 需用 TrollStore 安装（未签名，非 App Store） |

不要下载 `Source code`、`.blockmap` 或 `latest*.yml` 作为安装包；这些文件主要用于发布和更新校验。

## 安装说明

### macOS

1. 下载对应架构的 `.dmg` 文件。
2. 双击打开 DMG。
3. 将 `Voice of the Heart.app` 拖入 `Applications`。
4. 从 `Applications` 打开应用。

当前版本未使用 Apple Developer ID 公证。首次打开如果提示“无法验证开发者”，可以右键应用选择“打开”，或进入：

```text
系统设置 > 隐私与安全性
```

在页面底部选择“仍要打开”。

### Windows

1. 下载 `VoiceOfTheHeart-1.1.1-win-x64-portable.zip`。
2. 解压到任意文件夹。
3. 双击文件夹内的 `VoiceOfTheHeart.exe` 运行（首次运行无需安装）。

小众 Electron 应用可能触发浏览器、Windows Defender 或 SmartScreen 提醒。请先确认文件来自本仓库 Release；如 SmartScreen 拦截，可点击“更多信息”后选择“仍要运行”。

### Android

1. 下载 `VoiceOfTheHeart-Android-1.1.1.apk`。
2. 在系统设置中允许浏览器或文件管理器「安装未知来源应用」。
3. 点击 APK 完成安装（debug 签名，适合自用 / 内测）。

### iPhone（iOS）

本应用未上架 App Store，需要通过 **TrollStore** 安装：

1. 下载 `VoiceOfTheHeart-1.1.1-TrollStore.ipa`。
2. 在已安装 TrollStore 的 iPhone 上用 TrollStore 打开该 IPA。
3. 点击 Install 完成安装（TrollStore 安装永久有效，不受免费证书 7 天限制）。

## 文件校验

下载后可以用下面的 SHA256 校验文件完整性：

```text
VoiceOfTheHeart-1.1.1-arm64.dmg
b34d1929b4d0144740a021d97dcfce6f9e627c56ccc010c75b0f7b1e2b95c37d

VoiceOfTheHeart-1.1.1-x64.dmg
8f5247ad4d97a88bfabff5f5b5a98490d4cb44fac240dd292d613afd86d2339d

VoiceOfTheHeart-1.1.1-win-x64-portable.zip
90b68f27164ca8a1ee939562f20004932d3b6ecdf306520738298f3be64a89f9

VoiceOfTheHeart-Android-1.1.1.apk
347f01be749125028055f5aa41e10e32bcec524821f219e9ace9eb6198da3edf

VoiceOfTheHeart-iOS-1.1.1-TrollStore.ipa
cb08e0e0048732c8e68daed6f4a38777445b0c9e5db672dd6edb3cc86cf9a9cf
```

macOS / Linux：

```sh
shasum -a 256 "VoiceOfTheHeart-1.1.1-arm64.dmg"
```

Windows PowerShell：

```powershell
Get-FileHash .\VoiceOfTheHeart-1.1.1-win-x64-portable.zip -Algorithm SHA256
```

## 权限与数据

应用可能会请求麦克风权限，用于音频分析和频谱视觉。用户登录态、播放缓存、搜索历史、封面缓存和运行数据保存在本机用户目录中，不会被打包进安装包。

常见数据目录：

```text
~/Library/Application Support/Voice of the Heart/
```

## 项目说明

Voice of the Heart 不是网易云音乐、QQ 音乐、Apple Music 或任何第三方音乐平台的官方客户端。相关平台接入仅用于个人学习、本地客户端体验和用户自有账号的播放辅助。请遵守对应平台的用户协议、版权规则和会员权益规则。

## 授权

本项目基于 GPL-3.0 授权。界面视觉、Voice of the Heart 名称、图标和原创视觉表达归作者所有；第三方依赖和第三方服务分别遵循其各自授权与服务条款。
