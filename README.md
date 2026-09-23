# re-search

> Research = re + search. 让搜索配得上"研究"这个词。

多智能体 Agentic RAG：把问题拆解给多个 Agent 并行检索、交叉验证，输出带出处的答案。

**为什么做这个项目**：朴素 RAG 只搜一次。当问题需要综合多篇文档、比较多方结论时，它抓几个碎片就开始生成——错得很自信。Research 的构词本来就是 re + search（反复搜索），这个项目要让 RAG 真正做到这一点。

## Roadmap

- [x] W0 仓库初始化
- [ ] W1 朴素 RAG 端到端跑通：入库 → 检索 → 生成 → 流式问答 Demo，同步积累测试集与 badcase
- [ ] W2 检索链路优化：专业解析器、BM25 混合检索、Rerank
- [ ] W3 多轮对话与上下文工程：查询改写、父子块
- [ ] W4 评估体系：ragas 量化对比 Agentic vs Naive，产出对比数据
- [ ] W5 多 Agent DAG 并行编排落地
- [ ] W6 工程化收尾：压测、安全、部署

## Tech Stack

Java 17 · Spring Boot 3 · Spring AI Alibaba · PGVector · Redis · Docker

> Six-week build in progress. First runnable demo lands at v0.1 (end of W1).
