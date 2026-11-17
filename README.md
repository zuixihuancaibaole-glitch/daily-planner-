# 日计划 · Daily Planner

用「开始时间 + 持续时间」排出一天的时间表，把常用安排保存为计划卡片，在周视图回顾进度。也可以用 Wallpaper Engine 把今天的计划放到 Windows 桌面，直接勾选完成。

Build a schedule from start times and durations, save recurring tasks as plan cards, and review your week. You can also check off today's tasks from your Windows desktop with Wallpaper Engine.

[中文](#中文) · [English](#english) · [下载 / Download `index.html`](https://raw.githubusercontent.com/zuixihuancaibaole-glitch/daily-planner-/main/index.html)

## 中文

### 快速开始

下载 [`index.html`](index.html)，用浏览器打开即可使用。无需安装依赖或注册账号。顶部可切换中英文、日视图和周视图。选好日期，在「添加计划」中输入任务名称，按 Enter 或点击「添加计划」。时间、备注和分类均可选，也可设置高、中、低优先级。没有开始时间的任务显示为「全天」。

### 用持续时间排出一天

「开始时间」「结束时间」和「持续时间」会联动，持续时间以**分钟**输入。

| 操作 | 结果 |
| --- | --- |
| 填 `08:30` 为开始，持续时间填 `45` | 自动算出结束时间 `09:15`。未填开始时间时，持续时间不可编辑。 |
| 把结束时间改成 `09:30` | 同一天内，结束晚于开始时，持续时间反算为 `60` 分钟。 |
| 保留 `60` 分钟，把开始改成 `08:45` | 结束时间跟着移到 `09:45`，任务时长不变。 |
| 添加这条计划，再录入下一条 | 表单将最近添加的计划的结束时间带到下一条的开始栏；没填结束时间时，沿用它的开始时间。 |
| 点击开始时间旁的「现在」 | 填入电脑当前的时分；已填的持续时间也会用于重算结束时间。 |

适合连续安排课程、学习和休息：先定第一项几点开始，后面逐条填名称和分钟数即可。跨午夜时，按时长计算的结束时刻会回到 `00:00` 之后，但任务仍属于所选日期；从起止时间反算时长仅适用于结束晚于开始的同日时段。

### 用计划卡片复用常用安排

1. 在「添加计划」中填好开始时间，启用「计划卡片」按钮。
2. 要保存卡片，填写事件名称和持续时间（1–1439 分钟），按需填写备注、分类和优先级，然后点「计划卡片」→「保存当前表单」。
3. 要套用卡片，先填这次的开始时间，再点「计划卡片」，选中一张并点「套用卡片」。表单会带入卡片信息并算出结束时间。检查或修改表单后，点「添加计划」。

例如，开始时间填 `19:30`，套用一张 **45 分钟**的刷题卡片，结束时间就会填为 `20:15`。若计算出的结束时间会跨到次日，页面会提示提前开始时间，并保留当前表单。

### 日程、目标与专注

| 功能 | 用法 |
| --- | --- |
| 日视图与时间轴 | 用左右箭头翻日，或点日期选一天。日视图显示任务总数、完成数、待完成数、重要事项和完成进度；时间轴展示有开始时间的任务和当前时刻，正在进行的未完成任务会高亮。 |
| 任务管理 | 勾选完成、编辑名称与时间等信息，或删除。支持按时间、优先级、添加顺序查看，也可拖动排序。删除任务会先确认，之后可在提示条撤销。 |
| 复制到明天 | 把所选日期的任务复制到它的下一天，并跳到目标日期。副本保留原时间、备注、分类与优先级，完成状态重置。目标日期已有任务时，确认后追加，可撤销。 |
| 批量调整时间 | 在今天的日视图点击「批量调整时间」，选「提前」或「延后」，输入分钟数并确认。正在进行和尚未开始的未完成计划会一起移动；已完成、已结束和没有开始时间的计划不变。 |
| 周视图 | 按周一至周日查看任务预览、完成率和未完成的高优先级任务数。可翻周、返回本周，或点某一天进入其日视图。 |
| 便签、周目标和每日笔记 | 「当日」便签只在选定日期显示，「全部」便签跨日显示。周目标可在周视图添加，也会出现在当周日视图的便签区，两处均可勾选或删除。每日笔记按日期自动保存。 |
| 任务番茄钟 | 点击任务旁的 🍅。正在进行且有结束时间的任务可按剩余时间倒计时，也可手动设定 1–480 分钟。支持暂停、继续和重置；时间到会尝试播放提示音，在浏览器允许时发送通知。 |
| 浏览器提醒 | 按页面提示开启通知并保持页面打开。当天未完成、设有开始时间的任务可在开始前 1–10 分钟收到提醒；本地文件的通知权限取决于浏览器。 |
| 显示与打印 | 顶栏包含实时钟、打印按钮和七种主题：纸感、海洋、森林、午夜、玫瑰、沙色、薄荷。布局会随窗口宽度调整。 |

例如，选「提前」`20` 分钟会将 `15:00–15:45` 移到 `14:40–15:25`，时长不变。只有开始时间的计划只调整开始时间。如果任一计划会跨到前一天或后一天，整批不会改动；调整后可在提示条点击「撤销」。

### 把今日计划放到 Windows 桌面

安装并选用配套的 **Wallpaper Engine 网页壁纸**后，桌面会显示今日计划、完成进度、便签和本周目标。网页上修改计划后，壁纸会自动刷新；在壁纸上勾选任务或便签，完成状态也会同步回网页。壁纸还有任务番茄钟、可选的到点提醒，以及缩放、深浅外观、颜色和便签显示设置。

1. 准备 Windows、Steam 版 Wallpaper Engine、Node.js 和配套文件。当前仓库只包含网页，另需取得 `wallpaper-sync/每日计划.vbs`、`wallpaper-sync/sync-server.mjs`，以及 Wallpaper Engine 网页壁纸项目（至少包含 `project.json` 和 `wallpaper.html`，保留随附资源）。
2. 把下载的 `index.html` 另存为 `daily-planner.html`，放在 `wallpaper-sync/` 的上一级目录。双击 `wallpaper-sync/每日计划.vbs`，即可启动本机同步服务并打开网页。也可在项目目录手动运行 `node wallpaper-sync/sync-server.mjs`，再打开自己的计划网页。
3. 在 Wallpaper Engine 中添加并选用配套网页壁纸。网页顶栏的「桌面壁纸」按钮会尝试推送数据并通过 Steam 打开 Wallpaper Engine；首次使用仍需在引擎中添加并选择壁纸。
4. 查看 **数据 → 壁纸同步**。显示「已连接」时，两端通过 `http://127.0.0.1:17931/api/data` 同步，通常几秒内更新。若显示离线，先检查 `http://127.0.0.1:17931/health`；服务未运行时重新打开启动器，壁纸可能暂时显示上次缓存。需要随 Windows 登录启动时，可用 `shell:startup` 打开启动文件夹，并添加以 `server` 为参数运行启动器的快捷方式。

同步发生在同一台电脑上。跨设备或更换浏览器请用 JSON 备份迁移。通过在线网页同步时，还取决于浏览器是否允许访问本机服务；遇到限制可使用启动器打开本地网页。

### 数据、离线使用与部署

- 计划、每日笔记和便签（包括周目标）保存在当前浏览器的 IndexedDB，并保留 `localStorage` 缓存。计划卡片及主题、语言和视图偏好保存在 `localStorage`。顶部 **数据 → 导出 JSON** 可备份计划、笔记、便签和计划卡片，换浏览器、电脑或站点地址时可导入。
- 导入时，备份中已有的日期会覆盖对应日期的任务列表和笔记。若文件包含便签列表，会替换现有便签及周目标。计划卡片会合并，内容完全相同的卡片只保留一张。导入前建议先导出当前数据。
- **历史清理：**数据面板可查看存储用量、清理 60 天前的计划和每日笔记，或清理今天以前的所有计划和每日笔记。页面加载时也会清理超过 180 天的计划和每日笔记；想长期保留请定期导出。
- **离线使用：**单个 HTML 可离线运行核心功能。无法加载 Google Fonts 时，页面使用系统备用字体。
- **GitHub Pages：**在自己的 GitHub 仓库中打开 **Settings → Pages**，选择 **Deploy from a branch**，设为 `main` 和 `/ (root)`，保存后使用设置页提供的站点地址。部署只发布网页；壁纸同步服务仍在本机运行。[GitHub Pages 官方说明](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## English

### Get started and schedule by duration

Download [`index.html`](index.html) and open it in a browser. No installation or account is required for the planner. Select a date, enter a task name, and press Enter or choose **Add Plan**. Time, notes, and category are optional, and each task can have high, medium, or low priority. Tasks without a start time appear as all-day tasks.

- Enter `08:30` and `45` minutes to get an end time of `09:15`. The duration field becomes available once you set a start time.
- Change the end time to `09:30` to calculate a duration of `60` minutes. If you then change the start to `08:45`, the planner keeps the duration and moves the end to `09:45`.
- The next entry defaults to the most recently added task's end time, or its start time when it has no end. **Now** fills in the current time and recalculates the end if a duration is already set.
- Adding minutes can wrap the clock past midnight while keeping the task on its selected date. Calculating a duration from two times works when the end is later than the start on the same day.

### Reuse common tasks with Plan Cards

1. Set a start time in the **Add Plan** form to enable **Plan Cards**.
2. To save a card, enter an event name and a duration of 1–1439 minutes. Add notes, a category, and a priority as needed. Choose **Plan Cards → Save Current Form**.
3. To use a card, enter the start time for this occasion, open **Plan Cards**, select a card, and choose **Apply Card**. The form fills in the saved fields and calculates the end time. Review or edit the form, then choose **Add Plan**.

For example, applying a **45-minute** practice card at `19:30` fills in an end time of `20:15`. If the card would end on the next day, the planner keeps the current form and asks you to choose an earlier start time.

### Planning, notes, and focus

| Feature | What it does |
| --- | --- |
| Day view and timeline | Browse with the date arrows or picker. See completion stats, timed tasks and the current time on the timeline, and a highlight for unfinished tasks in progress. |
| Task management | Check off, edit, or delete tasks. Sort by time, priority, or creation order, or drag to reorder. Confirm a deletion and use the toast to undo it. |
| Copy to next day | Copy the selected day's tasks as unfinished, then open the next date. The app asks before appending to existing tasks, and the copy can be undone. |
| Shift plans | In today's day view, choose **Shift plans**, select **Earlier** or **Later**, enter the number of minutes, and confirm. This moves in-progress and upcoming unfinished tasks. Completed tasks, tasks that have ended, and tasks without a start time stay as they are. |
| Week view | Browse Monday to Sunday, see task previews and weekly completion, and select a day to open its plan. Jump back to the current week at any time. |
| Stickies, weekly goals, and notes | Use date-specific or all-days stickies. Weekly goals appear in both the week view and the corresponding daily sticky area. Daily notes autosave for the selected date. |
| Pomodoro timer and reminders | Open the timer from a task to use its remaining time or set 1–480 minutes yourself. Pause, resume, or reset. The timer attempts to play a sound and can send a notification when allowed. With browser permission and the page open, today's unfinished timed tasks can also trigger alerts 1–10 minutes before they start. Local-file notification support varies by browser. |
| Appearance and printing | Switch between Chinese and English and seven themes. The page adapts to the window width and offers a live clock and a print button. |

For example, shifting `15:00–15:45` **Earlier** by `20` minutes gives `14:40–15:25`, with the same duration. Tasks with only a start time keep that format. The entire shift is blocked if any task would move outside today. Use **Undo** in the confirmation toast to restore the previous times.

### Use today's plan as a Windows wallpaper

The companion Wallpaper Engine web wallpaper displays today's tasks and progress, stickies, and this week's goals. Task and sticky checkmarks sync back to the webpage. The wallpaper also offers a Pomodoro timer, optional start-time reminders, UI scaling, light and dark appearance, colors, and a switch for the sticky panel.

1. Install Node.js and Wallpaper Engine on Windows. The repository contains the planner page; get the separate launcher and sync server (`wallpaper-sync/每日计划.vbs` and `wallpaper-sync/sync-server.mjs`) and the companion Wallpaper Engine project (`project.json`, `wallpaper.html`, and any accompanying assets).
2. Save `index.html` as `daily-planner.html` one level above `wallpaper-sync/`. Run `每日计划.vbs` to start the local service and open the page. Alternatively, run `node wallpaper-sync/sync-server.mjs` and open the planner yourself.
3. Add and select the companion project in Wallpaper Engine. The planner's **Desktop Wallpaper** button sends data to the service and tries to launch Wallpaper Engine via Steam; you still need to select the wallpaper on first use.
4. Check **Data → Wallpaper Sync**. When connected, changes normally appear within a few seconds via `http://127.0.0.1:17931/api/data`. Check `http://127.0.0.1:17931/health` if offline. The wallpaper may show cached data until the service is back. To start the service at Windows sign-in, put a shortcut to the launcher with the `server` argument in the Startup folder.

Wallpaper sync stays on the same computer. If a hosted page is blocked from reaching the local service, use the local HTML file. Use JSON backups for moving data across browsers or devices.

### Storage, offline use, and deployment

- The current browser stores plans, daily notes, stickies, and weekly goals in IndexedDB with a `localStorage` cache. Plan cards and language, theme, and view preferences are stored in `localStorage`. Export plans, notes, stickies, and plan cards from **Data** as a JSON backup before moving to a different browser, device, or site address.
- Import replaces task lists and daily notes for matching dates. If the backup contains stickies, it replaces the sticky note list, including weekly goals. Plan cards are merged, with identical cards kept once. Export your current data first if you need a recovery copy.
- The data panel shows storage usage and offers cleanup for tasks and daily notes older than 60 days or dated before today. Startup also clears tasks and notes older than 180 days. Export records you want to keep.
- The downloaded HTML runs the core planner offline and uses system fallback fonts if Google Fonts is unavailable.
- For GitHub Pages, go to **Settings → Pages → Deploy from a branch**, choose `main` and `/ (root)`, and open the URL shown after deployment. Pages hosts the planner only; the wallpaper service runs on your computer. [GitHub Pages publishing guide](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## 文件与许可 / Files and license

- [`index.html`](index.html) — 单文件网页应用 / The planner in one HTML file, with CSS and vanilla JavaScript.
- [`LICENSE`](LICENSE) — MIT License.
