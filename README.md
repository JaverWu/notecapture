# NoteCapture / 涂画录屏

一款面向 苹果芯片 Mac 的免费录屏软件，强调轻量录制、实时标注和清晰的操作演示。
多种录制模式并且可以在录屏期间进行文字标注、涂鸦等等
<img width="960" height="638" alt="image" src="https://github.com/user-attachments/assets/fc731141-2b1c-4cbb-91e4-b5dd99750e8f" />
期待您的捐款赞助，助力开发更多软件！😭
<img width="1304" height="1776" alt="IMG_20260919_190940" src="https://github.com/user-attachments/assets/d4ac5b0d-23e6-40c9-ad77-b0a420037e12" />


## 下载

请前往 [Releases](https://github.com/JaverWu/notecapture/releases/latest) 下载最新版：

- `NoteCapture-<版本>-Apple-Silicon.dmg`
- `NoteCapture-<版本>-Apple-Silicon.sha256`

目前仅支持 Apple Silicon（M1、M2、M3、M4 及后续芯片）和 macOS 14.0 或更高版本。

## 项目亮点

- **多种录制来源**：支持整个屏幕、自定义区域、单个窗口、单个应用和系统音频录制。
- **双屏与多屏区域录制**：所有可录制显示器会同时出现透明框选层；在哪块屏幕开始拖拽，就自动录制对应屏幕。
- **可调整的区域录制**：录制过程中可以拖动录制框；四角手柄支持等比例缩放，画面同步放大或缩小。
- **鼠标居中模式**：录制框平滑跟随鼠标，支持 10–100 平滑度调节；按 Esc 可暂时释放或恢复跟踪，超出屏幕部分自动补黑。
- **实时激光笔**：白色中心搭配红、蓝、绿描边，轨迹可在 0.1–2 秒内自动淡出，并同步写入录制视频。
- **文字标注**：定位文字时自动暂停录制；支持字号、颜色、描边和粗细调整，文字可拖动，双击即可删除。
- **直线与箭头**：录制时可绘制任意角度直线和箭头，并同步写入最终视频；按 Esc 可快速退出工具。
- **按键与点击展示**：显示 `L-click`、`R-click`、键盘按键、长按状态及组合键，适合教程与演示录制。
- **悬浮录屏工具栏**：采用紧凑布局，集中提供开始、暂停、停止、鼠标、激光笔、文字、直线和箭头等操作。
- **录制状态提示**：区域框选顶部显示倒计时和录制时间，并自动适配深色与浅色背景。
- **本地隐私优先**：不需要账号，不含广告与遥测；录制和标注处理均在本机完成。
- **紧凑玻璃质感界面**：使用 SwiftUI、AppKit、ScreenCaptureKit 与 AVFoundation 构建，压缩无效留白并保留清晰层级。

## 安装与首次打开

1. 下载并双击 DMG。
2. 将 `NoteCapture.app` 拖入 `Applications` 文件夹。
3. 尝试打开 NoteCapture。
4. 因当前版本未使用付费 Apple Developer ID 和 Apple 公证，请前往“系统设置 → 隐私与安全性”，点击“仍要打开”。
5. 在“屏幕与系统音频录制”中允许“涂画录屏”。
6. 如需展示鼠标和键盘按键，还需在“输入监控”中允许“涂画录屏”。
7. 修改权限后，请完全退出并重新打开应用。

请勿关闭 Gatekeeper 或 SIP。仅从本仓库的 Releases 页面下载安装包，并核对 SHA-256。

## 校验下载文件

在 DMG 所在目录运行：

```bash
shasum -a 256 -c NoteCapture-<版本>-Apple-Silicon.sha256
```

出现 `OK` 表示文件与发布者提供的校验值一致。

## 隐私

NoteCapture 不要求注册账号，不上传录像、按键记录或使用数据。屏幕、麦克风和输入监控权限只用于用户主动启用的录制功能。详情请阅读 [PRIVACY.md](PRIVACY.md)。

## 安全提示

当前安装包使用不包含姓名、邮箱或 Apple Team ID 的固定本地签名，以帮助 macOS 在应用更新后保持录屏权限。该签名不是 Apple Developer ID，因此首次打开仍需用户手动确认。

发现安全问题时，请阅读 [SECURITY.md](SECURITY.md)。

## 许可

本仓库不提供源代码许可。二进制软件的使用和分发条件见 [LICENSE.txt](LICENSE.txt)。

## 致谢

产品设计与部分交互思路参考了 [QuickRecorder](https://github.com/lihaoyun6/QuickRecorder)。NoteCapture 为独立实现，未在本仓库分发 QuickRecorder 源码或品牌资源。
