# AI News Factory 三条核心主线

## 1. Shared State

Shared State 是单条新闻在一次 Workflow 运行过程中的统一状态模型。

主要状态：

1. initialized
2. raw_collected
3. normalized
4. scored
5. selected
6. drafted
7. quality_reviewed
8. fact_checked
9. safety_reviewed
10. formatted
11. published
12. rejected
13. failed

运行位置：Dify Workflow

定义位置：GitHub schemas 目录

当前实现方式：通过 Dify 节点输出变量和节点间变量引用实现。

---

## 2. Database Flow

Database Flow 定义关键业务数据未来如何被持久化。

当前数据库状态：未启用。

目前只在 GitHub 中维护：

- 存储节点
- 数据实体
- 字段结构
- 数据关联
- 接入优先级

未来数据库接入后，由 Dify 通过 HTTP Request 调用数据库接口。

---

## 3. Quality Standard

Quality Standard 定义每个关键阶段进入下一阶段前必须满足的条件。

主要质量门禁：

1. 原始数据有效性
2. 清洗质量
3. 新闻价值
4. 文章质量
5. 事实一致性
6. 安全合规
7. 发布格式

规则定义位置：GitHub quality_rules 目录

执行位置：Dify Workflow

执行方式：

- 确定性规则：Code、If
- 语义性判断：LLM
- 流程控制：If/Else
- 不通过修订：Loop
