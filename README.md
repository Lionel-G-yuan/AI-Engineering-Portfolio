# AI Engineering Portfolio

Lionel-G-yuan · 企业软件授权与智能文档审核

客户购买了软件，哪些服务应当开通？模型读出了一个数值，审核员凭什么采用它？这两个项目分别处理企业软件交付中的授权判断与证据核验。

| 项目 | 代表场景 | 已实现的能力 |
| --- | --- | --- |
| [Project 02｜中央授权管理平台](02-central-licensing.md) | 客户单独续订 AI 服务 | 按客户、实例和服务判断权益，追踪续费、暂停与恢复 |
| [Project 01｜企业级 AI 证书审核系统](01-certificate-audit.md) | 陌生模板中的测量值应填入哪一列？ | 用 OCR 和 AI Extraction 提取带原文证据的候选，交由 Python 核验；用回放验证字段修复与并发优化 |

授权平台案例通过两个虚构客户展示分项续费。证书审核案例从上传、识别、能力匹配一直画到复核与报告归档，再用一条合成测量记录展示候选值如何通过原文校验。[查看证书审核流程图](01-certificate-audit.md#证书审核流程)

**从项目中学到的系统设计。** 我把 OCR 的任务并发数和每个进程的推理线程数分开测量，用同一组任务比较耗时、CPU 占用和复核结果。梳理部署时，我也按 Web 服务、Python 工作进程和主机软件包追踪依赖来源，整理了一套升级前的核查方法。[阅读运行环境与依赖核验](01-certificate-audit.md#从运行环境到依赖核验)

## English overview

**[Project 02 · Centralized software licensing](02-central-licensing.md)** translates contracts into per-service access decisions for individual customer installations. The case study walks through a renewal affecting one customer and one service, with local regression coverage for isolation and repeated requests.

**[Project 01 · AI Certificate Review System](projects/ai-certificate-review-system/README.md)** combines PDF parsing, OCR and evidence-grounded field extraction with deterministic checks and human review. The case study covers a parsing fix verified on 20 synthetic certificates, a four-task signature OCR benchmark, and my contribution to enterprise IT security assessment and remediation planning.
