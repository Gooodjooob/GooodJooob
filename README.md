# 你好，我是 Gooodjooob

做开发出身，现在专注 FDE（Forward Deployed Engineer）方向——大模型怎么在企业里真正用起来、用稳。

我关心的问题都挺具体：Agent 干完活，怎么证明它真的干了？返工之后上一版还在不在？"提交成功"和"已执行"中间的坑怎么填？[Conductor](https://github.com/Gooodjooob/Conductor-Agent) 就是拿来啃这些的——多 Agent 协作控制面，把任务、执行、交付、审核记成一本可查的账。有个细节我一直没妥协：审核绑定具体版本，返工不覆盖历史。仓库里有 5 个案例写了当时的取舍，包括[离线测试全绿、我仍然拒绝宣布接通的那次](https://github.com/Gooodjooob/Conductor-Agent/blob/main/docs/case-studies/04-entry-gate.md)。

另外我给自己销售作业写过一套 Agent 工具链（技能路由、能力注入、发布门禁），跑在真实业务上有一阵子了，正在做脱敏整理准备开源。做那个东西最大的教训：让模型"记得调工具"不能靠嘱咐，得靠机制。

技术栈主要是 Python / SQLite / React，Agent 侧用 LangGraph、MCP 这类，RAG 全链路也搭过完整的。比起会用什么，我更在意边界感——哪里自动化，哪里留人工，哪里必须拒。

简历和详细项目资料可另附，欢迎交流。
