# AI Engineering Portfolio

Lionel-G-yuan · 企业软件授权与智能文档审核

客户购买了软件，哪些服务应当开通？模型读出了一个数值，审核员凭什么采用它？这两个项目分别处理企业软件交付中的授权判断与证据核验。

| 项目 | 代表场景 | 已实现的能力 |
| --- | --- | --- |
| [Project 02｜中央授权管理平台](02-central-licensing.md) | 客户单独续订 AI 服务 | 按客户、实例和服务判断权益，追踪续费、暂停与恢复 |
| [Project 01｜企业级 AI 证书审核系统](01-certificate-audit.md) | 陌生模板中的测量值应填入哪一列？ | 用 OCR 和 AI Extraction 提取带原文证据的候选，交由 Python 核验；用回放验证字段修复与并发优化 |

授权平台案例通过两个虚构客户展示分项续费。证书审核案例附证据校验对照图，以及两次实际修复的样本、方法和结果。

## English overview

**[Project 02 · Centralized software licensing](02-central-licensing.md)** translates contracts into per-service access decisions for individual customer installations. The case study walks through a renewal affecting one customer and one service, with local regression coverage for isolation and repeated requests.

**[Project 01 · AI-assisted calibration certificate auditing](01-certificate-audit.md)** combines document extraction with deterministic checks. The case study follows one synthetic measurement through evidence validation, then examines a parsing fix on 20 synthetic certificates and a four-task replay of signature OCR under load.
