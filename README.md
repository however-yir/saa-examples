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

| module | purpose | command | required services | env vars |
|---|---|---|---|---|
| spring-ai-alibaba-mcp-example | MCP demo | `mvn -pl spring-ai-alibaba-mcp-example spring-boot:run` | none/local mcp tool | model api key |
| spring-ai-alibaba-rag-example | RAG demo | `mvn -pl spring-ai-alibaba-rag-example spring-boot:run` | vector db (optional by profile) | model api key, embedding model |
| spring-ai-alibaba-tool-calling-example | tool calling | `mvn -pl spring-ai-alibaba-tool-calling-example spring-boot:run` | none | model api key |

## 常见启动问题 / Troubleshooting

- `AI_DASHSCOPE_API_KEY` 未设置 / Missing `AI_DASHSCOPE_API_KEY`: 先确认环境变量已在当前 shell 或 IDE 中生效，再重新启动示例。
- 端口被占用 / Port already in use: 检查对应模块 `application.yml` 中的 `server.port`，释放端口或改端口后重试。
- 本地依赖未启动 / Required local services not running: RAG、MCP、向量库或 Docker 相关示例通常需要先启动对应的中间件或容器。
- 模块里暂时没有 `.env.example` / No `.env.example` in a module yet: 优先查看该模块 README 和 `src/main/resources/application.yml`，确认真实的变量名和依赖服务。
