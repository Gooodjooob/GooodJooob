# 你好，我是 Gooodjooob

FDE（Forward Deployed Engineer，前沿部署工程师）方向，关注**大模型企业应用落地**：Agent 工作流、RAG 检索链路、多 Agent 协作控制面。做交付出身的视角——先问"能不能跑起来、出了问题怎么查、边界在哪里"。

## 精选项目

### [Conductor](https://github.com/Gooodjooob/Conductor-Agent) · 多 Agent 开发协作控制面

把任务派发、执行、交付、审核建成**可追溯的账本**，解决多 Agent 协作里"返工覆盖历史、提交成功≠已执行"的问题。

几个我坚持的设计：

- **task / attempt 分离建模** —— 返工新建轮次，旧交付保留可查，审核绑定具体版本
- **写入契约（write contract）** —— 草稿→预览→确认→写入→回读，不信任返回的 "success"
- **unknown 是一等状态** —— 超时先对账（进程、源码、回执、数据库），再决定是否重试
- **证据分级，不外推** —— 每个数字带限定范围，手工环节如实标注

仓库里有 [5 个工程案例研究](https://github.com/Gooodjooob/Conductor-Agent/tree/main/docs/case-studies)（问题→关键动作→结果与证据→取舍→追问准备）和一份[表述边界与证据分级](https://github.com/Gooodjooob/Conductor-Agent/blob/main/docs/claims-and-boundaries.md)文档——后者是我对"怎么诚实地写工程成果"的答案。

> 该项目为进行中状态，源码快照非稳定发行版，边界与未验证项见仓库内说明。

*（筹备中：DSH 宿主适配器最小切片 · RAG 全链路可跑通 demo · 故障排查笔记）*

## 技术栈

| 领域 | 内容 |
|---|---|
| Agent 与编排 | LangGraph、MCP 工具封装、多 Agent 工作流、Function-Call 设计 |
| 检索与 RAG | 文档解析 / 分块 / Embedding / 向量检索 / 混合检索 / Rerank / 引用溯源 |
| 后端 | Python、SQLite（事件溯源、幂等与冲突处理）、Java |
| 前端与交付 | React（只读看板）、本机安装与恢复、交付验证 |

## 我在意的三件事

1. **交付可靠性** —— 可追溯、可验证；不把手工环节包装成全自动
2. **表述诚实** —— 区分「历史真实验证 / 实现可定位 / 设计与规则 / 待核」，不同模块不合成"全部上线"
3. **恢复优先** —— 失败后先回答"旧操作发生了什么"，再决定补采集还是重试

## 联系

简历与详细项目资料可另附，欢迎就 Agent 工程化、RAG 落地、交付可靠性交流。
