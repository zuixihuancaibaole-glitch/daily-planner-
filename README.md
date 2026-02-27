# 🗒 Daily Planner · 日计划

<div align="center">

A beautiful, fully offline daily planner — no server, no login, no dependencies.  
一款精美的全离线日计划应用，无需服务器、无需登录、无需依赖。

![HTML](https://img.shields.io/badge/HTML-Single%20File-orange?style=flat-square&logo=html5)
![CSS](https://img.shields.io/badge/CSS-Vanilla-blue?style=flat-square&logo=css3)
![JS](https://img.shields.io/badge/JavaScript-Vanilla-yellow?style=flat-square&logo=javascript)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

[English](#english) · [中文](#中文)

</div>

---

## English

### Overview

Daily Planner is a single-file (`daily-planner.html`) productivity app that runs entirely in your browser. Open the file, start planning — no installation, no internet connection, no accounts required. All data is stored locally in your browser's `localStorage`.

### ✨ Features

**Planning**
- Add daily plans with start time, end time, duration, name, notes, category, and priority
- Real-time "in progress" highlight — the current task glows automatically
- Drag-and-drop to reorder tasks
- Sort by time, priority, or creation order
- Task completion tracking with progress bar

**Views**
- **Day View** — focused single-day planning with sidebar stats, timeline, and sticky notes
- **Week View** — 7-day grid overview with weekly goals that sync to daily sticky notes

**Pomodoro Timer 🍅**
- Launch a timer directly from any task
- Auto-calculates remaining time if the task is currently in progress and has an end time
- Fullscreen focus mode with animated countdown ring
- Pause, resume, and reset support
- Plays a sound and sends a browser notification when the session ends

**Sticky Notes & Weekly Goals**
- Global sticky notes panel for quick jottings
- Weekly goals defined in the week view auto-appear in the day view sticky panel
- Bidirectional sync — toggle or delete from either view

**Customization**
- 6 built-in themes: Default, Ocean, Forest, Midnight, Rose, Sand
- Full Chinese / English bilingual interface (toggle in the header)

**Data Management**
- Export all data (tasks, notes, stickies) to a JSON file for backup
- Import from a JSON backup — merges with existing data
- Storage usage monitor with manual cleanup tools (60-day prune or full clear)
- Silent auto-prune of data older than 180 days to keep localStorage lean

**Other**
- Browser notifications before tasks start (opt-in)
- Live clock in the header
- Date navigation (previous / next day, or pick from calendar)
- Print-friendly layout
- Fully responsive design (mobile-friendly)

### 🚀 Getting Started

1. Download `daily-planner.html`
2. Open it in any modern browser (Chrome, Firefox, Safari, Edge)
3. That's it — start planning!

> **Tip:** Bookmark the local file path or host it on GitHub Pages for quick access from any device.

### 🌐 Hosting on GitHub Pages

1. Fork or upload this repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)` folder
4. Your planner will be live at `https://<your-username>.github.io/<repo-name>/daily-planner.html`

### 📦 Tech Stack

| Layer | Technology |
|-------|-----------|
| Structure | HTML5 |
| Styling | CSS3 (CSS Variables, Grid, Flexbox) |
| Logic | Vanilla JavaScript (ES6+) |
| Storage | `localStorage` |
| Fonts | Google Fonts (Playfair Display, DM Sans, DM Mono) |
| Icons | Unicode Emoji |

No frameworks. No build tools. No `node_modules`. Just one file.

### 🗂 File Structure

```
daily-planner.html   ← the entire application
README.md            ← this file
```

### 📄 License

MIT License — free to use, modify, and distribute.

---

## 中文

### 项目简介

日计划是一款**单文件**（`daily-planner.html`）生产力应用，完全在浏览器中运行。打开文件即可开始规划，无需安装、无需网络、无需账号。所有数据保存在浏览器的 `localStorage` 中，完全本地化。

### ✨ 功能列表

**计划管理**
- 添加计划，支持：开始时间、结束时间、持续时长、名称、备注、分类、优先级
- 实时"进行中"高亮——当前任务自动发光标记
- 拖拽排序
- 支持按时间、优先级、添加顺序排序
- 任务完成追踪与进度条

**视图模式**
- **日视图** — 专注单日规划，含统计面板、时间轴、便签
- **周视图** — 7 天网格总览，周目标自动同步至每日便签

**番茄钟 🍅**
- 直接从任意计划启动计时器
- 若计划正在进行且设置了结束时间，自动计算剩余时长
- 全屏专注模式，带动画倒计时圆环
- 支持暂停、继续、重置
- 计时结束时播放提示音并发送浏览器通知

**便签与周目标**
- 全局便签面板，随手记录
- 在周视图中添加的周目标会自动出现在日视图的便签区
- 双向同步——在任意视图勾选或删除均实时同步

**个性化**
- 6 款内置主题：默认、海洋、森林、午夜、玫瑰、沙漠
- 完整中英文双语界面（顶栏一键切换）

**数据管理**
- 将所有数据（计划、笔记、便签）导出为 JSON 文件备份
- 从 JSON 备份恢复，与现有数据合并
- 存储用量监控，支持手动清理（60 天前数据或全部清除）
- 自动静默清理 180 天前的数据，保持 localStorage 轻量

**其他**
- 任务开始前的浏览器通知（用户授权后生效）
- 顶栏实时时钟
- 日期导航（上一天/下一天，或从日历选择）
- 打印友好布局
- 完整响应式设计，移动端适配

### 🚀 快速开始

1. 下载 `daily-planner.html`
2. 用任意现代浏览器打开（Chrome、Firefox、Safari、Edge）
3. 就这些——开始规划吧！

> **小技巧：** 将本地文件路径加入书签，或部署到 GitHub Pages，方便从任意设备访问。

### 🌐 部署到 GitHub Pages

1. Fork 或上传本仓库
2. 进入 **Settings → Pages**
3. 将 Source 设置为 `main` 分支，`/ (root)` 目录
4. 稍等片刻，即可通过 `https://<用户名>.github.io/<仓库名>/daily-planner.html` 访问

### 📦 技术栈

| 层级 | 技术 |
|------|------|
| 结构 | HTML5 |
| 样式 | CSS3（CSS 变量、Grid、Flexbox）|
| 逻辑 | 原生 JavaScript（ES6+）|
| 存储 | `localStorage` |
| 字体 | Google Fonts（Playfair Display、DM Sans、DM Mono）|
| 图标 | Unicode Emoji |

无框架，无构建工具，无 `node_modules`，只有一个文件。

### 🗂 文件结构

```
daily-planner.html   ← 完整应用
README.md            ← 本文件
```

### 📄 许可证

MIT 许可证——可自由使用、修改与分发。

---

<div align="center">

Made with ☕ and lots of planning.  
用 ☕ 和无数规划打造。

</div>
