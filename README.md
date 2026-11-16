# 你好，我是王奕灵 👋

**AI Agent 开发方向｜大模型应用开发｜后端工程**

哈尔滨工业大学（深圳）计算机科学与技术专业本科在读（2024—2028）。我关注能够调用工具、检索知识、管理多轮状态并可靠完成业务任务的 AI Agent。目前主要实践方向是 Agent 工作流编排、RAG、模型微调和大模型应用后端开发。

## 重点项目

### 电商智能客服 AI Agent

*2026.10—2026.11｜Python · LangGraph · LangChain · RAG · FastAPI · PostgreSQL · Redis*

面向订单、物流、商品和售后等多步骤咨询，开发具备工具调用、知识检索和多轮上下文管理能力的客服 Agent。

- **双 LLM 分工：** 将工具规划与证据收集、基于证据的答复生成分开，分别处理流程控制和用户回复。
- **工具执行与证据管理：** 接入订单、物流、商品和售后查询；通过 Evidence Gate 与证据版本管理，避免切换订单或商品后复用过期结果。
- **RAG 检索：** 为平台规则和商品说明书设计独立检索流程，并结合商品与 SKU 上下文约束检索范围。
- **状态持久化与并发控制：** 使用 LangGraph PostgreSQL checkpoint、Redis 锁和 PostgreSQL 单写入者协调，支持会话恢复及一致的状态更新。
- **验证：** 在隔离的模拟业务数据环境中，使用真实 LLM 完成涵盖订单发货、预计送达时间和商品信息的三轮对话测试。

### Qwen-VL 皮肤病灶分类微调

*AI 算法工程实习｜2026.01—2026.03｜PyTorch · Qwen-VL-8B · LoRA*

基于 PAD-UFES 数据集，对视觉语言模型进行六分类皮肤病灶识别微调。

- 通过动态过采样与图像增强缓解类别不平衡，将 SCC 类别 F1 从 **0.35 提升至 0.46**。
- 调整 LoRA 配置和训练策略，结合冻结视觉塔与提前停止减轻过拟合。
- 测试集取得 **86.5% Accuracy** 和 **0.87 Macro F1**。
- 引入额外 ISIC 数据，改善少数类别识别，并减少 SCC 与 BCC 的混淆。

### 电商评论分析与商品评价

*2025.10—2025.11｜Python · Selenium · Pandas · Qwen1.5 · 监督微调*

- 使用 Selenium 采集动态加载的电商评论，并清洗评论文本、用户信息和评分数据。
- 通过模型辅助翻译构建中文评论数据集。
- 对 Qwen1.5 进行监督微调，用于虚假评论识别与商品评价。

## 技术能力

| 方向 | 技术 |
| --- | --- |
| Agent 与大模型 | LangGraph、LangChain、工具调用、RAG、LLM 微调 |
| 机器学习 | PyTorch、Scikit-learn、Transformers、深度学习 |
| 后端开发 | Python、FastAPI、SQLAlchemy、RESTful API |
| 数据与状态 | PostgreSQL、Redis、SQL、LangGraph Checkpointing |
| 开发工具 | Git、Docker、Slurm、阿里云 |
| 编程语言 | Python、C、SQL |

## 联系我

- GitHub：[wyl250130](https://github.com/wyl250130)
- 邮箱：180993109@qq.com

期待参与 AI Agent 开发与大模型应用工程相关的项目和实践。
