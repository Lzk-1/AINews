# AINews

AI 驱动的大模型技术与应用资讯聚合平台。

从多源采集 → 去重清洗 → AI 评分过滤 → 摘要增强 → 多渠道分发，帮你从信息洪流中筛出真正值得看的内容。

## 核心特性

- **多源立体采集**：RSS / Hacker News / Reddit / GitHub Trending / arXiv / X/Twitter / 微信公众号，三层信源交叉验证
- **AI 评分过滤**：LLM 对每条内容 0-10 分评分，只保留高价值内容
- **三级去重**：URL 精确去重 + SimHash 标题去重 + 语义向量去重
- **摘要增强**：AI 生成冷静克制的中文摘要，高价值内容补充背景分析和社区讨论
- **多渠道分发**：Web 浏览 / 邮件日报 / 飞书/钉钉/Discord/Slack 推送 / REST API / MCP Server
- **零运维部署**：Docker Compose 一键部署，SQLite 单文件存储

## 文档

- [需求文档（PRD）](docs/需求文档.md)
- [开发方案设计文档](docs/开发方案设计文档.md)

## 技术栈

| 层级 | 技术 |
|------|------|
| 后端 | Python 3.12+ / FastAPI / SQLAlchemy / APScheduler |
| 数据存储 | SQLite + ChromaDB（嵌入式向量库） |
| AI | OpenAI 兼容接口（DeepSeek/GPT/Claude/Gemini/Ollama） + sentence-transformers |
| 前端 | Next.js 15 / React 19 / TypeScript / shadcn/ui / Tailwind CSS |
| 部署 | Docker Compose |

## License

MIT
