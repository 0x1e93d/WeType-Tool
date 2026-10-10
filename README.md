# WeType Tool

WeType Tool 是面向微信输入法的功能扩展模块。本仓库用于发布正式版安装包。

## 下载

当前正式版：[v2.0.2](https://github.com/0x1e93d/WeType-Tool/releases/tag/v2.0.2)。

- `WeType-Tool-v2.0.2.apk`：用于 LSPosed 的模块安装包。
- `WeType-4.0.0-Patched-v1.2.apk`：已内置模块的微信输入法安装包，无需额外安装模块。
- `SHA256SUMS.txt`：两个 APK 的 SHA-256 校验值。

内置版使用[微信输入法官方安装包](https://z.weixin.qq.com/android/download?channel=latest)和 [JingMatrix LSPatch v1.2](https://github.com/JingMatrix/LSPatch/releases/tag/v1.2)构建。两个 APK 的具体版本、构建信息及更新内容见对应 Release。

## 安装

使用 LSPosed 时安装模块 APK，并在模块管理器中启用微信输入法作用域；使用内置版时安装已打包的微信输入法 APK。两种方式只需选择一种。

内置版签名与微信输入法官方包不同，无法直接覆盖安装；请先备份输入法数据，再卸载官方包并安装内置版。

## 问题反馈

请在本仓库的 [Issues](https://github.com/0x1e93d/WeType-Tool/issues) 中提供安装包文件名、设备与 Android 版本、复现步骤及已脱敏的诊断日志。
