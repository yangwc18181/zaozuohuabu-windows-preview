# 造作画布（ZZHB AI Canvas）

造作画布是一款面向 AI 图片、视频和音频工作流的 Windows 本地可视化画布。

**[直接下载造作画布 v0.2.7](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/download/v0.2.7/ZZHB-0.2.7-win-x64.zip)** · [画布使用手册](https://acaiy.cn/article/canvas-guide/) · [查看 v0.2.7 发布说明](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/tag/v0.2.7) · [全部历史版本](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases)

你可以在同一个项目里整理参考图、提示词、音频、视频、模型结果和设计说明，再把它们连接成可持续修改的工作流程。本仓库只用于发布 Windows 成品和公开使用说明，不提供商业产品源码。

<img width="1709" height="799" alt="造作画布项目界面" src="https://github.com/user-attachments/assets/f179aed0-7a0c-44c8-81fb-35bda2fe947b" />

<img width="1718" height="815" alt="造作画布节点与模型配置" src="https://github.com/user-attachments/assets/c7eeac40-cc13-4b90-9e60-c885bb0792de" />

<img width="1718" height="815" alt="造作画布工作流界面" src="https://github.com/user-attachments/assets/07815762-94f0-46b3-b6cc-fc62d322f36e" />

欢迎加入 画布交流群！反馈问题、交流使用体验或提出新功能建议。

<img width="500" height="500" alt="PixPin_2026-08-14_14-30-48" src="https://github.com/user-attachments/assets/b7170e0f-5a45-42c2-958b-fbadb501e3cd" />



## 下载与安装

1. 下载 [`ZZHB-0.2.7-win-x64.zip`](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/download/v0.2.7/ZZHB-0.2.7-win-x64.zip)。
2. 将 ZIP **完整解压**到普通文件夹，不要直接在压缩包内运行。
3. 双击 `ZZHB\ZZHB.exe`，等待本地服务启动并自动打开 Windows 默认浏览器。
4. 使用期间保持程序运行；关闭程序会同时停止本地服务。

当前程序尚未代码签名，Windows 可能提示“未知发布者”。请确认文件来自本仓库，并使用下方 SHA-256 核对下载内容。

## 第一次使用

- 打开“模型与供应商”，自行添加官方或第三方模型服务提供商的连接和 API Key；也可以连接自己的 ComfyUI。
- 模型调用可能产生费用，网络、价格、额度、隐私政策和模型可用性由所选服务决定，请先从少量测试开始。
- 不要公开分享 API Key，也不要在 Issue 中粘贴 Key、客户资料、私人项目、未脱敏截图或完整日志。
- ComfyUI 工作流需要你自行安装并启动对应的本机或云端 ComfyUI 服务，再填写可访问的 Base URL。

## v0.2.7 主要更新

这一版重点补强了长任务恢复、生成过程追溯和项目整理：

- **ComfyUI 长任务更可靠**：支持预览、刷新或本地服务重启后找回原任务、安全取消，并可把已有结果接回画布。
- **生成历史可追溯、可复用**：图片、视频和 ComfyUI 历史可以查看当次实际输入，并在确认后精确复用当时的提示词、素材、角色与顺序。
- **MiniMax H3 2K 路径补全**：增加视频规格预检、中断恢复、旧任务找回和真实媒体时长读取。
- **首页项目管理增强**：支持项目封面、单层文件夹、单个或批量移动、批量移入垃圾箱，以及批量导出画布模板和项目备份。
- **大图体验改善**：画布采用分级预览，单张图片上传上限提高到 200MB，并支持按需查看原图。
- **视频与对话修复**：改进视频真实时长、视频对比播放和相关恢复状态；文字附件可在设定的记忆轮数内参与后续对话。

## 下载校验

| 项目 | 内容 |
| --- | --- |
| 文件名 | `ZZHB-0.2.7-win-x64.zip` |
| 文件大小 | 75,725,673 bytes |
| SHA-256 | `c00c0c20ab9af3f2be6c2e99af77049735edf08d74d02311c6780a6755f3dd6b` |

## 已知边界

文件夹嵌套、排序、搜索、标签和文件夹整体导入 / 导出尚未提供。旧 H3 或 ComfyUI 任务能否找回取决于原服务是否仍允许查询该任务；部分付费路径和具体自定义 ComfyUI 节点的兼容性取决于用户选择的服务、网络条件和节点定义。大项目性能仍在持续优化。本说明不表示所有真实付费渠道、所有公网素材服务或所有自定义节点组合都已经完成验证。

## 使用范围

允许个人学习、研究、试用和课程内容制作。未经授权，不允许转售、改名分发、重新打包，或将本程序作为 SaaS、托管服务或付费产品再次发布。


## 反馈

欢迎通过 [GitHub Issues](https://github.com/yangwc18181/zaozuohuabu-windows-preview/issues) 反馈启动失败、模型配置、生成失败、画布交互或功能建议。请尽量提供 Windows 版本、软件版本、操作步骤和脱敏后的错误信息。
