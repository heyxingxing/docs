# LangGraph 简体中文翻译说明

> 本分支是基于 `langchain-ai/docs` 的社区简体中文翻译，非 LangChain 官方中文版本。

## 翻译范围

优先翻译 `src/oss/langgraph/` 下的 LangGraph 文档。保持原有文件路径，以便复用官方 `docs.json` 导航、内部链接和 Mintlify 构建流程。

## 翻译规则

1. **保持结构不变**：不修改 MDX 组件名、import、路径、anchor、API 引用、代码围栏和构建指令。
2. **代码保持原样**：Python、TypeScript、Shell、JSON 等代码块原则上不翻译，避免示例失真。
3. **翻译可见文案**：包括 frontmatter 的 `title` / `sidebarTitle` / `description`、正文、表格、Tip/Info/Card/Accordion 等组件中的可见文字。
4. **API 标识保持英文**：类名、方法名、参数名、环境变量、包名等不翻译，例如 `StateGraph`、`Command`、`interrupt()`、`LANGSMITH_TRACING`。
5. **术语一致优先**：难以稳定直译或会与 API 名混淆的术语，首次出现时采用“中文（英文）”，后续按术语表统一。
6. **技术准确优先于逐词直译**：保留原文技术含义和约束，不为“中文化”而改变行为描述。

## 核心术语表

| English | 简体中文建议 |
| --- | --- |
| agent | 智能体（Agent） |
| orchestration | 编排 |
| runtime | 运行时 |
| state | 状态 |
| stateful | 有状态的 |
| graph | 图 |
| node | 节点 |
| edge | 边 |
| conditional edge | 条件边 |
| reducer | Reducer（归约器） |
| checkpoint | 检查点（Checkpoint） |
| checkpointer | Checkpointer |
| persistence | 持久化 |
| durable execution | 持久化执行 |
| interrupt | 中断 |
| human-in-the-loop | 人在回路（Human-in-the-loop） |
| streaming | 流式输出 / 流式传输（按上下文） |
| subgraph | 子图 |
| store | Store（存储） |
| short-term memory | 短期记忆 |
| long-term memory | 长期记忆 |
| thread | 线程（Thread） |
| super-step | 超步（Super-step） |
| tool calling | 工具调用 |
| tool call | 工具调用请求 |
| tool node | 工具节点 |
| routing | 路由 |
| retry | 重试 |
| fault tolerance | 容错 |
| observability | 可观测性 |
| tracing | 追踪（Tracing） |
| deployment | 部署 |
| Graph API | Graph API |
| Functional API | Functional API |

## 上游同步

建议保留 `main` 跟踪英文上游，在 `zh-cn` 分支持续维护翻译：

```bash
git remote add upstream https://github.com/langchain-ai/docs.git
git fetch upstream
git diff <last-sync-commit>..upstream/main -- src/oss/langgraph
```

对发生语义变化的段落做增量翻译，避免整页重新翻译导致术语漂移。

## 版权

原始文档来自 `langchain-ai/docs`，遵循其 MIT License。本分支保留原仓库许可证和版权要求。
