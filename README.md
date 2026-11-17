# Daily Planner · 日计划

把一天的安排放进时间轴，用周视图回顾进度，把临时想法和本周目标留在便签里。日计划是一个单页网页应用，下载后可直接用浏览器打开。

Plan your day on a timeline, review the week at a glance, and keep quick notes and weekly goals beside your schedule. Download one HTML file and open it in your browser.

[中文](#中文) · [English](#english) · [下载 / Download `index.html`](https://raw.githubusercontent.com/zuixihuancaibaole-glitch/daily-planner-/main/index.html)

## 中文

### 快速开始

1. 下载仓库根目录的 `index.html`。如果链接打开的是 HTML 源码，可在浏览器中按 **Ctrl+S** 保存为 `index.html`。
2. 用浏览器打开文件。页首可以切换中英文、配色以及日视图和周视图。
3. 选好日期，在新增计划表单中填写任务名称。也可补充开始时间、结束时间或预计时长，以及分类、优先级和备注。

### 安排一天和一周

| 功能 | 用法 |
| --- | --- |
| 日视图 | 用日期箭头或日历跳到指定日期。任务列表用于勾选、编辑、删除和排序，时间轴展示有时间安排的任务，进度区显示当日完成情况。当前时间落在某项未完成任务的时间段内时，该任务会高亮。 |
| 任务排序 | 可按时间、优先级或添加顺序查看，也可拖动任务调整位置。 |
| 复制计划到次日 | 将当前所选日期的任务追加到下一天，并把副本设为未完成。次日已有任务时会先提示确认，复制后可在提示条中撤销。 |
| 周视图 | 按周一至周日查看任务和完成情况，点击某天可进入对应的日视图。 |
| 笔记、便签和周目标 | 每日笔记随所选日期保存。便签可以设为「当日」或「全部」。周视图创建的目标也会显示在对应一周的日视图便签区，可从任一视图勾选或删除。 |
| 番茄钟 | 点击任务旁的 🍅 打开计时器。正在进行且设有结束时间的任务可用剩余时间预填倒计时，也可手动设置。计时器支持暂停、继续和重置，结束时会尝试播放提示音，并在浏览器权限允许时发送通知。 |
| 开始前提醒 | 在浏览器支持通知的环境中授权，并保持页面开启。当天未完成且设有开始时间的任务可提前 1–10 分钟提醒。直接打开本地文件时，通知能否使用取决于浏览器。 |

页首提供打印按钮和七款配色，包括默认、海洋、森林、午夜、玫瑰、沙色和薄荷。页面会根据屏幕宽度调整布局。

### 数据保存、备份和迁移

- 任务、每日笔记和便签保存在当前浏览器中。应用使用 IndexedDB 持久化，同时保留 `localStorage` 缓存。主题、语言和视图偏好保存在 `localStorage`。
- 在页首打开数据管理，导出 `daily-planner-YYYY-MM-DD.json`。换浏览器、换设备或改用在线地址前，可以先导出，再在新环境里导入。
- 导入按日期写入备份中的任务和笔记。备份与现有数据有同一天的记录时，对应数据会被覆盖。备份包含便签时，便签列表会被替换。导入前可以先导出当前数据。
- 页面加载时会清理超过 180 天的任务和每日笔记。数据管理也提供 60 天前数据清理，以及清理今天以前的任务和每日笔记。需要长期保留的记录可先导出。

### 离线使用和可选壁纸同步

下载 HTML 后，日常规划功能可以离线使用。页面会尝试加载 Google Fonts，离线时使用备用字体。

页面带有 Wallpaper Engine 入口。壁纸同步需要另行配置本机同步服务和壁纸，页面通过 `127.0.0.1:17931` 与本机服务通信。GitHub 仓库提供网页文件，独立下载即可使用日程、便签和番茄钟。

### 部署到 GitHub Pages

将仓库放到自己的 GitHub 账号下，在 **Settings → Pages** 中选择 **Deploy from a branch**，再选择 `main` 分支和 `/ (root)`，点击 **Save**。部署完成后，在 Pages 设置页打开站点地址，根路径会加载 `index.html`。本地文件和在线站点各有浏览器存储，搬迁时使用 JSON 导出与导入。

[GitHub Pages 官方配置说明](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## English

### Getting started

1. Download `index.html` from the repository. If the download link opens the source, use your browser’s **Save As** command.
2. Open the file in your browser. Use the header to choose a language, theme, and day or week view.
3. Select a date and enter a task name. Add a start time, end time or estimated duration, category, priority, and notes as needed.

### Planning and focus

| Feature | How to use it |
| --- | --- |
| Day view | Navigate with the date arrows or calendar. Check off, edit, delete, or sort tasks. Timed tasks appear on the timeline, and an unfinished task is highlighted during its scheduled time window. |
| Sorting | View tasks by time, priority, or creation order, or drag a task to rearrange the list. |
| Copy to the next day | Append the selected date’s tasks to the following day as unfinished copies. The app asks for confirmation when the destination already has tasks and offers Undo immediately after copying. |
| Week view | Review tasks and completion from Monday through Sunday. Select a day to open its daily plan. |
| Notes and goals | Daily notes follow the selected date. Sticky notes can be scoped to one day or shown across days. Weekly goals also appear in the sticky notes area for the corresponding week and can be checked off or deleted from either view. |
| Pomodoro timer | Use the 🍅 button on a task. For a task already in progress with an end time, the timer can start with the time remaining. You can also set the duration yourself, pause, resume, or reset. The app attempts to play a sound when time is up and shows a notification when permitted. |
| Task reminders | Allow browser notifications and keep the page open for reminders 1–10 minutes before an unfinished task scheduled for today starts. Support for notifications on local files depends on the browser. |

The header includes a print button and seven themes (Default, Ocean, Forest, Midnight, Rose, Sand, and Mint). The layout adapts to screen width.

### Storage, backups, and migration

- Tasks, daily notes, and sticky notes are saved in the current browser using IndexedDB and a `localStorage` cache. Theme, language, and view preferences are kept in `localStorage`.
- Use the data management panel to export a `daily-planner-YYYY-MM-DD.json` backup before moving to another browser, device, or site address. Import it in the new environment to bring your plans and notes over.
- Import replaces task lists and daily notes for matching dates included in the backup. If the backup includes sticky notes, it replaces the sticky note list. Export your current data first if you want a recovery copy.
- At startup, the app prunes tasks and daily notes older than 180 days. The data panel also offers cleanup for records older than 60 days or dated before today. Export records you want to keep long term.

### Offline use and optional wallpaper integration

Core planning features work with the downloaded HTML file offline. The page requests Google Fonts and falls back to available fonts when offline.

The page can launch Wallpaper Engine. Desktop wallpaper synchronization requires a separately configured wallpaper and local service at `127.0.0.1:17931`. Planning, notes, and the timer run directly from the HTML file.

### Deploying to GitHub Pages

In your GitHub repository, open **Settings → Pages**, choose **Deploy from a branch**, then select `main` and `/ (root)`, then click **Save**. Once deployed, open the URL shown in Pages settings. GitHub Pages serves `index.html` at the root of the site. Use JSON export and import to transfer data between a local file and a hosted site.

[GitHub Pages publishing documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## 文件与许可 / Files and license

- [`index.html`](index.html) — 网页应用，包含 HTML、CSS 和原生 JavaScript / The entire app in HTML, CSS, and vanilla JavaScript.
- [`LICENSE`](LICENSE) — MIT License.
