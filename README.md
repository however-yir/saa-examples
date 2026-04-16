# Spring AI Alibaba Examples

> Spring AI Alibaba Repo: https://github.com/alibaba/spring-ai-alibaba
>
> Spring AI Alibaba Website:  https://java2ai.com
>
> Spring AI Alibaba Website Repo: https://github.com/springaialibaba/spring-ai-alibaba-website

[English](./README-en.md) | 中文

## 介绍

此仓库中包含许多 Example 模块项目来介绍 Spring AI 和 Spring AI Alibaba 从基础到高级的各种用法和 AI 项目的最佳实践。

更详细的介绍请参阅每个子项目中的 README.md 和 [Spring AI Alibaba 官网](https://java2ai.com)。

## 参与建设

欢迎任何形式的代码贡献。

## Quickstart Matrix (Community Contribution)

| module | purpose | command | required services | env vars | env template | entry |
|---|---|---|---|---|---|---|
| spring-ai-alibaba-helloworld | basic chat and advisor examples | `mvn -pl spring-ai-alibaba-helloworld spring-boot:run` | none | `AI_DASHSCOPE_API_KEY` | — | [README](./spring-ai-alibaba-helloworld/README.md) |
| spring-ai-alibaba-chat-example/dashscope-chat | DashScope chat basics | `mvn -pl spring-ai-alibaba-chat-example/dashscope-chat spring-boot:run` | none | `AI_DASHSCOPE_API_KEY` | — | [README](./spring-ai-alibaba-chat-example/dashscope-chat/README.md) |
| spring-ai-alibaba-image-example/dashscope-image | DashScope image generation | `mvn -pl spring-ai-alibaba-image-example/dashscope-image spring-boot:run` | none | `AI_DASHSCOPE_API_KEY` | — | [README](./spring-ai-alibaba-image-example/dashscope-image/README.md) |
| spring-ai-alibaba-mcp-example | MCP demo | `mvn -pl spring-ai-alibaba-mcp-example spring-boot:run` | none/local mcp tool | model api key | [`.env.example`](./spring-ai-alibaba-mcp-example/.env.example) | [README](./spring-ai-alibaba-mcp-example/README.md) |
| spring-ai-alibaba-rag-example | RAG demo | `mvn -pl spring-ai-alibaba-rag-example spring-boot:run` | vector db (optional by profile) | model api key, embedding model | [`.env.example`](./spring-ai-alibaba-rag-example/.env.example) | [README](./spring-ai-alibaba-rag-example/README.md) |
| spring-ai-alibaba-tool-calling-example | tool calling | `mvn -pl spring-ai-alibaba-tool-calling-example spring-boot:run` | none | model api key, map api key | [`.env.example`](./spring-ai-alibaba-tool-calling-example/.env.example) | [README](./spring-ai-alibaba-tool-calling-example/README.md) |
