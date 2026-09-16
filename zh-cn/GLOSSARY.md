# LangGraph 中文术语表

本术语表用于保证中文文档在不同章节之间保持一致。遇到 API、类名、方法名和框架专有名词时，优先保留英文原名。

| English | 中文建议 | 说明 |
|---|---|---|
| agent | 智能体 | 首次出现时可写“智能体（Agent）” |
| agentic | 智能体驱动的 / Agentic | 视语境选择；作为领域术语时可保留 Agentic |
| orchestration | 编排 | 指控制流、状态和执行生命周期的编排 |
| runtime | 运行时 | 例如 Agent runtime → 智能体运行时 |
| state | 状态 | 指 Graph 在执行过程中的共享状态 |
| stateful | 有状态的 | |
| stateless | 无状态的 | |
| node | 节点 | Graph 中执行具体逻辑的单元 |
| edge | 边 | Graph 中节点之间的连接 |
| conditional edge | 条件边 | 基于状态或返回值决定路由 |
| graph | 图 | |
| subgraph | 子图 | |
| workflow | 工作流 | |
| deterministic | 确定性的 | 常用于“确定性步骤” |
| durable execution | 持久化执行 | 强调执行可恢复、可继续 |
| persistence | 持久化 | |
| checkpoint | 检查点 | 保存某一时刻 Graph state 的快照 |
| checkpointer | Checkpointer | 保留 API 术语；首次出现时解释为“检查点存储组件” |
| interrupt | 中断 | 指暂停 Graph 等待外部输入 |
| resume | 恢复执行 | |
| replay | 重放 | |
| human-in-the-loop | 人在回路 | 可简称 HITL |
| streaming | 流式输出 / 流式传输 | 视语境而定 |
| memory | 记忆 | |
| short-term memory | 短期记忆 | |
| long-term memory | 长期记忆 | |
| store | Store / 存储 | API 名保留 `Store`，概念描述可写“存储” |
| reducer | Reducer / 归约器 | API 语境保留英文，概念解释可写“归约器” |
| message | 消息 | |
| tool | 工具 | |
| tool call | 工具调用 | |
| tool calling | 工具调用 | |
| thread | 线程 | LangGraph 中常指一条持久化执行会话 |
| superstep | 超步 | Pregel 术语 |
| routing | 路由 | |
| branch | 分支 | |
| fan-out | 扇出 | 一对多并行执行 |
| fan-in | 汇聚 | 多路结果汇合 |
| retry | 重试 | |
| fault tolerance | 容错 | |
| observability | 可观测性 | |
| tracing | 追踪 | |
| trace | Trace / 追踪记录 | 产品界面或专有概念可保留 Trace |
| deployment | 部署 | |
| production-ready | 生产就绪 | |
| harness | Harness / 智能体脚手架 | 在 Agent 语境中建议首次解释后保留 Harness |
| prebuilt | 预构建 | |
| invocation | 调用 | |
| invoke | 调用 | 方法名 `invoke()` 不翻译 |
| async | 异步 | |
| sync | 同步 | |
| context | 上下文 | |
| context management | 上下文管理 | |
| context window | 上下文窗口 | |
| evaluation | 评测 | 在 LLM/Agent 语境中优先用“评测”而非“评价” |
