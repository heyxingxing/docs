# LangGraph 中文术语表

本术语表用于保证中文文档在不同章节之间保持一致。遇到 API、类名、方法名和框架专有名词时，优先保留英文原名。

| English | 中文建议 | 说明 |
|---|---|---|
| agent | 智能体 | 首次出现时可写“智能体（Agent）” |
| agentic | 智能体驱动的 / Agentic | 视语境选择；作为领域术语时可保留 Agentic |
| orchestration | 编排 | 指控制流、状态和执行生命周期的编排 |
| runtime | 运行时 | 例如 Agent runtime → 智能体运行时 |
| state | 状态 / State | 概念说明用“状态”，涉及 LangGraph 数据对象时可保留 State |
| stateful | 有状态的 | |
| stateless | 无状态的 | |
| State Schema | State Schema / 状态模式 | API 与代码语境保留 `StateSchema` |
| node | 节点 / Node | 概念说明用“节点”，强调 LangGraph 抽象时可保留 Node |
| edge | 边 / Edge | 概念说明用“边”，强调 LangGraph 抽象时可保留 Edge |
| conditional edge | 条件边 | 基于状态或返回值决定路由 |
| graph | 图 / Graph | |
| subgraph | 子图 / Subgraph | |
| workflow | 工作流 | |
| deterministic | 确定性的 | 常用于“确定性步骤” |
| determinism | 确定性 | |
| non-deterministic | 非确定性的 | |
| idempotent | 幂等的 | |
| idempotency | 幂等性 | |
| side effect | 副作用 | 例如写文件、发送邮件、外部 API 写操作 |
| serialization | 序列化 | |
| durable execution | 持久化执行 | 强调执行可恢复、可继续 |
| persistence | 持久化 | |
| checkpoint | 检查点 / Checkpoint | 保存某一时刻 Graph State 的快照；技术语境常保留 Checkpoint |
| checkpointing | Checkpointing / 检查点持久化 | 描述机制时可保留英文 |
| checkpointer | Checkpointer | 保留 API 术语；首次出现时解释为“检查点存储组件” |
| interrupt | 中断 / Interrupt | 方法名 `interrupt()` 不翻译 |
| resume | 恢复执行 | `resume` 参数名保持英文 |
| replay | 重放 / Replay | 描述恢复语义时可首次写“重放（Replay）” |
| human-in-the-loop | 人在回路 | 可简称 HITL |
| streaming | 流式输出 / Streaming | API 能力名称可保留 Streaming |
| memory | 记忆 | |
| short-term memory | 短期记忆 | |
| long-term memory | 长期记忆 | |
| store | Store / 存储 | API 名保留 `Store`，概念描述可写“存储” |
| reducer | Reducer / 归约器 | API 语境保留英文，概念解释可写“归约器” |
| entrypoint | Entrypoint | Functional API 核心抽象；API 名 `entrypoint` 不翻译 |
| task | Task / 任务 | Functional API 核心抽象；API 名 `task` 不翻译 |
| future | Future | 异步结果占位对象，通常保留英文 |
| command | Command | LangGraph 路由与状态更新原语；API 名不翻译 |
| message | 消息 | |
| tool | 工具 | |
| tool call | 工具调用 | |
| tool calling | 工具调用 | |
| thread | 线程 / Thread | LangGraph 中常指一条持久化执行会话 |
| thread id | Thread ID | 配置键 `thread_id` 保持原样 |
| superstep | 超步 / Superstep | Pregel 术语 |
| routing | 路由 | |
| branch | 分支 | |
| fan-out | 扇出 | 一对多并行执行 |
| fan-in | 汇聚 | 多路结果汇合 |
| retry | 重试 | |
| Retry Policy | Retry Policy / 重试策略 | API 名和配置概念常保留英文 |
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
