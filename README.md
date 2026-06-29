# Voice of the Heart Pro Max

> 基于开源项目 Mineradio 二次开发的沉浸式音乐播放器发布页。

**Voice of the Heart Pro Max** 把搜索、播放、歌词、封面、粒子、照片轮播和移动端横屏舞台整合成一个可以“看见音乐”的私人现场。

这不是源码仓库，这里只放公开说明、截图、安装包下载和版本更新信息。

当前版本：`v1.1.2`

平台覆盖：`Windows` / `macOS` / `iOS` / `iPadOS` / `Android`

iOS / iPadOS 最低系统：`iOS 15.0`

## 预览

![Voice of the Heart 首页](./docs/assets/readme/voice-home.png)

![Voice of the Heart 搜索结果](./docs/assets/readme/voice-search.png)

![Voice of the Heart 播放器控制台](./docs/assets/readme/voice-player-panel.png)

## 核心特色

- **沉浸式音乐视觉**：歌词、封面色彩、粒子运动和视觉预设共同驱动 Now Playing 舞台。
- **全平台安装包**：Windows、macOS、iOS/iPadOS、Android 都有对应安装包。
- **iPhone + iPad 同步适配**：iOS / iPadOS 版本最低支持 iOS 15。
- **Android 横屏视觉**：支持单指拖动、双指滑动、双指捏合缩放和横屏 Now Playing。
- **桌面端完整能力**：Windows/macOS 保留桌面歌词、窗口控制、全局快捷键和自动更新等桌面体验。
- **暗色高级质感**：玻璃、微光、暗场和粒子视觉，适合长期听歌和录屏展示。

## 下载 v1.1.2

请到 GitHub Release 下载对应系统的安装包：

[下载 Voice of the Heart v1.1.2](https://github.com/futuredo/voice-of-the-heart/releases/tag/v1.1.2)

| 平台 | 文件 | 说明 |
| --- | --- | --- |
| Windows | `VoiceOfTheHeart-1.1.2-Setup.exe` | 推荐给普通 Windows 用户 |
| Windows 便携版 | `VoiceOfTheHeart-1.1.2-win-x64-portable.zip` | 解压后运行 `VoiceOfTheHeart.exe` |
| macOS Apple Silicon | `VoiceOfTheHeart-1.1.2-arm64.dmg` | M1/M2/M3/M4/M5 等 Apple Silicon Mac |
| macOS Intel | `VoiceOfTheHeart-1.1.2-x64.dmg` | Intel 处理器 Mac |
| iOS / iPadOS | `VoiceOfTheHeart-iOS-1.1.2-TrollStore.ipa` | iPhone / iPad，最低 iOS 15，需要 TrollStore 或其他侧载方式 |
| Android | `VoiceOfTheHeart-Android-1.1.2.apk` | 安卓手机侧载测试，需要允许未知来源安装 |

不要把 GitHub 自动生成的 `Source code` 当成安装包；安装包请下载上表对应文件。

## 平台能力对比

| 功能 | Windows | macOS | iOS / iPadOS | Android |
| --- | --- | --- | --- | --- |
| 基础播放 | 支持 | 支持 | 支持 | 支持 |
| 搜索和队列 | 支持 | 支持 | 支持 | 支持 |
| 歌词显示 | 支持 | 支持 | 支持 | 支持 |
| 粒子视觉 | 支持 | 支持 | 支持 | 支持 |
| 视觉预设 27-30 | 支持 | 支持 | 支持 | 支持 |
| 视觉控制台 | 支持 | 支持 | 部分支持 | 支持 |
| 触控视觉操作 | 鼠标 | 鼠标 | 支持 | 支持 |
| 双指视觉操作 | 不适用 | 不适用 | 支持 | 支持 |
| 横屏 Now Playing | 窗口化 | 窗口化 | 支持 | 支持 |
| iPad 适配 | 不适用 | 不适用 | 支持 | 不适用 |
| 最低 iOS 15 | 不适用 | 不适用 | 支持 | 不适用 |
| 桌面歌词 | 支持 | 支持 | 不支持 | 不支持 |
| 系统托盘 / 窗口控制 | 支持 | 支持 | 不支持 | 不支持 |
| 全局快捷键 | 支持 | 支持 | 不支持 | 不支持 |
| 自动更新 | 支持 | 支持 | 不支持 | 不支持 |

更完整的说明：

- [v1.1.2 全平台更新说明](./docs/RELEASE_NOTES_v1.1.2.md)
- [v1.1.2 平台功能对比与特色功能](./docs/PLATFORM_FEATURES_v1.1.2.md)

## v1.1.2 重点变化

- Android 从早期 WebView 壳层补齐到可用版本：搜索框、设置入口、横屏视觉、双指触控、头像显示、启动页和性能档位都已处理。
- macOS 安装包已重新打包，和当前视觉效果同步，包含新增视觉预设 `27 / 28 / 29 / 30`。
- iOS / iPadOS 同步适配 iPhone 和 iPad，最低系统 iOS 15。
- 全平台分享包已补齐 Android APK、全平台更新说明、平台功能对比和 SHA256 校验。

## 安装提示

### macOS

当前 DMG 未做 Apple 公证。首次打开如果提示“无法验证开发者”，可以右键 App，选择“打开”，再确认打开。

### iOS / iPadOS

IPA 面向 TrollStore / 自签名等侧载环境，不是 App Store 包。支持 iPhone 和 iPad，最低 iOS 15。

### Android

APK 是 release 构建、debug keystore 签名的侧载测试包。部分国产安卓系统会弹出“未知来源”“高风险”“USB 安装权限”等提示，需要手动允许。

## 项目来源和边界

Voice of the Heart Pro Max 是基于开源项目 Mineradio 的二次开发版本，保留并扩展了沉浸式音乐播放器、粒子视觉和桌面播放体验。

Voice of the Heart 不是网易云音乐、QQ 音乐、酷狗音乐或 Apple Music 的官方客户端，也不隶属于任何音乐平台。第三方平台接入仅用于个人学习、本地客户端体验和用户自有账号的播放辅助。请遵守对应平台的用户协议、版权规则和会员权益规则。
