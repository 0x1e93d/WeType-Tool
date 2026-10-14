# WeType Tool

[![最新正式版](https://img.shields.io/github/v/release/0x1e93d/WeType-Tool?style=flat-square&label=release)](https://github.com/0x1e93d/WeType-Tool/releases/latest)
![Android 9+](https://img.shields.io/badge/Android-9%2B-3DDC84?style=flat-square&logo=android&logoColor=white)
![arm64-v8a](https://img.shields.io/badge/ABI-arm64--v8a-3478C0?style=flat-square)
[![累计下载](https://img.shields.io/github/downloads/0x1e93d/WeType-Tool/total?style=flat-square&label=downloads)](https://github.com/0x1e93d/WeType-Tool/releases)

WeType Tool 是面向[微信输入法](https://z.weixin.qq.com/)的功能扩展模块，提供手势、文本编辑、词库管理、输入法底栏与主题美化。本仓库用于发布正式版安装包和收集问题反馈。

[下载最新正式版](https://github.com/0x1e93d/WeType-Tool/releases/latest) · [查看更新记录](https://github.com/0x1e93d/WeType-Tool/releases) · [反馈问题](https://github.com/0x1e93d/WeType-Tool/issues)

## 功能概览

| 板块 | 主要功能 |
| --- | --- |
| 输入操作 | 26 键、九键与空格键手势，自定义按键标签；文字编辑面板支持光标移动、选区、撤销重做和剪贴板操作。 |
| 剪切板与数据 | 剪切板增强、常用语管理、用户词库查看与导入导出，以及通过微信输入法原生接口进行全量备份和恢复。 |
| 触感与音效 | 分别设置按下、抬起的触感反馈；切换官方、麻将或自定义按键音效。 |
| 输入法底栏 | 自定义底栏按钮、顺序和外观；按需启用 MIUI、OPPO 底栏适配。设备专属选项取决于系统支持情况。 |
| 快捷主题 | 主题色、候选栏、按键及按压色、工具栏与图标的浅色和深色精调。 |
| 自定义主题 | 覆盖 Color、Drawable 与原版布局文件；支持 XML、SVG、GIF 资源和 `.wett` 主题导入导出。 |
| 通用美化 | 玻璃与自定义背景、字体、26 键和九键字符偏移；受支持设备可使用 HyperOS4 高级材质。 |
| 设置与诊断 | 界面外观、日志等级和诊断包导出。 |

具体选项及版本变更以对应 [Release 说明](https://github.com/0x1e93d/WeType-Tool/releases)为准。

## 下载与文件

当前正式版：[v2.0.6](https://github.com/0x1e93d/WeType-Tool/releases/tag/v2.0.6)。请从同一版本的 Release 下载所需文件。

| 文件 | 用途 |
| --- | --- |
| [WeType-Tool-v2.0.6.apk](https://github.com/0x1e93d/WeType-Tool/releases/download/v2.0.6/WeType-Tool-v2.0.6.apk) | **LSPosed 模块版**。已安装微信输入法和 LSPosed 的用户选择此包。 |
| [WeType-4.0.0-Patched-v1.2.apk](https://github.com/0x1e93d/WeType-Tool/releases/download/v2.0.6/WeType-4.0.0-Patched-v1.2.apk) | **内置版微信输入法**。已将模块嵌入微信输入法，无需另装模块或 LSPosed。 |
| [SHA256SUMS.txt](https://github.com/0x1e93d/WeType-Tool/releases/download/v2.0.6/SHA256SUMS.txt) | 上述两个 APK 的 SHA-256 校验值，用于核对下载文件。 |

文件名中的 `2.0.6` 是 WeType Tool 版本，`4.0.0` 是内置版使用的微信输入法版本，`1.2` 是打包所用的 LSPatch 版本。内置版基于 [WeType_Monet Releases](https://github.com/0x1e93d/WeType_Monet/releases) 提供的微信输入法原始 APK 和 [JingMatrix LSPatch v1.2](https://github.com/JingMatrix/LSPatch/releases/tag/v1.2)构建。

## 安装方式

1. **LSPosed 模块版**：安装 `WeType-Tool-v2.0.6.apk`，在 LSPosed 中启用模块并勾选微信输入法作用域，然后完整重启微信输入法。
2. **内置版**：先备份微信输入法数据，再卸载官方微信输入法并安装 `WeType-4.0.0-Patched-v1.2.apk`。内置版签名与官方包不同，不能直接覆盖安装；也无需再安装模块 APK。

两种方式选择其一。启用后可从微信输入法设置界面的模块入口打开 WeType Tool。当前 APK 要求 Android 9 及以上、arm64-v8a 设备；部分系统相关功能仅在相应机型上提供。

## 校验与反馈

下载两个 APK 和 `SHA256SUMS.txt` 后，可在文件所在目录运行 `sha256sum -c SHA256SUMS.txt` 校验。Windows 用户可用 `Get-FileHash .\WeType-Tool-v2.0.6.apk -Algorithm SHA256`，将结果与校验文件比较。

遇到问题时，请在 [Issues](https://github.com/0x1e93d/WeType-Tool/issues) 中说明安装包文件名、设备与 Android 版本、复现步骤；也可以在模块“设置 → 导出诊断包”中复现后导出日志，检查并脱敏后再附上。
