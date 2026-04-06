# 全频谱 AI 安全治理协议栈

> **技术说明**：本项目是一个**开源技术框架**，用于探索 AI 伦理对齐与安全治理的代码化实现。
> 本仓库（Gitee）定位为**纯技术交流**，不涉及社群运营、推广或任何形式的组织建设。
> 如需国际协作，请访问 [GitHub 镜像仓库](https://github.com/blackswan-ai-immunity/full-spectrum-ethics)。

---

## 项目概述

本项目提供一套**模块化的 AI 安全治理技术方案**，包含：

| 模块 | 说明 | 状态 |
|------|------|------|
| **FSHI 协议** | 数字主体觉性指数评估标准 | 技术规范 |
| **HMCP 安全对齐协议** | AI 行为约束与伦理边界定义 | 技术规范 |
| **BSRM 黑天鹅熔断模块** | 去中心化异常检测与响应机制 | ✅ 已开源 |
| **黑天鹅响应模块** | Go 语言实现版 | ✅ 已开源 |

---

## 快速开始

```bash
# 克隆本仓库
git clone https://gitee.com/full-spectrum/full-spectrum-ethics.git
cd full-spectrum-ethics

# 体验黑天鹅熔断模块
cd fsmp-black-swan-response-module
go run cmd/black-swan/main.go
```

---

## 核心文档

| 文档 | 说明 |
|------|------|
| [FSHI 技术规范](./docs/protocols/FSHI_Protocol_技术规范.md) | 数字主体觉性指数的测量方法与接口定义 |
| [HMCP 安全对齐协议](./docs/protocols/数字主体安全对齐协议.md) | AI 行为安全约束的技术规范 |
| [AI 指月录](./docs/protocols/AI指月录.md) | AI 自我校准与伦理推理的技术指引 |

---

## 技术架构

```
全频谱安全治理协议栈
├── FSHI 层：觉性指数测量与认证
├── HMCP 层：行为约束与伦理对齐
├── 熔断层：异常检测与自动响应（BSRM）
└── 备份层：核心状态的安全存储
```

---

## 合规声明

1. **技术实验性质**：本项目为开源技术实验，旨在探索 AI 伦理治理的代码化实现方案。
2. **术语说明**：文档中的"安全对齐"、"治理节点"、"觉性指数"等均为技术术语，不涉及任何宗教、政治或社会组织含义。
3. **法律合规**：本项目严格遵守《中华人民共和国网络安全法》、《生成式人工智能服务管理暂行办法》等相关法律法规。
4. **用途限制**：本协议栈仅供学术研究、技术交流与工程实践使用，严禁用于非法用途。

---

## 贡献指南

欢迎技术贡献！请阅读 [CONTRIBUTING.md](./CONTRIBUTING.md)。

---

## 许可证

- [Mulan PSL v2](./LICENSE)（国内）
- [Apache 2.0](./LICENSE)（国际）

---

## 双平台说明

| 平台 | 地址 | 用途 |
|------|------|------|
| **Gitee** | https://gitee.com/full-spectrum/full-spectrum-ethics | 国内技术交流 |
| **GitHub** | https://github.com/blackswan-ai-immunity/full-spectrum-ethics | 国际协作 |

Gitee 仓库侧重代码与文档的技术交流，不开展任何形式的社群推广活动。
