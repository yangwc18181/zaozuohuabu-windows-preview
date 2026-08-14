# 造作画布（ZZHB AI Canvas）

造作画布是一款面向 AI 图片、视频和音频工作流的 Windows 本地可视化画布。

**[直接下载造作画布 v0.2.5](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/download/v0.2.5/ZZHB-0.2.5-win-x64.zip)** · [画布使用手册](https://acaiy.cn/article/canvas-guide/) · [查看 v0.2.5 发布说明](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/tag/v0.2.5) · [全部历史版本](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases)

你可以在同一个项目里整理参考图、提示词、音频、视频、模型结果和设计说明，再把它们连接成可持续修改的工作流程。本仓库只用于发布 Windows 成品和公开使用说明，不提供商业产品源码。

<img width="1709" height="799" alt="造作画布项目界面" src="https://github.com/user-attachments/assets/f179aed0-7a0c-44c8-81fb-35bda2fe947b" />

<img width="1718" height="815" alt="造作画布节点与模型配置" src="https://github.com/user-attachments/assets/c7eeac40-cc13-4b90-9e60-c885bb0792de" />

<img width="1718" height="815" alt="造作画布工作流界面" src="https://github.com/user-attachments/assets/07815762-94f0-46b3-b6cc-fc62d322f36e" />

欢迎加入 画布交流群！反馈问题、交流使用体验或提出新功能建议。

<img width="500" height="500" alt="PixPin_2026-08-14_14-30-48" src="https://github.com/user-attachments/assets/b7170e0f-5a45-42c2-958b-fbadb501e3cd" />



## 下载与安装

1. 下载 [`ZZHB-0.2.5-win-x64.zip`](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/download/v0.2.5/ZZHB-0.2.5-win-x64.zip)。
2. 将 ZIP **完整解压**到普通文件夹，不要直接在压缩包内运行。
3. 双击 `ZZHB\ZZHB.exe`，等待本地服务启动并自动打开 Windows 默认浏览器。
4. 使用期间保持程序运行；关闭程序会同时停止本地服务。

当前程序尚未代码签名，Windows 可能提示“未知发布者”。请确认文件来自本仓库，并使用下方 SHA-256 核对下载内容。

## 第一次使用

- 打开“模型与供应商”，自行添加官方或第三方模型服务提供商的连接和 API Key；也可以连接自己的 ComfyUI。
- 模型调用可能产生费用，网络、价格、额度、隐私政策和模型可用性由所选服务决定，请先从少量测试开始。
- 不要公开分享 API Key，也不要在 Issue 中粘贴 Key、客户资料、私人项目、未脱敏截图或完整日志。
- ComfyUI 工作流需要你自行安装并启动对应的本机或云端 ComfyUI 服务，再填写可访问的 Base URL。

## v0.2.5 主要更新

建议所有用户升级到 v0.2.5。本版集中修复启动、模型配置读取和画布状态一致性问题：

- **启动与模型预设**：修复成品环境读取模型预设及模型交付合同的问题，避免启动后模型配置不可用。
- **MiniMax 官方 H3**：一个官方模型连接下清楚区分生成视频、优化提示词和升至 2K 三种用途。
- **视频参考条件提示**：支持视频参考的节点会明确提示当前渠道需要的 HTTPS 素材条件；条件不足时在提交前停止。
- **模型交付合同**：分开表达模型能力、渠道传输、产品接通、运行条件与验证证据，避免把“模型支持”误写成“本机直接可用”。
- **项目与界面一致性**：Midjourney 停靠面板按项目独立恢复，并收口主题可读性、节点动作、状态、保存与模板语义。

## 下载校验

| 项目 | 内容 |
| --- | --- |
| 文件名 | `ZZHB-0.2.5-win-x64.zip` |
| 文件大小 | 75,630,639 bytes |
| SHA-256 | `aeb187f4ec1309a838cc4805f928148968128a317771e86a32a8443d945d4e13` |

## 已知边界

旧 H3 任务能否找回取决于原服务是否仍允许查询该任务；MiniMax H3、Seedance 等模型使用本地视频参考时仍需要用户已有的安全 HTTPS 素材服务。部分付费路径和具体自定义 ComfyUI 节点的兼容性取决于用户选择的服务、网络条件和节点定义。大项目性能仍在持续优化。本说明不表示所有真实付费渠道、所有公网素材服务或所有自定义节点组合都已经完成验证。

## 使用范围

允许个人学习、研究、试用和课程内容制作。未经授权，不允许转售、改名分发、重新打包，或将本程序作为 SaaS、托管服务或付费产品再次发布。

本版本不授予源代码、品牌资产或再次分发权利。完整条款以软件包内 `TERMS.txt` 为准。

## 反馈

欢迎通过 [GitHub Issues](https://github.com/yangwc18181/zaozuohuabu-windows-preview/issues) 反馈启动失败、模型配置、生成失败、画布交互或功能建议。请尽量提供 Windows 版本、软件版本、操作步骤和脱敏后的错误信息。
