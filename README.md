# Claude 数据导出查看器 (Claude Export Viewer)

一个**单文件、纯浏览器、零后端**的工具，用来本地查看和检索你从 Claude 导出的对话数据。

直接用浏览器打开 `claude-export-viewer.html` 即可使用，无需安装、无需联网上传你的数据。你的导出文件全程只在本地浏览器内解析，**不会上传到任何服务器**。

## ✨ 功能特性

- 📂 **拖拽即用**：支持导入 Claude 官方导出的 `.zip` 压缩包或 `conversations.json` 文件，拖进页面或点击选择均可
- 💬 **对话浏览**：按项目（Projects）和对话（Conversations）分类查看，列表支持按最近更新、创建时间、消息数排序
- 🔍 **全文搜索**：跨所有对话快速检索关键词
- 🧠 **思考过程**：可展开查看 Claude 的 thinking / reasoning 推理内容
- 🛠️ **工具调用**：渲染 tool_use 工具调用与 artifact 产物
- 📊 **数据统计**：一览导出数据的整体概况
- 🌿 **分支与时间线**：可视化对话的分支结构
- 🖼️ **图片查看**：内置图片浏览，支持上传本地图片对照查看
- 📐 **Mermaid 图表**：自动渲染对话中的 Mermaid 图表
- 📤 **导出**：单条对话可导出为 Markdown，或通过打印另存为 PDF

## 🚀 使用方法

1. 下载本仓库的 `claude-export-viewer.html`（或点击右上角 **Code → Download ZIP**）
2. 用浏览器（Chrome / Edge / Firefox / Safari 均可）双击打开该 HTML 文件
3. 将你的 Claude 导出文件（`.zip` 或 `conversations.json`）拖入页面，或点击选择文件
4. 开始浏览、搜索、导出

### 如何获取 Claude 导出数据

在 Claude 网页端进入 **Settings（设置）→ Privacy（隐私）→ Export data（导出数据）**，按提示发起导出，稍后会收到包含数据的下载链接。

## 🔒 隐私说明

本工具是**纯前端**实现，所有解析均在你的浏览器本地完成，数据不经过任何服务器。可以完全离线使用。

## 📦 依赖

页面通过 CDN 加载两个第三方库：

- [Mermaid](https://mermaid.js.org/) — 用于渲染图表
- [JSZip](https://stuk.github.io/jszip/) — 用于解析 `.zip` 导出包

> ⚠️ 因为依赖通过 CDN 引入，**首次使用建议保持联网**以加载这两个库。若需完全离线运行，可自行将这两个库下载到本地并修改 HTML 中的 `<script>` 引用路径。

## 🌐 浏览器兼容性

支持现代浏览器（Chrome、Edge、Firefox、Safari 等）。建议使用最新版本以获得最佳体验。

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📄 许可证

本项目基于 [MIT License](LICENSE) 开源。
