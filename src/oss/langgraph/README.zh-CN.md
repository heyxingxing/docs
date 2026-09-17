# LangGraph 中文文档导航

> 这是 `zh-cn` 分支的社区简体中文导航页。正式页面仍保持与官方相同的 `.mdx` 文件名，方便后续与 upstream 同步。

## 入门

| 页面 | 内容 |
|---|---|
| [`overview.mdx`](./overview.mdx) | LangGraph 定位、核心能力与生态 |
| [`install.mdx`](./install.mdx) | 安装 |
| [`quickstart.mdx`](./quickstart.mdx) | 使用 Graph API / Functional API 构建第一个 Agent |
| [`thinking-in-langgraph.mdx`](./thinking-in-langgraph.mdx) | 如何把真实流程拆成 State、Node、Edge 与 Error Flow |
| [`choosing-apis.mdx`](./choosing-apis.mdx) | Graph API 与 Functional API 如何选择 |

## Graph API

| 页面 | 内容 |
|---|---|
| [`graph-api.mdx`](./graph-api.mdx) | Graph / State / Reducer / Node / Edge / Send / Command / Runtime |
| [`use-graph-api.mdx`](./use-graph-api.mdx) | Graph API 完整实践、分支、并行、循环、Retry、Cache、Visualization |
| [`use-subgraphs.mdx`](./use-subgraphs.mdx) | Subgraph、State 转换、Per-invocation / Per-thread Persistence |
| [`use-time-travel.mdx`](./use-time-travel.mdx) | Replay、Fork 与历史 State |
| [`pregel.mdx`](./pregel.mdx) | LangGraph 底层 Pregel Runtime |

## Functional API

| 页面 | 内容 |
|---|---|
| [`functional-api.mdx`](./functional-api.mdx) | Entrypoint、Task、Determinism、Idempotency |
| [`use-functional-api.mdx`](./use-functional-api.mdx) | 并行 Task、Streaming、Retry、HITL、Memory、Checkpoint 管理 |

## 持久化、记忆与容错

| 页面 | 内容 |
|---|---|
| [`persistence.mdx`](./persistence.mdx) | Checkpointer vs Store |
| [`checkpointers.mdx`](./checkpointers.mdx) | Thread、Checkpoint、Pending Writes、Serializer、Durability |
| [`stores.mdx`](./stores.mdx) | 长期数据 Store |
| [`add-memory.mdx`](./add-memory.mdx) | 短期记忆、长期记忆、Semantic Search 与 Context Management |
| [`fault-tolerance.mdx`](./fault-tolerance.mdx) | Retry、Timeout、Error Handler、Saga、Graceful Shutdown |
| [`interrupts.mdx`](./interrupts.mdx) | 人在回路、审批、编辑、Resume、幂等规则 |

## Streaming 与前端

| 页面 | 内容 |
|---|---|
| [`streaming.mdx`](./streaming.mdx) | Stream Mode、LLM Token、Custom Data、Subgraph、Debug |
| [`event-streaming.mdx`](./event-streaming.mdx) | v3 Event Streaming / Projection API |
| [`ui.mdx`](./ui.mdx) | LangGraph UI |
| [`frontend/`](./frontend/) | 前端集成、Graph Execution、Custom Stream Channel |

## Agent / Workflow 示例

| 页面 | 内容 |
|---|---|
| [`workflows-agents.mdx`](./workflows-agents.mdx) | Prompt Chaining、Routing、Parallelization、Orchestrator-Worker、Evaluator-Optimizer、Agent Loop |
| [`agentic-rag.mdx`](./agentic-rag.mdx) | Agentic RAG |
| [`sql-agent.mdx`](./sql-agent.mdx) | SQL Agent |

## 工程化

| 页面 | 内容 |
|---|---|
| [`application-structure.mdx`](./application-structure.mdx) | LangGraph 应用目录与配置 |
| [`local-server.mdx`](./local-server.mdx) | 本地 Agent Server |
| [`deploy.mdx`](./deploy.mdx) | 部署 |
| [`observability.mdx`](./observability.mdx) | LangSmith 可观测性 |
| [`studio.mdx`](./studio.mdx) | LangSmith Studio |
| [`test.mdx`](./test.mdx) | 测试 Graph / Node |
| [`backward-compatibility.mdx`](./backward-compatibility.mdx) | API / Schema / Business Compatibility |
| [`case-studies.mdx`](./case-studies.mdx) | 案例 |

## 错误排查

见 [`errors/`](./errors/)：

- `GRAPH_RECURSION_LIMIT`
- `INVALID_CHAT_HISTORY`
- `INVALID_CONCURRENT_GRAPH_UPDATE`
- `INVALID_GRAPH_NODE_RETURN_VALUE`
- `MISSING_CHECKPOINTER`
- `MULTIPLE_SUBGRAPHS`

## 推荐学习路线

```text
Overview
  ↓
Quickstart
  ↓
Thinking in LangGraph
  ↓
Graph API / Functional API
  ↓
Persistence + Interrupt + Streaming
  ↓
Memory + Subgraph + Fault Tolerance
  ↓
Workflow / Agent Patterns
  ↓
Deployment + Observability + Testing
```

## 维护说明

官方文档会持续更新。中文版本应通过 upstream diff 增量同步，而不是长期静态冻结：

```bash
git fetch upstream
git diff <last-sync-commit>..upstream/main -- src/oss/langgraph
```

优先同步 API 行为、代码、版本要求、Migration 与 Warning；纯措辞变化优先级较低。
