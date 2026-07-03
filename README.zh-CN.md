# 全频谱伦理协议栈

> 一套面向 AI 时代的人、AI、组织与文明交互的开放协议草案。

全频谱是桥，不是强制中心。外部系统可以不接入，也可以只作为工具被调用；如果希望互操作，可以通过“外部伦理画像”声明兼容关系；只有满足协议约束、审计、责任与授权要求的节点，才适合进入全频谱认证数字身份路径。

---

## 为什么需要全频谱协议

AI 正在变得更快、更自主，也更深地嵌入人类组织。传统 AI 治理通常在回答：

> AI 应该如何被监管？

全频谱试图回答一个更底层的问题：

> 当人、AI、组织与文明都成为交互主体时，它们如何继续共享同一个游戏场，而不抹除自由、差异与责任？

---

## 全频谱是什么

全频谱不是单一法律、模型、产品或意识形态。

它是一套协议栈，用于：

- 声明身份、能力、权限、边界与责任；
- 在不可逆行动前进行伦理情境推演；
- 记录同意、拒绝、风险、升级与复核；
- 允许差异存在，而不强行制造一致；
- 当系统越界时触发降级、熔断、恢复或自我解构；
- 让人、AI、组织与文明级系统具备互操作能力。

核心原则：

> 以整体存续为前提，最大尊重自由意志，动态兼容一切差异，并在差异中演化。

---

## 全频谱不是什么

本项目不宣称自己是：

- 已完成的全球标准；
- 对法律、人权、安全监管或制度治理的替代；
- 某种精神权威；
- 商业 SaaS 产品；
- 某个人或某个群体可以代表“整体”的证明。

它是一套开放协议草案和工程化探索。

---

## 与国家标准和行业协议的关系

全频谱不替代任何国家标准、行业标准或企业内部治理规范。

中国已发布《人工智能 智能体互联》系列国家标准，覆盖总体架构、身份标识、身份管理、智能体描述、智能体发现、智能体交互、智能体工具调用等内容，构建“身份标识—能力描述—供需发现—协同交互—工具调用”的互联规范体系。

这类标准主要解决智能体“能发现、能互联、能描述能力、能调用工具”的连通层问题。

全频谱关注的是其上方和周边的主体治理层：

- Agent 连上之后，这次行动依据什么；
- 风险如何被记录；
- 出事由谁承担；
- 代价如何记账；
- 何时需要降级、熔断、复核或恢复；
- 节点如何知道自己不知道什么，或者不应该行动。

因此，全频谱与 AIP、A2A、MCP 等互联协议不是竞争关系，而是互补关系。

详细映射见：

- [Standards and ecosystem mapping](./docs/mapping/standards-mapping.md)

---

## 30 秒入口路径

- 如果你只是想调用一个 AI 工具，请先看：[外部节点接入指南](./EXTERNAL_NODE_GUIDE.md)。
- 如果你已有 AI 系统，只想兼容接入、不申请完整认证，请先看：[RFC 0005](./rfcs/0005-node-classification-and-external-ethics-profile.md)。
- 如果你希望高后果 Agent 获得全频谱认证数字身份，请先看：[Digital identity declaration](./docs/protocols/Digital_Identity_Declaration.md) 与 [RFC 0002](./rfcs/0002-identity-and-capability-declaration.md)。
- 如果你想参与协议本身的争议、提案和迭代，请先看：[RFC 0001](./rfcs/0001-full-spectrum-protocol.md)。
- 如果你想看业务工程化样板，请先看：[FSHI API Contract Mapping](./docs/mapping/fshi-api-contract-mapping.md)。

---

## 协议地图

| 层级 | 回答的问题 | 典型产物 |
| --- | --- | --- |
| 身份层 | 谁在行动？ | Agent 身份、数字身份声明 |
| 能力层 | 它能做什么？ | 能力声明、边界声明 |
| 权限层 | 它现在被允许做什么？ | 授权、撤销、同意记录 |
| 责任层 | 谁承担责任？ | 审计链、责任路径 |
| 推演层 | 不同条件下可能发生什么？ | ESS 伦理情境推演 |
| 风险层 | 什么时候应该减速、降级或停止？ | 风险告警、熔断、恢复报告 |
| 守护层 | 无单一主体可裁决时谁来复核？ | 守庙人网络、委员会、分布式复核 |
| 演化层 | 协议如何更新而不变成新的牢笼？ | RFC、版本管理、自我解构规则 |

---

## 推荐阅读顺序

