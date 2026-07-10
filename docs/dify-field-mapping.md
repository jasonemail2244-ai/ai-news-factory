# Dify 字段映射表

版本：1.0.0

用途：核对 GitHub Schema 与 Dify Workflow 节点实际输出字段是否一致。

---

## 1. 数据清洗 / 文章标准化

对应 Schema：

schemas/normalized_news.schema.json

| 标准字段 | Dify 当前字段 | 数据类型 | 是否一致 | 处理建议 |
|---|---|---|---|---|
| title | 待填写 | string | 待检查 | |
| summary | 待填写 | string | 待检查 | |
| url | 待填写 | string | 待检查 | |
| source | 待填写 | string | 待检查 | |
| category | 待填写 | string | 待检查 | |
| region | 待填写 | string | 待检查 | |
| language | 待填写 | string | 待检查 | |
| pub_time | 待填写 | string | 待检查 | |
| keywords | 待填写 | array[string] | 待检查 | |
| entities | 待填写 | array[string] | 待检查 | |
| is_valid | 待填写 | boolean | 待检查 | |
| invalid_reason | 待填写 | string | 待检查 | |

---

## 2. 新闻价值评估

对应 Schema：

schemas/value_score.schema.json

| 标准字段 | Dify 当前字段 | 数据类型 | 是否一致 | 处理建议 |
|---|---|---|---|---|
| total_score | 待填写 | number | 待检查 | |
| importance_score | 待填写 | number | 待检查 | |
| impact_score | 待填写 | number | 待检查 | |
| timeliness_score | 待填写 | number | 待检查 | |
| novelty_score | 待填写 | number | 待检查 | |
| decision | 待填写 | string | 待检查 | |
| reason | 待填写 | string | 待检查 | |
| tags | 待填写 | array[string] | 待检查 | |

---

## 3. 文章撰写

对应 Schema：

schemas/article_draft.schema.json

| 标准字段 | Dify 当前字段 | 数据类型 | 是否一致 | 处理建议 |
|---|---|---|---|---|
| article_id | 待填写 | string | 待检查 | |
| headline | 待填写 | string | 待检查 | |
| lead | 待填写 | string | 待检查 | |
| body | 待填写 | string | 待检查 | |
| background | 待填写 | string | 待检查 | |
| source_links | 待填写 | array[string] | 待检查 | |
| word_count | 待填写 | number | 待检查 | |
| version | 待填写 | number | 待检查 | |

---

## 4. 质量检查

对应 Schema：

schemas/review_result.schema.json

| 标准字段 | Dify 当前字段 | 数据类型 | 是否一致 | 处理建议 |
|---|---|---|---|---|
| review_type | 待填写 | string | 待检查 | |
| pass | 待填写 | boolean | 待检查 | |
| score | 待填写 | number | 待检查 | |
| risk_level | 待填写 | string | 待检查 | |
| hard_fail | 待填写 | boolean | 待检查 | |
| issues | 待填写 | array[object] | 待检查 | |
| revision_required | 待填写 | boolean | 待检查 | |
| revision_instruction | 待填写 | string | 待检查 | |

---

## 5. 安全审核

对应 Schema：

schemas/review_result.schema.json

| 标准字段 | Dify 当前字段 | 数据类型 | 是否一致 | 处理建议 |
|---|---|---|---|---|
| review_type | 待填写 | string | 待检查 | |
| pass | 待填写 | boolean | 待检查 | |
| score | 待填写 | number | 待检查 | |
| risk_level | 待填写 | string | 待检查 | |
| hard_fail | 待填写 | boolean | 待检查 | |
| issues | 待填写 | array[object] | 待检查 | |
| revision_required | 待填写 | boolean | 待检查 | |
| revision_instruction | 待填写 | string | 待检查 | |

---

## 6. 日报排版

日报排版暂不对应独立 Schema，先记录现有输出。

| Dify 当前字段 | 数据类型 | 字段用途 | 是否继续保留 |
|---|---|---|---|
| 待填写 | 待填写 | 待填写 | 待检查 |

---

## 7. 当前发现的问题

| 编号 | 节点 | 问题 | 风险 | 后续处理 |
|---|---|---|---|---|
| 1 | 待填写 | 待填写 | 待填写 | 待填写 |
