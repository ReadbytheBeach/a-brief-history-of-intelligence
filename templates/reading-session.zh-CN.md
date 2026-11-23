# Session NN · <本次主题>

> 模板占位稿：复制到 `sessions/` 后填写，不把此模板注册进索引。
> 主题：<已读章节、用户问题与本次讨论范围>
> 内容日期：<原文明示的讨论或存档日期；未知注明未知>
> 日期类型：<discussion / archive>
> 资料核查/证据截止日：<仅明确核查时填写，否则未知>

## 阅读材料与问题

- 已读范围：<章节、页码或原始材料；不预告后续未读内容>
- 核心问题：<本次要回答的问题>
- 批注或用户前提：<保留原话归属及条件>

## 原书观点与讨论

<按内容组织正文。区分原作者报告、作者假说、读书会推断、用户前提与待验证建议；引用要保留位置与上下文。>

## 限定与开放问题

<注明哪些是未验证解释或类比、哪些资料未取得；延续讨论和补档日期另列。不以存档日代替证据核查日。>

## 来源

<列出本次实际阅读的书页与原始资料。未读资料不要写成已核验来源。>

## 登记与生成（完成后移除此节）

1. 在 `content-index.json` 追加下一个未使用的 `ABHI-NNN`，令 `document_id` 与 `session_id` 同值，保留正文 H1 和最终路径。
2. 填写英文检索标题、`reading_session` 类型、分类、3–6 对中英主题、核心问题、2–3 条带标签摘要、适用边界、0–3 个真实关联 ID 与日期。
3. `content_date` / `content_date_kind` 对应明确讨论或存档日；`evidence_as_of` 未明确核查则为 `null`；`indexed_on` 为索引维护日。摘要不替代正文。
4. 标签按 `AGENTS.md` 与注册表使用：`FACT`、`AUTHOR_REPORT`、`AUTHOR_HYPOTHESIS`、`DISCUSSION`、`PROPOSAL`、`LOCAL_RESULT`、`USER_CONTEXT`。书本理论和工程类比不一概标为 `FACT`。
5. 运行 `python3 scripts/build_reading_index.py` 与 `python3 scripts/build_reading_index.py --check`，将正文、JSON 与生成结果放在同次提交；不手写生成摘要或第二份权威索引。

回答书页问题不主动关联 MicroDuck/鸭子项目，除非用户点名；不剧透尚未读到的后续章节。
