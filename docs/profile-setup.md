# 个人主页维护说明

## 首次启用

将修改推送到 `GrushTom/GrushTom` 的 `main` 分支。工作流文件的首次推送会触发 **Generate contribution snake**，成功后将两张动画发布到 `output` 分支。首次运行完成前，README 的动画位置可能显示替代文字。

也可以在仓库 **Actions → Generate contribution snake → Run workflow** 手动生成。此后每天 UTC 00:17（日本时间 09:17）更新。工作流使用 GitHub 自动提供的 `GITHUB_TOKEN`，无需创建个人 Token；仓库需要允许 GitHub Actions 运行。若发布阶段提示 403，请检查仓库或组织策略是否允许工作流的 `contents: write` 权限。

## 修改内容

- 自我介绍、技术栈与博客链接：编辑 `README.md`。
- 统计卡片：修改 README 中的 `github-stats-extended.vercel.app` URL；深色和浅色参数分别设置。卡片由公共服务提供并缓存，偶尔可能限流或不可用。
- 贪吃蛇：编辑 `.github/workflows/snake.yml`。`output` 分支由生成任务维护。
- 打字动画、技术图标和徽章使用第三方图片服务；文字介绍及博客链接独立保留。

当前只使用原 README 已确认的 JavaScript、TypeScript 和 Python，未添加未经确认的技术、项目、邮箱或个人经历。若要扩展，可补充代表项目的仓库链接、其他常用技术，以及想展示的公开联系方式。

## 参考

- [GitHub Stats Extended](https://github.com/stats-organization/github-stats-extended)：贡献统计与语言卡片。
- [GitHub Profile Tutorial](https://github.com/wmuj/github-profile-tutorial)：打字动画、技术图标、贡献贪吃蛇的组合思路。
- [Platane/snk](https://github.com/Platane/snk)：贡献动画生成。

本版未启用需要额外账号配置的 WakaTime 或 Metrics。
