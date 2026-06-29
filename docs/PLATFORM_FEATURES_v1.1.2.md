# Voice of the Heart v1.1.2 平台功能对比与特色功能

Voice of the Heart 的核心不是“再做一个播放器”，而是把播放、歌词、封面、粒子和移动端舞台融合起来，让音乐有可看的现场感。

## 不同平台怎么选

| 平台 | 推荐安装包 | 推荐用途 |
| --- | --- | --- |
| Windows | `VoiceOfTheHeart-1.1.2-Setup.exe` | 功能完整的主力桌面播放器 |
| Windows 便携 | `VoiceOfTheHeart-1.1.2-win-x64-portable.zip` | 不想安装，解压即用 |
| macOS Apple Silicon | `VoiceOfTheHeart-1.1.2-arm64.dmg` | M 系列芯片 Mac |
| macOS Intel | `VoiceOfTheHeart-1.1.2-x64.dmg` | Intel Mac |
| iOS / iPadOS | `VoiceOfTheHeart-iOS-1.1.2-TrollStore.ipa` | iPhone / iPad 移动端 demo，最低 iOS 15 |
| Android | `VoiceOfTheHeart-Android-1.1.2.apk` | 安卓手机侧载测试，横屏视觉体验 |

## 核心功能对比

| 功能 | Windows | macOS | iOS / iPadOS | Android |
| --- | --- | --- | --- | --- |
| 基础播放 | 支持 | 支持 | 支持 | 支持 |
| 搜索和队列 | 支持 | 支持 | 支持 | 支持 |
| 歌词显示 | 支持 | 支持 | 支持 | 支持 |
| 粒子视觉 | 支持 | 支持 | 支持 | 支持 |
| 视觉控制台 | 支持 | 支持 | 部分支持 | 支持 |
| 视觉预设 27-30 | 支持 | 支持 | 支持 | 支持 |
| 触控视觉操作 | 鼠标 | 鼠标 | 支持 | 支持 |
| 双指视觉操作 | 不适用 | 不适用 | 支持 | 支持 |
| 横屏 Now Playing | 窗口化 | 窗口化 | 支持 | 支持 |
| iPad 适配 | 不适用 | 不适用 | 支持 | 不适用 |
| 最低 iOS 15 | 不适用 | 不适用 | 支持 | 不适用 |
| 桌面歌词 | 支持 | 支持 | 不支持 | 不支持 |
| 系统托盘 / 窗口控制 | 支持 | 支持 | 不支持 | 不支持 |
| 全局快捷键 | 支持 | 支持 | 不支持 | 不支持 |
| 自动更新 | 支持 | 支持 | 不支持 | 不支持 |
| 侧载安装 | 不适用 | 不适用 | IPA | APK |

## 音源能力对比

| 音源 / 能力 | Windows | macOS | iOS / iPadOS | Android |
| --- | --- | --- | --- | --- |
| 网易云 | 支持 | 支持 | 支持 | 支持 |
| QQ 音乐 | 支持 | 支持 | 暂未完整支持 | 部分支持 |
| 酷狗 | 支持 | 支持 | 支持 | 支持 |
| Apple Music 30s 试听 | 支持 | 支持 | 支持 | 支持 |
| 本地 / 桌面增强音源 | 支持 | 支持 | 不支持 | 不支持 |
| LX 自定义音源 | 支持 | 支持 | 不支持 | 暂未完整支持 |

## 主要特色

### 1. 音乐可视化不是背景，是主舞台

Voice of the Heart 会把歌词、封面色彩、粒子运动和视觉预设一起推到前台。它更像一个私人音乐现场，而不是普通播放列表。

### 2. 移动端 Now Playing 舞台

iPhone、iPad 和 Android 都围绕移动端重新适配。Android 支持横屏视觉播放；iOS / iPadOS 最低 iOS 15，并同步适配 iPad。

### 3. 桌面端能力完整

Windows/macOS 继续保留桌面播放器应该有的窗口、托盘、桌面歌词、全局快捷键和自动更新能力，适合长期使用。

### 4. 多平台分享友好

全平台安装包按目录拆好，配套下载说明、更新说明、功能对比和 SHA256 校验，适合直接发给测试用户或粉丝。

### 5. 暗色高级视觉

整体 UI 使用暗色、玻璃、微光和粒子语言，避免普通播放器的廉价按钮堆叠感。

## 后续方向

- 为 Android 准备正式 release keystore。
- 继续补齐 iOS / Android 的 QQ、LX、自定义音源能力。
- 做更多 Android 机型兼容性测试。
- 若要上架商店，补齐隐私合规、正式签名、截图、审核材料和权限说明。
