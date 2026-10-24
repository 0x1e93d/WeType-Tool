<div align="center">

<p><img src="docs/images/wetype-tool-logo.svg" width="104" height="104" alt="WeType Tool Logo"></p>

<h1>WeType Tool</h1>

<p>微信输入法 · 功能增强与主题美化</p>
<p>手势、剪切板、布局与底栏，按自己的习惯设置。</p>

<p>
  <a href="https://github.com/0x1e93d/WeType-Tool/releases/latest"><img src="https://img.shields.io/github/v/release/0x1e93d/WeType-Tool?style=flat-square&amp;label=Release" alt="最新正式版"></a>
  <a href="https://github.com/0x1e93d/WeType-Tool/releases"><img src="https://img.shields.io/github/downloads/0x1e93d/WeType-Tool/total?style=flat-square&amp;label=Downloads" alt="累计下载量"></a>
  <img src="https://img.shields.io/badge/Android-9%2B-3DDC84?style=flat-square&amp;logo=android&amp;logoColor=white" alt="Android 9 及以上">
  <img src="https://img.shields.io/badge/ABI-arm64--v8a-3478C0?style=flat-square" alt="arm64-v8a">
  <img src="https://img.shields.io/badge/Xposed-API%20102-4F639D?style=flat-square" alt="模块版需要 libxposed API 102">
</p>

<p>
  <a href="https://github.com/0x1e93d/WeType-Tool/releases/latest">下载</a> ·
  <a href="#功能特性">功能特性</a> ·
  <a href="#安装使用">安装使用</a> ·
  <a href="#常见问题">常见问题</a> ·
  <a href="#问题反馈">问题反馈</a>
</p>

</div>

