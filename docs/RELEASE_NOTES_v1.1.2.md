# Voice of the Heart v1.1.2 全平台更新说明

Voice of the Heart Pro Max 是基于开源项目 Mineradio 二次开发的跨平台沉浸式音乐播放器。本次 v1.1.2 重点是把桌面端的视觉和播放体验扩展到移动端，并补齐 Windows、macOS、iOS/iPadOS、Android 四个平台的安装包。

## 版本定位

v1.1.2 是一次“全平台可分享版”：

- 桌面端继续作为功能最完整的主力版本。
- iOS / iPadOS 作为移动端 demo 重点适配，支持 iPhone 和 iPad，最低 iOS 15。
- Android 从早期壳层补齐到接近 iOS demo 的可用版本。
- 分享包包含安装说明、功能对比和 SHA256 校验。

## 新增和强化

### 全平台安装包

- Windows 安装版：`VoiceOfTheHeart-1.1.2-Setup.exe`
- Windows 便携版：`VoiceOfTheHeart-1.1.2-win-x64-portable.zip`
- macOS Apple Silicon：`VoiceOfTheHeart-1.1.2-arm64.dmg`
- macOS Intel：`VoiceOfTheHeart-1.1.2-x64.dmg`
- iOS / iPadOS：`VoiceOfTheHeart-iOS-1.1.2-TrollStore.ipa`
- Android：`VoiceOfTheHeart-Android-1.1.2.apk`

### 移动端适配

- iOS / iPadOS 同步适配 iPhone 和 iPad。
- iOS / iPadOS 最低系统版本为 iOS 15。
- Android 增加首页、歌单、视觉三段式移动导航。
- Android 增加右上角控制中枢，提供设置、视觉控制台和横屏视觉入口。
- Android 增加“视觉页横屏播放”设置项。

### 沉浸式视觉系统

- 保留粒子、歌词、封面色彩和专辑图驱动的视觉舞台。
- macOS 重新打包并同步新增视觉预设 `27 / 28 / 29 / 30`。
- Android 支持单指拖动画布。
- Android 支持双指滑动和双指捏合缩放。
- Android 横屏后隐藏冗余 UI，更接近手机横屏 Now Playing。

### Android 重点修复

- 修复搜索框位置偏下。
- 修复搜索框不能自动隐藏。
- 修复没有设置入口。
- 修复设置按钮与账号头像重叠。
- 修复账号头像空白或破图。
- 修复视觉页不能触控。
- 修复双指滑动/缩放无效。
- 修复横屏后无法回到竖屏。
- 优化启动加载界面。
- 增加视觉画质档位和 Android 渲染限流。

### macOS 重新打包

- 重新生成 arm64 / x64 两个 DMG。
- 新包已同步当前视觉效果。
- 新包包含最新视觉排序和新增预设。

## 已知边界

- iOS / iPadOS IPA 面向 TrollStore / 自签名等侧载环境，不是 App Store 包。
- Android APK 是 release 构建、debug keystore 签名的侧载测试包，不是应用商店上架签名。
- macOS DMG 当前未公证，首次打开可能需要右键打开。
- 桌面端音源和系统能力最完整；移动端音源能力仍会受平台原生桥、登录方式、版权和系统策略影响。
