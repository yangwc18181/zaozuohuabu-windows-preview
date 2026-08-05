# 造作画布（ZZHB AI Canvas）

造作画布是一款面向室内设计师与视觉创作者的 Windows 本地 AI 无限画布，支持多模型调用、ComfyUI 工作流与自定义 API。

**[下载最新版](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/latest)** · [查看图文教程](https://acaiy.cn/infinite-canvas)

你可以在同一个项目里整理参考图、提示词、模型结果、对话记录和设计说明，再把它们连接成可持续修改的工作流程。本仓库只用于发布 Windows 可执行版本和公开使用说明，不提供商业产品源码。

<img width="1709" height="799" alt="造作画布项目界面" src="https://github.com/user-attachments/assets/f179aed0-7a0c-44c8-81fb-35bda2fe947b" />

<img width="1718" height="815" alt="造作画布节点与模型配置" src="https://github.com/user-attachments/assets/c7eeac40-cc13-4b90-9e60-c885bb0792de" />

<img width="1718" height="815" alt="造作画布工作流界面" src="https://github.com/user-attachments/assets/07815762-94f0-46b3-b6cc-fc62d322f36e" />

## 当前版本：v0.1.4

v0.1.4 重点完成 Midjourney 工作台、参考图与连续变化闭环，并补充 MiniMax H3 视频能力和画布可靠性收口：

- 新增画布旁 Midjourney 工作台，支持当前版本的普通参考、风格参考、角色参考、深度参考、细微 / 强烈连续变化、来源图定位和上游任务结果找回。
- MiniMax H3 接入现有视频节点，支持纯提示词、首帧 / 尾帧和图片 / 视频 / 音频全能参考模式。
- 修复视频上传、项目模板导入 / 导出、画布保存和跨项目任务隔离等问题。
- 修复 Windows 便携包静态资源 MIME 映射；`ZZHB.exe` 继续使用 Windows 默认浏览器，Edge 等浏览器可以正常加载界面。
- 模型配置页增加 API Key 显示 / 隐藏图标和渠道选择提示。

## 发布包内容

- 34 条模型连接模板，所有 Key 均为空。
- 大语言模型提示词预设为 0，不随包提供用户提示词。
- ComfyUI runtime 与 Base URL 均为空，不携带本机运行配置。
- 仅包含 `krea2-turbo` 与 `z-image-turbo` 两条 ComfyUI 工作流。

使用模型或工作流前，请在应用中填写你自己的 API Key、Base URL 或本机 ComfyUI 地址。不要提交或分享 Key、客户资料、私人项目、未脱敏截图或完整日志。

## 下载与启动

1. 打开 [最新版 Release](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/latest)，下载 Windows x64 ZIP。
2. 完整解压 ZIP，不要直接在压缩包内运行。
3. 双击 `ZZHB\ZZHB.exe`，等待本地服务启动并自动打开 Windows 默认浏览器。
4. 使用期间保持程序运行；关闭程序会同时停止本地服务。

当前程序尚未代码签名，Windows 可能提示“未知发布者”。请确认文件来自本仓库，并使用 Release 中的 SHA-256 文件核对下载内容。

## 第一次使用

打开“模型与供应商”，在准备使用的供应商连接中填写自己的 Key。模型调用可能产生费用；使用官方或第三方供应商前，请先确认价格、额度、隐私政策和服务条款，并从少量测试开始。

ComfyUI 工作流需要你自行安装并启动对应的本机或云端 ComfyUI 服务，再填写可访问的 Base URL。

## 历史版本

- v0.1.3：新增视频节点第一批能力、Seedance / Kling 可选预设、应用配色、项目级画布底纹、4× 缩放和拼接图像的 ComfyUI 输入支持。
- v0.1.2：新增对话、图像拼接与裁剪、便签、模板、提示词预设、ComfyUI 工作流和图像对比等能力。
- v0.1.1：优化对话选区、便签滚动、主要操作图标与节点交互。

## 使用范围

允许个人学习、研究、试用和课程内容制作。未经授权，不允许转售、改名分发、重新打包，或将本程序作为 SaaS、托管服务或付费产品再次发布。

本版本不授予源代码、品牌资产或再次分发权利。完整条款以软件包内 `TERMS.txt` 为准。

## 反馈

欢迎通过 [GitHub Issues](https://github.com/yangwc18181/zaozuohuabu-windows-preview/issues) 反馈启动失败、模型配置、生成失败、画布交互或功能建议。请尽量提供 Windows 版本、软件版本、操作步骤和脱敏后的错误信息。
