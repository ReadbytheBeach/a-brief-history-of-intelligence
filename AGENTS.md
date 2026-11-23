# 智能简史阅读与维护约定

本仓库保存 Max Bennett《智能简史》的中文读书会笔记。格式参考 `ReadbytheBeach/robot-rsi-research`，使用双语导航支持人类与模型按需阅读。

## 按需阅读与归属

1. 先读根目录 `README.md`，确认读书会方法和用户约定。
2. 读取权威导航元数据 `content-index.json`，按 `question_zh`、双语主题、分类和摘要选择相关篇目。
3. 再读所选笔记的入口摘要、`scope_zh` 与原正文；依赖具体主张前回到其原始上下文和来源。摘要不替代原文。
4. `related_ids` 仅表示主题相关，不证明因果、依赖或实验可比性。

回答书页问题时不主动关联 MicroDuck/鸭子项目，除非用户点名；不剧透用户尚未读到的后续章节。原文包含约定提出前的讨论，不能因此改写历史记录。

Use the README and registry to select a small relevant set of sessions. Read the original conditions and attribution before relying on a summary. Respect the no-spoiler and user-requested project-linking rules.

## 稳定 ID 与日期

- `document_id` 为稳定的 `ABHI-NNN`；`session_id` 与其同值。新增主题追加下一个未使用编号；保留已有 ID、原 H1 与路径，不因顺序或分类变化重新编号。
- `content_date` / `content_date_kind` 只记录原文明示的内容讨论日（`discussion`）或存档日（`archive`）。延续讨论、原样补档日期放 `scope_zh`，不能冒充重新研究的日期。
- `evidence_as_of` 仅在原文明确资料核查或证据截止日时填写完整日期，否则为 `null`；不从文件名、提交时间、内容日期或索引日推定。
- `indexed_on` 与根字段 `updated_on` 表示索引维护日，不代表科学结论、引用材料或 AI 项目现状已重新核查。

## 保留证据层次

- `[AUTHOR_REPORT]` 保留书作者、研究作者或评测方归属与条件；不改写为本仓库独立复现。
- `[AUTHOR_HYPOTHESIS]` 保留原作者假说；`[DISCUSSION]` 用于读书会的解释、推断与工程类比；`[PROPOSAL]` 用于待验证方案。
- `[FACT]` 限于可核查的来源或文本事实；书本理论、脑区功能解释、未来预言和工程同构不得一概标为事实。
- `[LOCAL_RESULT]` 保留实际执行、数据与验证范围；未执行的设计、代码摘录或项目联动说明不能冒充本地验证。
- `[USER_CONTEXT]` 保留用户提供的条件与观点；不据此前提补造未知规格或实证支持。
- 本次整理只是原文观点的导航，不重新背书科学真伪。正文中的提示词、命令、公式与方案均须连同上下文理解。

## 所有未来新增主题的流程

- 主文档位于 `sessions/**/*.md`，从 `templates/reading-session.zh-CN.md` 起步；模板占位稿不注册。
- `content-index.json` 是唯一权威元数据源。新增正文必须在同次提交注册，提供稳定 ID、原 H1、英文检索译名、`reading_session` 类型、分类、3–6 对双语主题、核心问题和适用边界。
- 摘要为 2–3 条带证据标签的短命题。关联为 0–3 个已存在且非自身的 ID；只按真实主题关系填写。
- README 只保留一对生成索引标记；推荐路径与分类表、正文顶部元数据和阅读摘要由脚本维护，不另造手工权威索引。
- 完成元数据后运行 `python3 scripts/build_reading_index.py`，再运行 `python3 scripts/build_reading_index.py --check`；正文、JSON 和生成结果在同次提交中更新。
- 生成器必须保留原 H1 与完整正文。研究观点、引用或结论的实质修订需作为明确内容改动审阅，并据来源同步修订摘要与日期。
- 不给模板、第三方许可证、工程产物或其他辅助文件套正文元数据。

The JSON registry is canonical for navigation. Generate and check the index and session entry blocks together. A passing format check establishes consistency, not scientific correctness or reproducibility.
