# LangGraph 中文文档

这是 `langchain-ai/docs` 中 LangGraph 官方文档的简体中文社区翻译分支。

> 本项目为**非官方中文翻译**。英文原文及代码版权归 LangChain, Inc. 与原贡献者所有，遵循原仓库 MIT License。

## 阅读入口

LangGraph 中文正文保持与官方仓库相同的路径结构：

```text
src/oss/langgraph/
```

建议按以下顺序阅读：

1. `overview.mdx` — LangGraph 概览
2. `quickstart.mdx` — 快速入门
3. `thinking-in-langgraph.mdx` — LangGraph 思维方式
4. `graph-api.mdx` — Graph API
5. `functional-api.mdx` — Functional API
6. `persistence.mdx` / `checkpointers.mdx` — 持久化与 Checkpoint
7. `interrupts.mdx` — 人在回路
8. `streaming.mdx` / `event-streaming.mdx` — Streaming
9. `fault-tolerance.mdx` — 容错
10. `use-subgraphs.mdx` — 子图
11. `add-memory.mdx` / `stores.mdx` — 记忆与 Store

## 翻译原则

- 保留 API、类名、方法名、参数名、包名、环境变量等技术标识。
- 保留 MDX 组件、import、代码块、链接路径与 Anchor。
- 翻译标题、正文、表格、提示框和可见 UI 文案。
- 术语优先保证技术准确，而不是逐词直译。
- `Checkpointer`、`Reducer`、`Store` 等容易歧义的核心术语在中文正文中保留英文标识。

详细规范见 [`ZH_CN_TRANSLATION.md`](./ZH_CN_TRANSLATION.md)。

## 与官方同步

建议将官方仓库添加为 `upstream`：

```bash
git remote add upstream https://github.com/langchain-ai/docs.git
git fetch upstream
```

查看 LangGraph 官方文档变更：

```bash
git diff <last-sync-commit>..upstream/main -- src/oss/langgraph
```

翻译维护采用**增量同步**：只处理官方新增或语义发生变化的段落，尽量避免整页重新翻译导致术语漂移。

## 当前状态

`zh-cn` 分支已完成 LangGraph 顶层文档的中文覆盖。`errors/` 与 `frontend/` 子目录继续按同一规范补齐，并在完成后执行 MDX / 链接 / CI 校验。
