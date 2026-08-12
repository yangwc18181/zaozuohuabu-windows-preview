# 造作画布（ZZHB AI Canvas）

造作画布是一款面向 AI 图片、视频和音频工作流的 Windows 本地可视化画布。

**[直接下载造作画布 v0.2.3](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/download/v0.2.3/ZZHB-0.2.3-win-x64.zip)** · [画布使用手册](https://acaiy.cn/article/canvas-guide/) · [查看 v0.2.3 发布说明](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/tag/v0.2.3) · [全部历史版本](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases)

你可以在同一个项目里整理参考图、提示词、音频、视频、模型结果和设计说明，再把它们连接成可持续修改的工作流程。本仓库只用于发布 Windows 成品和公开使用说明，不提供商业产品源码。

<img width="1709" height="799" alt="造作画布项目界面" src="https://github.com/user-attachments/assets/f179aed0-7a0c-44c8-81fb-35bda2fe947b" />

<img width="1718" height="815" alt="造作画布节点与模型配置" src="https://github.com/user-attachments/assets/c7eeac40-cc13-4b90-9e60-c885bb0792de" />

<img width="1718" height="815" alt="造作画布工作流界面" src="https://github.com/user-attachments/assets/07815762-94f0-46b3-b6cc-fc62d322f36e" />

## 下载与安装

1. 下载 [`ZZHB-0.2.3-win-x64.zip`](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/download/v0.2.3/ZZHB-0.2.3-win-x64.zip)。
2. 将 ZIP **完整解压**到普通文件夹，不要直接在压缩包内运行。
3. 双击 `ZZHB\ZZHB.exe`，等待本地服务启动并自动打开 Windows 默认浏览器。
4. 使用期间保持程序运行；关闭程序会同时停止本地服务。

当前程序尚未代码签名，Windows 可能提示“未知发布者”。请确认文件来自本仓库，并使用下方 SHA-256 核对下载内容。

## 第一次使用

- 打开“模型与供应商”，自行添加官方或第三方模型服务提供商的连接和 API Key；也可以连接自己的 ComfyUI。
- 模型调用可能产生费用，网络、价格、额度、隐私政策和模型可用性由所选服务决定，请先从少量测试开始。
- 不要公开分享 API Key，也不要在 Issue 中粘贴 Key、客户资料、私人项目、未脱敏截图或完整日志。
- ComfyUI 工作流需要你自行安装并启动对应的本机或云端 ComfyUI 服务，再填写可访问的 Base URL。

## v0.2.3 主要更新

- **H3 兼容修复**：供应商显示名称变化不再导致已配置的 MiniMax 官方或第三方模型服务提供商 H3 被误判为身份不匹配。
- **H3 结果找回**：修复第三方 H3 已完成任务的结果地址解析；找回入口更醒目，并明确只查询原任务、不重新提交生成。
- **模型能力一致性**：设置、首页、正式节点、底部生成器和模板统一读取 Connection 已保存的模型能力，避免预设更新悄悄改变已有配置的运行选项。
- **发布保护**：候选构建会与上一版本的稳定模型能力基线比较，并排除构建电脑上的个人连接。

## 下载校验

| 项目 | 内容 |
| --- | --- |
| 文件名 | `ZZHB-0.2.3-win-x64.zip` |
| 文件大小 | 74,483,131 bytes |
| SHA-256 | `5ab1df7d9745763b87adc7355417f60b5138190338c2e642d68a3d15f8ba2b4c` |

## 已知边界

旧 H3 任务能否找回取决于原服务是否仍允许查询该任务；部分付费 H3 路径和具体自定义 ComfyUI 节点的兼容性取决于用户选择的服务、网络条件和节点定义。大项目性能仍在持续优化。本说明不表示所有真实付费渠道或所有自定义节点组合都已经完成验证。

## 使用范围

允许个人学习、研究、试用和课程内容制作。未经授权，不允许转售、改名分发、重新打包，或将本程序作为 SaaS、托管服务或付费产品再次发布。

本版本不授予源代码、品牌资产或再次分发权利。完整条款以软件包内 `TERMS.txt` 为准。

## 反馈

欢迎通过 [GitHub Issues](https://github.com/yangwc18181/zaozuohuabu-windows-preview/issues) 反馈启动失败、模型配置、生成失败、画布交互或功能建议。请尽量提供 Windows 版本、软件版本、操作步骤和脱敏后的错误信息。
