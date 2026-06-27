# Voice of the Heart

Voice of the Heart 是一个 macOS 沉浸式音乐可视化播放器。它把音乐播放、歌词舞台、封面视觉、照片轮播和拼豆效果组合成一个更偏艺术化的桌面播放器体验。

## 下载

当前版本：

```text
v0.0.1
```

macOS Apple Silicon 用户下载：

```text
Voice of the Heart-0.0.1-arm64.dmg
```

SHA256：

```text
1634aaca4e3be1f96a57dae8c6a554459f6568c515da9a937bce9984366e6cfb
```

## 系统要求

- macOS
- Apple Silicon Mac：M1 / M2 / M3 / M4
- 当前 DMG 是 `arm64` 架构，Intel Mac 暂不作为推荐安装目标

## 安装方式

1. 下载 `Voice of the Heart-0.0.1-arm64.dmg`。
2. 双击打开 DMG。
3. 将 `Voice of the Heart.app` 拖入 `Applications`。
4. 从 `Applications` 打开 `Voice of the Heart.app`。

当前版本未使用 Apple Developer ID 公证，所以首次打开时 macOS 可能提示“无法验证开发者”。如果你确认 DMG 来源可信，可以：

1. 在 `Applications` 中右键 `Voice of the Heart.app`。
2. 选择“打开”。
3. 在系统弹窗中再次确认打开。

如果仍然被系统阻止，可以进入：

```text
系统设置 > 隐私与安全性
```

在页面底部选择“仍要打开”。

## 权限说明

应用可能会请求麦克风权限。这个权限用于音频分析，让视觉效果可以随着音乐律动。

Voice of the Heart 不会把你的本地播放缓存、系统缓存或 Electron 运行缓存打包进 DMG。每个用户的运行数据只会保存在自己电脑的用户目录中，例如：

```text
~/Library/Application Support/Voice of the Heart/
```

## v0.0.1 内容

- 音乐播放与沉浸式歌词舞台
- 多种视觉预设
- 支持专辑封面和用户自定义图片
- 照片轮播视觉
- 拼豆视觉预设
- 支持随音乐律动的视觉动画
- macOS DMG 安装包

## 文件校验

下载后可以在终端中校验 DMG：

```sh
shasum -a 256 "Voice of the Heart-0.0.1-arm64.dmg"
```

输出应为：

```text
1634aaca4e3be1f96a57dae8c6a554459f6568c515da9a937bce9984366e6cfb  Voice of the Heart-0.0.1-arm64.dmg
```

## 发布状态

这是 `v0.0.1` 的 macOS Apple Silicon DMG 发布包。当前版本用于手动下载安装，不包含自动更新承诺。

