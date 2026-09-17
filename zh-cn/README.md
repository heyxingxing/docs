# LangGraph 中文文档（社区翻译）

> 本目录是基于 LangChain 官方文档仓库中 `src/oss/langgraph/` 的简体中文社区翻译，**非 LangChain 官方中文站**。

## 翻译原则

- 保留 MDX 组件、代码块、API 名称、import、路径、anchor 和可执行示例。
- 翻译标题、正文、表格、提示框、可见 UI 文案和解释性说明。
- 产品名、类名、方法名、参数名、环境变量以及代码示例中的 Prompt/注释等技术内容默认保持英文，避免改变示例行为。
- 对容易歧义的术语，优先采用“中文 + 英文原词”或直接保留英文，例如 `Checkpointer`、`Reducer`、`Entrypoint`、`Task`。
- 翻译目标是技术准确和中文可读性，不做逐词直译。

## 目录

中文镜像位于：

```text
zh-cn/src/oss/langgraph/
```

英文上游位于：

```text
src/oss/langgraph/
```

术语表见 [`GLOSSARY.md`](./GLOSSARY.md)。

## 汉化进度

### 已完成

- [x] `overview.mdx` — LangGraph 概览
- [x] `install.mdx` — 安装
- [x] `quickstart.mdx` — 快速开始
- [x] `thinking-in-langgraph.mdx` — 用 LangGraph 的方式思考
- [x] `choosing-apis.mdx` — Graph API / Functional API 选择指南
- [x] `functional-api.mdx` — Functional API 概览
- [x] `persistence.mdx` — 持久化概览

### 下一批

- [ ] `graph-api.mdx` — Graph API 概览
- [ ] `use-graph-api.mdx` — 使用 Graph API
- [ ] `use-functional-api.mdx` — 使用 Functional API
- [ ] `interrupts.mdx` — Interrupt / 人在回路
- [ ] `streaming.mdx` — Streaming
- [ ] `checkpointers.mdx` — Checkpointer
- [ ] `stores.mdx` — Store / 长期记忆
- [ ] `add-memory.mdx` — Memory
- [ ] `use-subgraphs.mdx` — Subgraph
- [ ] `fault-tolerance.mdx` — 容错

其余教程、部署、Studio、错误参考等页面将在核心学习链路完成后继续翻译。

## 上游与版权

原始文档来自 [langchain-ai/docs](https://github.com/langchain-ai/docs)，版权归 LangChain, Inc. 及原贡献者所有。本翻译依据原仓库 MIT License 进行再分发与修改，并保留原许可证要求。

## 同步策略

后续通过 upstream diff 跟踪官方文档变更：

```bash
git remote add upstream https://github.com/langchain-ai/docs.git
git fetch upstream
git diff <last-sync-commit>..upstream/main -- src/oss/langgraph
```

仅对新增或发生语义变更的段落做增量翻译，避免整页重新翻译造成术语漂移。
