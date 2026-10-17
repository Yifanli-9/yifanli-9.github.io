# yifanli-9.github.io

个人学术主页（基于 [academicpages](https://github.com/academicpages/academicpages.github.io) 模板），线上地址：<https://yifanli-9.github.io>

## 怎么改内容

| 想改什么 | 改哪里 |
|---|---|
| 首页自我介绍 | `_pages/about.md` |
| 侧边栏（姓名、职位、单位、邮箱、ORCID 等） | `_config.yml` 的 `author:` 部分 |
| 头像 | 替换 `images/profile.jpg`（文件名保持不变） |
| 论文 | `_publications/` 每篇一个 `.md` 文件，照现有文件的格式抄 |
| 学会发表 | `_talks/`；invited talk 写 `type: "Invited talk"`，获奖写 `award: "🏆 奖名"`，两类报告置顶；其余按年份倒序，合作报告写 `first_author: false`，排在各年一作者报告之后；只知道年份时加 `date_precision: year` |
| 已接收论文 | `_publications/`；加 `status: accepted`，页面显示 Accepted for publication；`date` 用于年份分组和排序，正式出版后更新日期、DOI 和状态 |
| 授课 | `_teaching/`；学期写在 `semester:` 字段 |
| CV | `_pages/cv.md`（下方的 Publications / Talks / Teaching 三节是自动生成的，不用手动更新） |
| 顶部导航栏 | `_data/navigation.yml` |

## 怎么发布

```bash
git add -A && git commit -m "update" && git push
```

推送后 GitHub 自动构建，一两分钟生效。构建状态看仓库的 Actions 标签页（"pages build and deployment"）。
