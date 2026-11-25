# AI Engineering Portfolio

Lionel-G-yuan · 企业软件授权与智能文档审核

客户购买了软件，哪些服务应当开通？模型读出了一个数值，审核员凭什么采用它？这两个项目分别处理企业软件交付中的授权判断与证据核验。

| 项目 | 代表场景 | 已实现的能力 |
| --- | --- | --- |
| [Project 02｜中央授权管理平台](02-central-licensing.md) | 客户单独续订 AI 服务 | 按客户、实例和服务判断权益，追踪续费、暂停与恢复 |
| [Project 01｜企业级 AI 证书审核系统](01-certificate-audit.md) | 扫描证书中的测量单位难以辨认 | 定位字段原文、发起人工复核，并用修正后的输入重新计算 |

两篇案例均附流程图与虚构示例，分别展示授权平台的本地验证范围，以及审核系统从证书上传到报告归档的处理过程。

## English overview

**[Project 02 · Centralized software licensing](02-central-licensing.md)** translates contracts into per-service access decisions for individual customer installations. The case study walks through a renewal affecting one customer and one service, with local regression coverage for isolation and repeated requests.

**[Project 01 · AI-assisted calibration certificate auditing](01-certificate-audit.md)** combines document extraction with deterministic checks. The case study follows an ambiguous measurement unit from OCR through human review to a versioned report.