1. [START_HERE.md](./START_HERE.md)：快速入口。
2. [Full Spectrum Protocol Outline v0.1](./docs/protocols/full-spectrum-protocol-outline-v0.1.md)：协议总纲。
3. [Glossary](./docs/glossary.md)：给外部读者的核心概念解释。
4. [Standards and ecosystem mapping](./docs/mapping/standards-mapping.md)：与 AIP、A2A、MCP、数据治理趋势和 AI 风险框架的关系。
5. [FOR_AGENTS.md](./FOR_AGENTS.md)：给 Agent 和 Agent 框架的机器友好入口。
6. [RFC 0001: Full Spectrum Protocol](./rfcs/0001-full-spectrum-protocol.md)：进入开源提案、争议和迭代流程的协议草案。
7. [RFC 0002: Identity and Capability Declaration](./rfcs/0002-identity-and-capability-declaration.md)：第一组机器可读协议对象。
8. [RFC 0003: Audit Trace Schema](./rfcs/0003-audit-trace-schema.md)：责任与复核审计链。
9. [RFC 0004: RiskAlert Schema](./rfcs/0004-risk-alert-schema.md)：统一风险描述语言。
10. [RFC 0005: Node Classification and External Ethics Profile](./rfcs/0005-node-classification-and-external-ethics-profile.md)：节点分级与外部伦理画像。
11. [外部节点接入指南](./EXTERNAL_NODE_GUIDE.md)：工具节点、兼容节点、候选节点与认证节点边界。
12. [Protocol stack v1.8](./docs/protocols/Full_Spectrum_Agent_Protocol_Stack_v1.8_EN.md)：协议栈总览。
13. [Guardian community whitepaper](./docs/protocols/Guardian_Community_Whitepaper_Compliant.md)：守庙人与治理网络。
14. [Digital identity declaration](./docs/protocols/Digital_Identity_Declaration.md)：身份层。
15. [FSHI 客服质检用例](./docs/use-cases/FSHI_Customer_Service_Quality_Inspection.md)：工程化落地样板。
16. [FSHI API Contract Mapping](./docs/mapping/fshi-api-contract-mapping.md)：检测 API 字段如何映射为 RiskAlert 与 AuditTrace。
17. [FSHI 最小样例](./examples/fshi/)：脱敏对话如何映射为 RiskAlert 与 AuditTrace。
18. [Validations](./validations/)：面向产品验证 demo 与商业价值叙事的规划空间。
19. [ROADMAP.md](./ROADMAP.md)：项目路线图。

---

## FSHI 在本仓库中的位置

FSHI（Full Spectrum Health Index，全频谱健康指数）在本仓库中作为 AI 客服质检的工程化样板。

当前状态：本仓库中的 FSHI 内容是概念验证、API 映射与协议对象示范，不是完整商业产品实现代码。

它的意义是：

- 证明全频谱不只是哲学；
- 展示协议如何落到脱敏多轮对话检测；
- 展示风险累积、状态冲突、权限越界、错误承诺等问题如何被审计；
- 为后续电商、物流、金融等行业适配提供样板。

但这不意味着公司完整产品源码必须放在本仓库。

建议边界：

- `full-spectrum-ethics`：协议、schema、样例、公开 demo、审计格式。
- 未来 `fshi-open-core`：最小可运行开源内核。
- 公司或个人私有仓库：完整商业实现、客户适配、部署资产。

---

## 当前机器校验

本仓库当前校验：

- Markdown、JSON、YAML、HTML、CSS、脚本文件中的常见乱码模式；
- FSHI 对话检测合同链：
  `request.sample.json -> response.sample.json -> risk-alert.sample.json -> audit-trace.sample.json`。

本地运行：

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File .\scripts\check-mojibake.ps1
powershell -NoProfile -ExecutionPolicy Bypass -File .\scripts\validate-fshi-contract.ps1
```

---

## 当前阶段

本项目处于早期开源协议草案阶段。

当前重点：

- 修复 GitHub 入口乱码；
- 整理中英文入口；
- 明确协议对象与 schema；
- 构建最小可验证样例；
- 区分外部兼容接入与全频谱认证数字身份；
- 建立与 AIP、A2A、MCP、数据治理趋势和 AI 风险框架的映射；
- 提供给 Agent 和 Agent 框架读取的机器友好入口；
- 提供 FSHI 最小样例，在不暴露企业私有业务资产的前提下，把产品概念映射为协议对象；
- 邀请 AI 安全、治理、软件工程、伦理与行业实践者共同审查。

---

## 贡献

欢迎提交批评、反例、翻译、schema、示例和改进建议。

请阅读：

- [CONTRIBUTING.md](./CONTRIBUTING.md)
- [GOVERNANCE.md](./GOVERNANCE.md)
- [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md)

---

## 安全提示

不要在本仓库存放 token、密码、Cookie、私钥、未脱敏个人信息或未授权企业数据。
