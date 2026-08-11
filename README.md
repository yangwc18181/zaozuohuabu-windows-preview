# 造作画布（ZZHB AI Canvas）

造作画布是一款面向 AI 图片、视频和音频工作流的 Windows 本地可视化画布。

**[直接下载造作画布 v0.2.1](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/download/v0.2.1/ZZHB-0.2.1-win-x64.zip)** · [画布使用手册](https://acaiy.cn/article/canvas-guide/) · [查看 v0.2.1 发布说明](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/tag/v0.2.1) · [全部历史版本](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases)

你可以在同一个项目里整理参考图、提示词、音频、视频、模型结果和设计说明，再把它们连接成可持续修改的工作流程。本仓库只用于发布 Windows 成品和公开使用说明，不提供商业产品源码。

<img width="1709" height="799" alt="造作画布项目界面" src="https://github.com/user-attachments/assets/f179aed0-7a0c-44c8-81fb-35bda2fe947b" />

<img width="1718" height="815" alt="造作画布节点与模型配置" src="https://github.com/user-attachments/assets/c7eeac40-cc13-4b90-9e60-c885bb0792de" />

<img width="1718" height="815" alt="造作画布工作流界面" src="https://github.com/user-attachments/assets/07815762-94f0-46b3-b6cc-fc62d322f36e" />

## 下载与安装

1. 下载 [`ZZHB-0.2.1-win-x64.zip`](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/download/v0.2.1/ZZHB-0.2.1-win-x64.zip)。
2. 将 ZIP **完整解压**到普通文件夹，不要直接在压缩包内运行。
3. 双击 `ZZHB\ZZHB.exe`，等待本地服务启动并自动打开 Windows 默认浏览器。
4. 使用期间保持程序运行；关闭程序会同时停止本地服务。

当前程序尚未代码签名，Windows 可能提示“未知发布者”。请确认文件来自本仓库，并使用下方 SHA-256 核对下载内容。

## 第一次使用

- 打开“模型与供应商”，自行添加官方或第三方模型服务提供商的连接和 API Key；也可以连接自己的 ComfyUI。
- 模型调用可能产生费用，网络、价格、额度、隐私政策和模型可用性由所选服务决定，请先从少量测试开始。
- 不要公开分享 API Key，也不要在 Issue 中粘贴 Key、客户资料、私人项目、未脱敏截图或完整日志。
- ComfyUI 工作流需要你自行安装并启动对应的本机或云端 ComfyUI 服务，再填写可访问的 Base URL。

## v0.2.1 主要更新

- **音频工作台**：支持常见音频格式的上传、播放 / 暂停、进度、音量、倍速、波形和非破坏裁剪。
- **图片处理**：新增图片缩放和裁剪，处理结果继续作为受管资产在画布中连线。
- **分辨率选择器**：支持常见或自定义比例、百万像素、指定宽高和整除设置，分别输出宽度与高度。
- **ComfyUI 接线**：完善动态输入、固定 / 可选输入、音频输入输出以及枚举 / 下拉参数还原。导入动态接口时需要连接到包含权威节点定义的正确 ComfyUI 实例。
- **画布效率**：增加流程复制、上游选择和同类型线束中转；提示词输入可自适应增高，屏幕外重媒体不再全部提前运行。
- **H3 流程**：增加 MiniMax 官方与第三方模型服务提供商的 H3 入口、提示词优化、768P 到 2K 流程和任务找回能力。

## 下载校验

| 项目 | 内容 |
| --- | --- |
| 文件名 | `ZZHB-0.2.1-win-x64.zip` |
| 文件大小 | 75,736,686 bytes |
| SHA-256 | `80ee7019af6005ec00ac0fd87f73de1de8c7c84c428429690d99faea0ad12ca6` |

## 已知边界

部分付费 H3 路径和具体自定义 ComfyUI 节点的兼容性取决于用户选择的服务、网络条件和节点定义；大项目性能仍在持续优化。本说明不表示所有真实付费渠道或所有自定义节点组合都已经完成验证。

## 使用范围

允许个人学习、研究、试用和课程内容制作。未经授权，不允许转售、改名分发、重新打包，或将本程序作为 SaaS、托管服务或付费产品再次发布。

本版本不授予源代码、品牌资产或再次分发权利。完整条款以软件包内 `TERMS.txt` 为准。

## 反馈

欢迎通过 [GitHub Issues](https://github.com/yangwc18181/zaozuohuabu-windows-preview/issues) 反馈启动失败、模型配置、生成失败、画布交互或功能建议。请尽量提供 Windows 版本、软件版本、操作步骤和脱敏后的错误信息。
