# Agent Spec

目前行业里的 Agent 配置方式还比较分散，大多是在一个 `.md` 文件里简单配置一些 prompt、MCP、skill 等内容，整体比较轻量，但缺少统一的工程化规范。

我们可以参考 **npm / Maven** 的模式，将 Agent 抽象成一个可发布、可复用、可依赖管理的 **package**，并发布到统一的 **Agent Registry** 上。

## Agent Package 包含内容

一个 Agent Package 可以包含以下模块：

- **Prompt**：Agent 的角色设定、行为约束、任务目标等
- **MCP**：Agent 可连接和调用的外部工具、数据源与服务
- **Skills**：可复用的能力模块，例如代码生成、数据分析、文档处理等
- **Memory**：长期记忆、用户偏好、上下文沉淀机制
- **Knowledge Base**：领域知识库、文档索引、RAG 数据源等
- **Plugin**：用于扩展运行时能力和预览能力  
  例如集成 App 模拟器、调用内部系统的各种功能、自动提交日报等
- **Pipeline**：支持多 Agent 协作与复杂工作流编排  
  类似 npm / Maven 中的依赖关系，可声明、复用和组合其他 Agent Package

## 配套基础设施

围绕 Agent Package，可以建设一套完整的生态基础设施：

### Agent Registry

用于发布、发现、安装和管理 Agent Package，类似 npm registry 或 Maven central。

能力包括：

- Agent 包发布
- 版本管理
- 依赖解析
- 权限与可见性管理
- 质量评分与安全审查
- 企业私有 Registry

### Agent Runtime SDK

用于标准化 Agent Package 的执行方式，收敛工程实现。

它可以提供：

- Agent 包加载与解析
- Prompt / MCP / Skill / Plugin 初始化
- Pipeline 编排执行
- 运行时上下文管理
- 日志、监控与调试能力
- 本地与云端一致的运行接口

### Agent Service

基于 Agent Package 快速生成 Web Service，类似 FaaS 的模式。

开发者可以将一个 Agent Package 直接部署为服务，并获得：

- HTTP / RPC API
- 鉴权与限流
- 弹性伸缩
- 运行时隔离
- 日志与调用链追踪
- 多租户支持

## 多端交付形态

同一个 Agent Package 可以在多个场景中复用，并提供不同的交付方式：

- **CLI**：面向开发者和自动化脚本
- **Desktop**：面向本地工作流、系统集成和个人助理场景
- **Web UI**：面向普通用户和业务操作台
- **Web Service**：面向系统集成、API 调用和企业服务化

通过统一的 Agent Package Spec，一个 Agent 可以实现一次定义、多端运行、统一发布、持续演进。

## 核心价值

这套规范的核心目标是让 Agent 从「零散配置」走向「工程化资产」。

它可以带来：

- **标准化**：统一 Agent 的定义、发布、安装与运行方式
- **复用性**：Prompt、Skill、MCP、Plugin、Pipeline 都可以模块化复用
- **可组合性**：支持 Agent 之间像依赖包一样组合与编排
- **可治理性**：支持版本、安全、权限、审计和企业级管理
- **跨平台**：同一个 Agent Package 可运行在 CLI、Desktop、Web 和 Service 端
- **生态化**：通过 Registry 形成 Agent 能力市场和开发者生态

一句话概括：

> 将 Agent 从一个简单的配置文件，升级为可发布、可复用、可组合、可治理的工程化 Package。

## 交付

参考GoogleCloud开源的Open Knowledge Format (OKF)，参见https://github.com/GoogleCloudPlatform/knowledge-catalog/tree/main/okf

在github上提供类似的规范产物

- SPEC.md
- src/reference_agent
- samples
- bundles
- tests

## 参考

- https://github.com/A3S-Lab/a3s
- https://github.com/TencentEdgeOne/deepagents-research-nodejs
- https://dimagent.com/
- https://raven.evermind.ai/
- https://docs.agno.com/agent-os/introduction
- https://github.com/rivet-dev/agentos
- https://github.com/genkit-ai/genkit
