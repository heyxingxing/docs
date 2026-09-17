# LangGraph 简体中文汉化状态

> 分支：`zh-cn`  
> 中文文档路径：`src/oss/langgraph/`  
> 上游：`langchain-ai/docs` 的 `main` 分支

本分支直接在与官方一致的路径下维护 LangGraph 中文文档，便于与 upstream 做逐文件 Diff。

## 已完成核心文档

- `overview.mdx` — LangGraph 概览
- `install.mdx` — 安装
- `quickstart.mdx` — 快速开始
- `thinking-in-langgraph.mdx` — LangGraph 心智模型
- `choosing-apis.mdx` — Graph API / Functional API 选择
- `graph-api.mdx` — Graph API 概念
- `use-graph-api.mdx` — Graph API 使用指南
- `functional-api.mdx` — Functional API 概念
- `use-functional-api.mdx` — Functional API 使用指南
- `persistence.mdx` — 持久化
- `checkpointers.mdx` — Checkpointer
- `stores.mdx` — Store
- `add-memory.mdx` — 短期/长期记忆
- `interrupts.mdx` — 人在回路与 Interrupt
- `streaming.mdx` — Streaming
- `event-streaming.mdx` — Event Streaming
- `fault-tolerance.mdx` — Retry / Timeout / Error Handler / Graceful Shutdown
- `use-subgraphs.mdx` — Subgraph
- `use-time-travel.mdx` — Time Travel
- `pregel.mdx` — Pregel Runtime
- `workflows-agents.mdx` — Workflow 与 Agent 模式
- `agentic-rag.mdx` — Agentic RAG
- `sql-agent.mdx` — SQL Agent
- `application-structure.mdx` — 应用结构
- `backward-compatibility.mdx` — 向后兼容
- `case-studies.mdx` — 案例
- `deploy.mdx` — 部署
- `local-server.mdx` — 本地 Server
- `observability.mdx` — 可观测性
- `studio.mdx` — Studio
- `test.mdx` — 测试
- `ui.mdx` — UI

## 子目录

### `errors/`

已汉化：

- `GRAPH_RECURSION_LIMIT.mdx`
- `INVALID_CHAT_HISTORY.mdx`
- `INVALID_CONCURRENT_GRAPH_UPDATE.mdx`
- `INVALID_GRAPH_NODE_RETURN_VALUE.mdx`
- `MISSING_CHECKPOINTER.mdx`
- `MULTIPLE_SUBGRAPHS.mdx`

### `frontend/`

已汉化：

- `overview.md`
- `graph-execution.mdx`
- `custom-stream-channels.mdx`

## 翻译约定

- API 名、Class 名、Method 名、Package 名、环境变量保持英文。
- `State` / `Node` / `Edge` 等在解释语境中使用中文，但代码标识保持原样。
- `Checkpointer`、`Reducer`、`Store` 等容易歧义的专有抽象优先保留英文并辅以中文解释。
- 代码块保持官方代码结构，避免因翻译字符串改变示例行为。
- MDX Component、Import、Route、Anchor 尽量保持与官方一致。
- 中文标题可能改变 Markdown 自动 Anchor；重要内链优先保留官方显式 Anchor 或使用稳定路径。

## 上游同步

建议持续记录同步点：

```bash
git remote add upstream https://github.com/langchain-ai/docs.git
git fetch upstream

git diff <last-sync-commit>..upstream/main -- src/oss/langgraph
```

同步时优先处理：

1. 官方新增页面；
2. API / 参数变化；
3. 代码示例变化；
4. 新增 Warning / Migration / Version Requirement；
5. 最后才是纯措辞变化。

## 完整度说明

“已汉化”表示对应页面已经有简体中文版本并覆盖官方核心主题；上游文档仍会持续变化，因此不能把当前状态理解为永久完成。后续应通过 upstream diff 做增量维护。