WeType Tool 为[微信输入法](https://z.weixin.qq.com/)提供输入操作与外观扩展，支持 **LSPosed 模块版**和**免 Root 内置版**。本仓库用于发布正式版安装包和收集问题反馈。

## 功能特性

### 输入与编辑

| 功能 | 可以做什么 |
| :--- | :--- |
| 按键手势 | 分别设置 26 键、九键的下滑动作，支持空格上滑／下滑与回车上滑；可绑定复制、粘贴、语言切换、表情面板、滑移和滑选等动作，自定义键盘上的动作标签。 |
| 剪切板增强 | 显示跨设备内容，解除文本字数与存留时间限制；支持图片记录和原生预览，按分钟设置图片保留时间或设为无限制，调整图片行高、位置与边距。 |
| 剪切板分类 | 按正则自定义分类，提供文本、图片筛选和常用语入口，设置浅色／深色气泡背景。 |
| 文字编辑面板 | 从工具栏或手势打开，提供四向光标移动、选择、段首／段尾、全选、撤销重做与剪贴板操作，支持普通和悬浮键盘。 |
| 内嵌自动填充 | 在工具栏中显示 Bitwarden 等密码管理器提供的系统填充建议，保留认证与填充流程；可调整显示内容、气泡宽度、间距与字号。 |
| 触感与音效 | 分别设置按下与抬起反馈，支持时长、强度、系统反馈及自定义波形；按键音可使用官方、内置麻将或自定义音效。 |

### 数据与底栏

| 功能 | 可以做什么 |
| :--- | :--- |
| 常用语管理 | 添加、编辑、删除和排序常用语，支持导入与导出。 |
| 用户词库 | 查看、搜索学习词条，支持词库导入与 TXT 导出。 |
| 全量备份 | 通过微信输入法原生接口备份、恢复词库、常用语和词频等数据，导出为 `.backup` 文件。 |
| 自定义底栏 | 实时预览底栏，添加预设或自定义按钮；设置单击／长按动作、名称、图标、颜色与尺寸，长按拖动排序、拖出删除，支持批量导入图标。 |
| 系统底栏适配 | 提供 MIUI 与 OPPO 底栏设置；符合条件的设备可从自定义底栏打开 MIUI 剪切板与常用语、输入法切换。自定义底栏在悬浮键盘中自动隐藏。 |
| 其他设置 | 禁用热更新、禁用官方升级，以及通过部分资源签名校验。 |

### 主题与布局

主题支持**快捷**与**自定义**两种独立模式，切换时保留各自配置。主题选择与管理、当前主题内容编辑使用独立入口。

| 功能 | 可以做什么 |
| :--- | :--- |
| 主题管理 | 新建、复制、编辑主题信息，选择当前主题，通过 `.wett` 文件导入与分享主题。 |
| 快捷配色 | 设置主题色，分别精调浅色／深色的候选、普通键、功能键、Action 键及普通键按压色；精调优先于主题色。 |
| 按键与候选 | 调整圆角、阴影、边框、首字颜色与背景、左右边距；为按键、首字背景和工具栏项目添加高光。 |
| 背景材质 | 默认、自定义与玻璃背景；分别配置浅色／深色遮罩、模糊和高光。支持的设备可使用 HyperOS4 清透磨砂、柔光玻璃或 ColorOS 高级材质，并适配悬浮键盘。 |
| 字体与字符偏移 | 默认、内置苹方、系统或导入字体；26 键与九键独立设置字符的百分比偏移，覆盖键面及气泡等显示位置。 |
| Color 与 Drawable | 预览默认资源，搜索字段并替换颜色或图像；支持系统动态颜色引用、夜间覆盖、XML／SVG 参数编辑与 GIF 动画。 |
| 工具栏与图标 | 编辑、替换或隐藏 Logo，调整项目背景与高光；提供空格 Logo、表情 Logo 的内置样式与自定义资源。 |
| 剪切板与常用语样式 | 共用项目背景圆角及浅色／深色背景颜色，覆盖剪切板堆叠卡片；受支持设备可启用 HyperOS4 剪切板透明。 |
| 可视化布局编辑 | 使用微信输入法的渲染链路预览布局，缩放、移动并点选按键，编辑文字、尺寸、功能码和定位关系，增删行与按键、调整顺序，支持夜间布局编辑。 |
| 布局文件与精简 | 导入原名 JSON 或 ZIP 布局包，导出单个布局文件；可隐藏常用语提示。 |

模块设置还提供跟随系统／浅色／深色外观、日志等级和诊断包导出。功能是否可用取决于安装版本、微信输入法版本与设备系统，具体以对应 [Release 说明](https://github.com/0x1e93d/WeType-Tool/releases)为准。

## 下载文件

当前正式版：[v2.1.5](https://github.com/0x1e93d/WeType-Tool/releases/tag/v2.1.5)。请从同一版本的 Release 下载所需文件。

| 文件 | 内容与用途 |
| :--- | :--- |
| [WeType-Tool-v2.1.5.apk](https://github.com/0x1e93d/WeType-Tool/releases/download/v2.1.5/WeType-Tool-v2.1.5.apk) | **LSPosed 模块**。需要已安装微信输入法和支持 libxposed API 102 的 LSPosed 或兼容框架。 |
| [WeType-4.0.1-Patched-v1.2.apk](https://github.com/0x1e93d/WeType-Tool/releases/download/v2.1.5/WeType-4.0.1-Patched-v1.2.apk) | **免 Root 普通内置版**。基于原版输入法直接嵌入模块，未额外启用键盘内自动填充，无需另装模块或 LSPosed。 |
| [WeType-4.0.1-Patched-v1.2-inline-autofill.apk](https://github.com/0x1e93d/WeType-Tool/releases/download/v2.1.5/WeType-4.0.1-Patched-v1.2-inline-autofill.apk) | **免 Root 自动填充内置版**。文件名带 `-inline-autofill`，额外启用键盘内自动填充支持，可在工具栏显示 Bitwarden 等密码管理器的填充建议。 |
| [SHA256SUMS.txt](https://github.com/0x1e93d/WeType-Tool/releases/download/v2.1.5/SHA256SUMS.txt) | 本次发布 APK 的 SHA-256 校验值，用于核对文件是否完整。 |

文件名中的标识分别代表：

- `2.1.5`：WeType Tool 版本。
- `4.0.1`：内置版使用的微信输入法版本。
- `1.2`：打包使用的 LSPatch 版本。
- `-inline-autofill`：已为免 Root 内置版补齐内嵌自动填充支持，可在工具栏显示 Bitwarden 等密码管理器的填充建议，无需系统框架作用域。

内置版基于 [WeType_Monet Releases](https://github.com/0x1e93d/WeType_Monet/releases) 中的微信输入法原始 APK，使用 [JingMatrix LSPatch](https://github.com/JingMatrix/LSPatch/releases/tag/v1.2)嵌入本模块。

无需键盘内密码建议时选择**普通内置版**；需要此功能时选择 **`-inline-autofill` 版**。两者使用相同包名、发布签名和模块，选择一个安装即可。

## 安装使用

两种安装方式选择其一。当前安装包适用于 **Android 9 及以上、arm64-v8a** 设备。

### LSPosed 模块版

1. 安装微信输入法，并准备支持 **libxposed API 102** 的 LSPosed 或兼容框架。
2. 安装 `WeType-Tool-v2.1.5.apk`。
3. 在框架中启用模块，勾选**微信输入法**作用域。
4. 完整重启微信输入法，再进入其设置页面。

使用内嵌自动填充时，还需勾选**系统框架**作用域并重启设备，详见下方使用说明。

### 免 Root 内置版

内置版保留官方包名 `com.tencent.wetype`，签名与官方 APK 不同，不能直接覆盖官方版安装。

1. 备份需要保留的输入法数据。
2. 卸载官方微信输入法或签名不同的修改版。
3. 安装同一 Release 中的普通内置版 `WeType-4.0.1-Patched-v1.2.apk`，或按需选择带 `-inline-autofill` 后缀的自动填充内置版。
4. 在系统中启用微信输入法，然后打开其设置页面。

无需再安装模块 APK。后续使用本项目相同签名的内置版覆盖更新。

### 打开模块设置

进入**微信输入法设置页面**，点击右下角的模块入口。模块没有独立的桌面图标，功能和主题都在此入口中配置。

### 内嵌自动填充

此功能需要 Android 11 及以上，以及支持内嵌建议的密码管理器。

1. 在微信输入法工具栏中添加**收起键盘**按钮。
2. 模块版在框架中勾选**系统框架**作用域并重启设备；免 Root 用户使用带 **`-inline-autofill`** 后缀的内置包，无需勾选作用域或安装框架。
3. 在系统中选择密码管理器作为自动填充服务，并开启管理器中的**内嵌自动填充／键盘内建议**。
4. 开启模块中的**功能 → 输入操作 → 内嵌自动填充**，进入登录页的账号或密码输入框。

建议显示在工具栏中间，支持横向滚动，点击后由密码管理器完成认证和填充。免 Root 版始终保留建议文字，仍可调整图标与气泡外观。

## 常见问题

<details>
<summary>安装后找不到模块入口？</summary>

模块没有桌面图标，请从微信输入法设置页面进入。模块版还需确认框架支持 libxposed API 102、模块已启用且勾选微信输入法作用域，完成后完整重启微信输入法。

</details>

<details>
<summary>为什么没有 HyperOS4 或 ColorOS 材质选项？</summary>

设备专属选项会按机型与系统能力显示。HyperOS4 清透磨砂、柔光玻璃及剪切板透明面向符合条件的小米设备，ColorOS 高级材质面向符合条件的 OPPO／一加设备；其他设备可使用普通背景、美化与布局功能。

</details>

<details>
<summary>主题文件、布局文件和全量备份有什么区别？</summary>

- `.wett`：WeType Tool 主题，包含主题配置与所需资源。
- `.json`／`.zip`：键盘布局文件或布局包，供“美化 → 布局 → 键盘布局”导入。
- `.backup`：通过微信输入法原生接口导出的全量备份，在“功能 → 全量备份”中恢复。

更换内置版或卸载输入法前，请先导出需要保留的内容。

</details>

<details>
<summary>如何校验下载的 APK？</summary>

将本次发布的 APK 与 `SHA256SUMS.txt` 放在同一目录，可运行：

```shell
sha256sum -c SHA256SUMS.txt
```

Windows 也可计算单个文件的校验值，再与清单比较：

```powershell
Get-FileHash .\WeType-Tool-v2.1.5.apk -Algorithm SHA256
```

</details>

## 问题反馈

**未附诊断日志，或使用非原版微信输入法底包（如替换过官方布局、资源的第三方修改包）的 Issue，将直接关闭，不予排查。** 本项目发布的免 Root 内置版基于原版底包构建，可正常反馈。

请在 [Issues](https://github.com/0x1e93d/WeType-Tool/issues) 中附上**诊断包**，并提供安装包文件名、模块和微信输入法版本、设备型号、Android／系统版本、使用的框架，以及复现步骤。界面问题可另附截图或录屏，不能替代日志。

进入**设置 → 导出诊断包**，填写问题描述。诊断流程会临时提高日志等级并重启输入法；请在此状态下**复现问题后再保存**。诊断包包含设备、框架信息与日志，上传前请检查并脱敏。
