功能介绍

· 将你的所有配置（分类、磁贴、搜索引擎、背景设置）备份到指定的 GitHub 仓库中，实现多设备同步。
· 支持手动上传/下载，也可开启自动同步：每次数据变动（增删改磁贴、分类、搜索引擎、背景）后，自动将最新配置上传至 GitHub（防抖 2 秒）。

配置步骤

1. 点击任何弹窗底部的 GitHub同步 按钮。
2. 填写以下信息：
   · 仓库：格式 用户名/仓库名，例如 yourname/startpage-backup。
   · 文件路径：保存的文件名，如 homepage-data.json。
   · Token：GitHub 个人访问令牌，需要 repo 权限。可在 GitHub Settings → Developer settings → Personal access tokens → Tokens (classic) 生成。
3. 可选：勾选“自动同步”，之后每次数据变化都会自动上传。
4. 点击测试验证连接是否成功。
5. 点击上传手动备份当前配置；点击下载从仓库拉取配置并覆盖本地数据（下载后会提示确认覆盖）。

安全提示

· Token 保存在浏览器的 localStorage 中，仅用于与 GitHub API 通信。请勿将 Token 泄露给他人。
· 建议使用具有最小权限的 Token（仅 repo 权限）。

🛠️ 技术栈

· 纯 HTML/CSS/JavaScript，无任何后端依赖。
· 图标：Iconify（通过 <iconify-icon> 组件）
· 拖拽排序：SortableJS
· 文件保存：FileSaver.js
· 数据持久化：localStorage

📁 文件结构

· index.html – 单页面应用，包含所有样式和脚本。
· 无需额外资源文件，所有功能集成在一个 HTML 中。

🌐 浏览器兼容性

· 现代浏览器（Chrome、Firefox、Edge、Safari）均支持。
· 移动端触摸优化，支持长按、滑动等手势。

📄 许可证

本项目未明确指定许可证，仅供参考学习使用。

---

Enjoy your personalized start page!
如果有任何问题或建议，欢迎提交 Issue 或 Pull Request。