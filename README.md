<div align="center">

# 你好，我是廖文轩 👋

**四川农业大学 · 物联网工程 · 2029 届本科生**

写前端，也把后端、数据库、测试和部署一起做完。
比起「又加了一个功能」，我更在意**它能不能被验证、被复现、被线上用户真的用起来**。

[🚀 在线体验我的主项目](https://csp.bscjs.top/) · [📖 项目 README](https://github.com/Liao-wenxuan/content-sharing-platform)

</div>

---

## 🔨 主项目 · [content-sharing-platform](https://github.com/Liao-wenxuan/content-sharing-platform)

[![CI](https://github.com/Liao-wenxuan/content-sharing-platform/actions/workflows/ci.yml/badge.svg)](https://github.com/Liao-wenxuan/content-sharing-platform/actions/workflows/ci.yml)
[![Browser](https://github.com/Liao-wenxuan/content-sharing-platform/actions/workflows/browser.yml/badge.svg)](https://github.com/Liao-wenxuan/content-sharing-platform/actions/workflows/browser.yml)

**一个从零搭起来、现在还在线上跑着的内容社区。单人、两个多月、700+ 次提交，MIT。**

- **不是 CRUD demo**：个性化推荐流（兴趣画像 / 可解释的推荐理由 / 快照翻页）、WebSocket 实时聊天与通知、评论软删、收藏夹、私密笔记可见性过滤、话题与浏览记录。
- **站内 AI 问答**：切词召回 → 证据组织 → 每条结论可以点回原帖那一段。没接模型 API，retrieval 这层自己写，为什么不用向量库也讲得清。
- **数据层是真的**：`better-sqlite3` 手写 SQL、不用 ORM；迁移、软删、可见性过滤都落在真实读写路径上。
- **工程闭环**：**1045 条单测**（前端 568 / 后端 477）+ **15 套 Playwright e2e** + **35 个 a11y 状态 0 违规**；5-job CI 卡覆盖率、首屏体积、README 配图哈希；`docker compose up` 或 [`deploy/`](https://github.com/Liao-wenxuan/content-sharing-platform/tree/main/deploy) 都能复现部署。
- **性能是量出来的**：Slow 4G 线上 A/B，LCP **5512 → 3872 ms（-30%）**、首屏图片请求 **22 → 11**、总流量 **627 → 454 KB**，CLS 0。

想看怎么造的：[架构文档](https://github.com/Liao-wenxuan/content-sharing-platform/blob/main/docs/architecture.md) · [100+ 条面试题与「为什么这么造」](https://github.com/Liao-wenxuan/content-sharing-platform/blob/main/docs/interview.md) · [部署复现](https://github.com/Liao-wenxuan/content-sharing-platform/blob/main/deploy/README.md)

## 🧩 其他项目

| 项目 | 一句话 | 我更想聊的一点 |
| --- | --- | --- |
| [volleyball-team](https://github.com/Liao-wenxuan/volleyball-team) | 高校排球队管理：考勤 · 成长记录 · 平板战术板 | 零依赖单文件离线即用，也能切云端多端同步；PWA 缓存优先，238 单测 / 3 条 E2E |
| [vigil](https://github.com/Liao-wenxuan/vigil) | 前端可观测性：错误监控 + Web Vitals RUM + Issue 生命周期 | 自己埋点、自己收数据，把「线上到底慢在哪」变成可查的表 |
| [Guanmo-open](https://github.com/Liao-wenxuan/Guanmo-open) | AI 原生 Markdown 阅读器 | 本地 RAG 知识库 + 长期记忆 + Agent 工具，数据不出本机 |
| [coc_trpg](https://github.com/Liao-wenxuan/coc_trpg) | 局域网联机跑团辅助 | AI 主持 / 协助真人 KP 双模式，一次轻量 Agent 编排实践 |

## 🛠 常用技术栈

- **前端** — Vue 3 · TypeScript · Vite · Pinia · Element Plus
- **后端** — Node.js · Express · SQLite（手写 SQL）· WebSocket · JWT
- **工程** — Vitest · Playwright · GitHub Actions · Docker Compose · Caddy · pm2

## 📌 关于我

2029 届本科生，正在把课程之外的工程实践做扎实，也开放实习与技术交流机会。

给自己定的验收标准是：**陌生人 5 分钟能把项目装起来，连着问我 5 个「为什么这么造」，我能答上来。**
所以文档、部署脚本和那份 [interview.md](https://github.com/Liao-wenxuan/content-sharing-platform/blob/main/docs/interview.md) 写得比功能还认真。想聊某个具体实现，欢迎到主项目开 Issue。
