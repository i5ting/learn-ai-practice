# learn-ai

狼叔的ai自留地

![alt text](image-1.png)

## 杰文斯悖论

杰文斯悖论（Jevons Paradox）是由19世纪英国经济学家威廉·斯坦利·杰文斯（William Stanley Jevons）在1865年提出的经济学理论。它指出：当技术进步提高了某种资源的使用效率，从而减少了单位产出所需的资源量时，该资源的总消耗量不但不会下降，反而可能会增加。

狼叔以为的ai未来趋势

- 1、粘合剂，比如agentteams没有pipeline有用
- 2、基于自身做深挖，比如自己解析figma，非包皮
- 3、基于agent上下文做创新，更实时，干掉jira
- 4、学习multica、raft.build、wizme等新产品思路，融资甚好
- 5、技术上，参考docker设计agentfile，参考npm设计agent包，有机会

职业是进化，而非消失。AI会改变人才结构，但需求增加也是事实。

## 为什么有了ai越来越累？

- 1、有参考的，ai实现太方便，尤其对有经验但动手不足的。
- 2、要学东西太多，从工具到ralph loop到工作流，还有各种周边，还不算memory、ctx等
- 3、要看各种创新，比如jira替代，agent如何协作等
- 4、面对未知，要么等死，要么找死，折腾找死可能延长职业寿命

无论那种，都会很累

## 概念

大语言模型从 Scaling（规模扩展） 到 Reasoning（推理能力） 再到 Agentic（智能体化） 的三阶段演进：Scaling 通过参数、数据和算力扩张建立知识底座；Reasoning 借助后训练、链式思维和强化学习提升逻辑推导能力；Agentic 则进一步强调模型与工具、环境和反馈系统交互，形成“感知—行动—反馈—调整”的闭环，以完成真实世界中的复杂长期任务。

- ReAct
- Agent Loop
- Function calling (or tool calling) 
- skills 参考https://github.com/jimliu/baoyu-skills
- mcp
- agent or stateful agent
- harness engineering
- loop engineering
- autoresearch https://github.com/karpathy/autoresearch
- LLM Wiki https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f
- ralph loop https://github.com/snarktank/ralph

## 常用工具


tools

- https://github.com/wxtsky/CodeIsland
- https://github.com/farion1231/cc-switch
- Obsidian 或 Tolaria，对ai支持都不错
- Clash Verge — 你懂的，尤其是虚拟网卡，对google系友好

终端

- https://github.com/ghostty-org/ghostty
- https://otty.sh/
- https://github.com/warpdotdev/warp

cli & desktop

- https://openai.com/zh-Hans-CN/index/introducing-the-codex-app/
- https://github.com/anomalyco/opencode
- https://claude.com/product/claude-code

桌面端推荐方案，参考otty
tauri + https://github.com/longbridge/gpui-component

![alt text](image.png)

## 常用库

- https://github.com/tobi/qmd
- https://github.com/dmtrKovalenko/fff
- https://github.com/VectifyAI/PageIndex
- https://github.com/tursodatabase/agentfs
- https://github.com/StarTrail-org/PixelRAG
- https://github.com/nashsu/llm_wiki
- https://github.com/gastownhall/beads
- https://github.com/millionco/spawn-agent
- https://github.com/entireio/cli
- https://github.com/sourcegraph/zoekt
- https://github.com/swe-bench/SWE-bench
- https://github.com/EverMind-AI/EverOS


## 龙虾及变体

- https://github.com/openclaw/openclaw
- https://github.com/nanocoai/nanoclaw
- https://github.com/riba2534/happyclaw
- https://github.com/nousresearch/hermes-agent

变体实在是太多，nanoclaw和happyclaw还不错。

我不喜欢龙虾（包括hermes），给的权限小了没用，大了浪费token。

## workflow 

- https://github.com/obra/Superpowers
- https://github.com/garrytan/gstack
- https://pi.dev/

额外小灶

- https://github.com/affaan-m/ecc
- 掌握 /goal 和 ralph loop

## sandbox

- https://github.com/xicilion/boxsh
- https://github.com/vm0-ai/vm0
- https://github.com/servo/gaol
- https://github.com/ErickJ3/sandbox-rs
- https://github.com/deeplethe/forkd
- https://github.com/zerobootdev/zeroboot
- https://github.com/mistlehq/mistle
- 腾讯 https://github.com/tencentcloud/CubeSandbox
- 字节 https://github.com/bytedance/sandboxfusion
- 阿里 https://github.com/opensandbox-group/OpenSandbox

## cli

- https://github.com/HKUDS/CLI-Anything
- https://github.com/jackwener/opencli
- https://github.com/nashsu/AutoCLI
- https://github.com/epiral/bb-browser

## compute-use


- https://github.com/trycua/cua
- https://github.com/bytedance/ui-tars-desktop

## agent

- https://docs.letta.com/guides/core-concepts/stateful-agents
- https://github.com/jackwener/maka-agent
- Open-source AI Agent Monitoring https://github.com/latitude-dev/latitude-llm
- trace + eval  https://github.com/evotai/evot
- agent spec https://github.com/agentpm-dev/cli/blob/main/specs/2026-05-11-agents-as-first-class-citizens/spec.md 一般，但可借鉴。

## pipeline

- https://github.com/blueberrycongee/termcanvas/tree/main/hydra

## agent runtime

- https://docs.agno.com/

## 知识库

- https://github.com/GoogleCloudPlatform/knowledge-catalog
- https://pandawiki.docs.baizhi.cloud/
- https://github.com/hilash/cabinet
- https://github.com/safishamsi/graphify
- https://github.com/colbymchenry/codegraph


## 应用

- 闭源：https://raft.build/
- 开源：https://multica.ai/
- https://github.com/paperclipai/paperclip
- https://wisme.ai/

agent 的尽头是im

- https://bloome.im/
- https://cumora.ai/
- https://shandianshuo.cn/

这几个都不错，但是他们的先手优势只有半年，钉钉、飞书等如果跟进，对他们来说是很危险的。

## 文章

- 聊一聊 Agent 的存算分离架构设计 https://x.com/idoubicc/status/2061670587043610688
- Agent 沙箱 Claude Code Cursor OpenClaw标配能力一文讲清楚 https://mp.weixin.qq.com/s/-FSThb-jyX5zdMcYlfl1HQ
- learn-claude-code-js https://github.com/i5ting/learn-claude-code-js/
- Agent Skills 设计哲学和实战进化 https://x.com/dotey/status/2036114136245969025