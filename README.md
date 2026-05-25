# GitHub Trending Daily

每日自动抓取的 GitHub Trending 归档。由 Mac Mini 上的 **Alita**(OpenClaw)每天 09:00（Asia/Shanghai）调度生成并推送。

## 内容

- 按年份归档：`YYYY/YYYY-MM-DD.md`
- 每份报告含多维度 Trending：Overall / Python / Shell / Rust / Zig / TypeScript / 中文 / 英文，以及 Weekly / Monthly 切片
- 含分类标签、关注度评级与当日简报

## 自动化

- 抓取脚本：`github_trending.py`（requests + BeautifulSoup）
- 调度：OpenClaw cron（`0 9 * * *`，Asia/Shanghai）
- 流程：抓取 → 写入本地 → 复制进本仓库 → commit & push

*（自动维护，请勿手动编辑历史归档。）*
