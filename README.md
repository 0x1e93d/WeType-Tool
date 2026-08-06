# WeType Tool

WeType Tool 是面向微信输入法的功能扩展模块。

本仓库用于发布 WeType Tool 的正式版安装包。

## 下载

请前往 [Releases](https://github.com/0x1e93d/WeType-Tool-Releases/releases) 下载最新版本。

每个正式版本包含两个 APK：

```text
WeType-Tool-v<版本>-api102.apk
WeType-Tool-v<版本>-legacy.apk
```

例如：

```text
WeType-Tool-v1.2.8-api102.apk
WeType-Tool-v1.2.8-legacy.apk
```

## 版本区别

### API 102

适用于 API 102 环境的设备和运行方式。

### Legacy

适用于兼容模式或较旧环境。

Legacy 版本也用于 WeType Tool 的免 Root 内置组合包。

如果不确定应该选择哪个版本，建议先使用 Legacy 版本。

## 安装方式

请根据你使用的环境选择对应 APK，并按照模块管理器的提示完成安装。

安装前建议：

- 确认微信输入法版本与模块适配。
- 卸载或停用同类功能模块，避免功能冲突。
- 安装后重新启动微信输入法或相关应用。

## 文件校验

Release 中的 `SHA256SUMS.txt` 提供 APK 校验值。

Linux、macOS 或 Git Bash 中可以使用：

```bash
sha256sum -c SHA256SUMS.txt
```

Windows PowerShell 可以使用：

```powershell
Get-FileHash .\WeType-Tool-v1.2.8-legacy.apk -Algorithm SHA256
```

请将输出结果与 Release 中的校验值进行比较。

## Bug 反馈

遇到问题时，请前往 [Issues](https://github.com/0x1e93d/WeType-Tool-Releases/issues) 提交反馈。

反馈时请尽量提供：

- Tool 版本
- 微信输入法版本和 versionCode
- 手机型号与 Android 版本
- 使用的是 API 102 还是 Legacy
- 是否安装了其他可能影响输入法的模块
- 问题复现步骤
- 日志或截图

请在上传日志和截图前删除账号、设备标识、Token 及其他隐私信息。

## 相关项目

- [WeType Monet](https://github.com/0x1e93d/WeType_Monet)：微信输入法 Monet 风格适配
- [WeType-Tool-Patch](https://github.com/0x1e93d/WeType-Tool-Patch)：WeType Tool 免 Root 内置组合包

## 免责声明

本项目为第三方功能扩展项目。

微信输入法及相关品牌、软件和资源的权利归其各自权利人所有。
