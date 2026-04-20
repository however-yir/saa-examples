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

## Baseline Maintenance

### Environment

- Put runtime credentials in environment variables.
- Use `.env.example` as the configuration template.

### CI

- `baseline-ci.yml` provides a unified pipeline with `lint + build + test + secret scan`.

### Repo Hygiene

- Keep generated files (`dist/`, `build/`, `__pycache__/`, `.idea/`, `.DS_Store`) out of version control.

## Audit Baseline Notes

### Requirements

- Environment requirements are defined by this module and parent project documentation.
- Configure credentials via environment variables before startup.
- Use `.env.example` (or equivalent sample config) for local setup.

### Run

- Install dependencies for this module before execution.
- Use the standard project command to build and run (for example Maven, Gradle, npm, or Python entrypoint scripts in this repository).
