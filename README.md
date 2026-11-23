# 智能简史 · 读书会存档

读 Max Bennett《智能简史》（A Brief History of Intelligence）的专题笔记——五次突破逐章精读，与 AI Agent / 机器人工程逐条对账。

Reading notes on Max Bennett's *A Brief History of Intelligence*, with Chinese discussion records and bilingual navigation for readers and models.

## 方法与读书会约定

- **读法**：先通读全章，再逐段深钻；批注驱动的讨论（书页拍照 + 页边手写 → 逐条校准）；
- **对账维度**：每个神经科学概念对照三个坐标系——控制论/机器人学（IMU、SLAM、状态观测器）、强化学习（TD、Actor-Critic、model-free/model-based）、Agent 工程（harness、闭环、工具）；
- **核心框架**：五次突破 = 五次需求升级；解剖分区 = 功能需求的化石记录；化石双向可读（解剖→需求文档，痛点→预测器官）。这是读书会采用的解释框架，摘要保留其讨论归属。
- **后续讨论**：回答书页问题时不主动关联 MicroDuck/鸭子项目，除非用户点名；不剧透尚未读到的后续章节。早期笔记中约定提出前的讨论原样保留。

## 如何阅读 · How to Read

`sessions/` 保存按生物演化时间线编排的精读笔记。[content-index.json](content-index.json) 是唯一权威导航元数据源；下方路径与分类表、各篇入口摘要由脚本生成。先按核心问题、双语主题和阅读路径选少量文档，再读其摘要、适用边界与原正文。摘要不能替代正文或原始出处，关联 ID 只表示主题相关。

`document_id` 使用稳定的 `ABHI-NNN`，`session_id` 与其同值；新增主题追加下一个未使用编号，既有 ID 不随排序改变。英文标题用于检索，正文语言为中文。

日期有三种口径：`content_date` 与 `content_date_kind` 记录原文明确的讨论或存档日期；`evidence_as_of` 只用于明确的资料核查/证据截止日期，未知为 `null`；`indexed_on` 与根字段 `updated_on` 仅表示索引维护日期。原文补档或延续讨论在适用边界说明；索引更新不表示重新核验书中理论或 AI 项目现状。

摘要标签保留主张的证据层次：`AUTHOR_REPORT` 是原作者或外部报告，`AUTHOR_HYPOTHESIS` 是作者假说，`DISCUSSION` 是解释、推断或类比，`PROPOSAL` 是待验证建议。`FACT` 仅指可核查的来源事实，`LOCAL_RESULT` 须保留实际本地验证范围，`USER_CONTEXT` 表示用户前提。书本理论与工程类比不会因写入索引而升级为已验证事实。

Use the registry to select relevant sessions, then read the original discussion and its limits. Content dates, evidence cutoffs, and indexing dates have separate meanings. Translated titles and short summaries support navigation; they do not replace source prose or independently verify its claims.

<!-- BEGIN GENERATED RESEARCH INDEX -->
## 推荐阅读路径 · Suggested Reading Routes

### 身体状态怎样进入奖励与自我表征？ · How do bodily states enter rewards and self-representation?

1. [ABHI-001 Session 01 · 线虫模拟环境详解](sessions/01-%E7%BA%BF%E8%99%AB%E6%A8%A1%E6%8B%9F%E7%8E%AF%E5%A2%83%E8%AF%A6%E8%A7%A3.md)
2. [ABHI-002 Session 02 · 第一个世界模型：空间定位与自我的诞生](sessions/02-%E7%AC%AC%E4%B8%80%E4%B8%AA%E4%B8%96%E7%95%8C%E6%A8%A1%E5%9E%8B%EF%BC%9A%E7%A9%BA%E9%97%B4%E5%AE%9A%E4%BD%8D%E4%B8%8E%E8%87%AA%E6%88%91%E7%9A%84%E8%AF%9E%E7%94%9F.md)
3. [ABHI-003 Session 03 · 第二次突破：强化——RL 组件的演化组装](sessions/03-%E7%AC%AC%E4%BA%8C%E6%AC%A1%E7%AA%81%E7%A0%B4%EF%BC%9A%E5%BC%BA%E5%8C%96%E2%80%94%E2%80%94RL%E7%BB%84%E4%BB%B6%E7%9A%84%E6%BC%94%E5%8C%96%E7%BB%84%E8%A3%85.md)

### 感知与想象怎样共同约束世界模型？ · How do perception and imagination constrain world models?

1. [ABHI-004 Session 04 · 第三次突破：模拟、生成模型与趋同原理](sessions/04-%E7%AC%AC%E4%B8%89%E6%AC%A1%E7%AA%81%E7%A0%B4%EF%BC%9A%E6%A8%A1%E6%8B%9F%E3%80%81%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E4%B8%8E%E8%B6%8B%E5%90%8C%E5%8E%9F%E7%90%86.md)
2. [ABHI-005 Session 05 · 亥姆霍兹：感知即推断](sessions/05-%E4%BA%A5%E5%A7%86%E9%9C%8D%E5%85%B9%EF%BC%9A%E6%84%9F%E7%9F%A5%E5%8D%B3%E6%8E%A8%E6%96%AD.md)
3. [ABHI-006 Session 06 · 幻觉、梦与想象：受约束的幻觉](sessions/06-%E5%B9%BB%E8%A7%89%E6%A2%A6%E4%B8%8E%E6%83%B3%E8%B1%A1%EF%BC%9A%E5%8F%97%E7%BA%A6%E6%9D%9F%E7%9A%84%E5%B9%BB%E8%A7%89.md)
4. [ABHI-007 Session 07 · 预测一切：新皮质任务书与鸭子新皮质萌芽](sessions/07-%E9%A2%84%E6%B5%8B%E4%B8%80%E5%88%87%EF%BC%9A%E6%96%B0%E7%9A%AE%E8%B4%A8%E4%BB%BB%E5%8A%A1%E4%B9%A6%E4%B8%8E%E9%B8%AD%E5%AD%90%E6%96%B0%E7%9A%AE%E8%B4%A8%E8%90%8C%E8%8A%BD.md)

### 回放如何连接规划、自身意图与他人心智？ · How does replay connect planning, intention, and other minds?

1. [ABHI-008 Session 08 · 想象世界的老鼠：回放、世界模型与前额叶的意志](sessions/08-%E6%83%B3%E8%B1%A1%E4%B8%96%E7%95%8C%E7%9A%84%E8%80%81%E9%BC%A0%EF%BC%9A%E5%9B%9E%E6%94%BE%E3%80%81%E4%B8%96%E7%95%8C%E6%A8%A1%E5%9E%8B%E4%B8%8E%E5%89%8D%E9%A2%9D%E5%8F%B6%E7%9A%84%E6%84%8F%E5%BF%97.md)
2. [ABHI-009 Session 09 · 意图的进化：习惯、阈值与运动分层](sessions/09-%E6%84%8F%E5%9B%BE%E7%9A%84%E8%BF%9B%E5%8C%96%EF%BC%9A%E4%B9%A0%E6%83%AF%E3%80%81%E9%98%88%E5%80%BC%E4%B8%8E%E8%BF%90%E5%8A%A8%E5%88%86%E5%B1%82.md)
3. [ABHI-010 Session 10 · 如何模拟他人心智：二阶模型与群体自我的判据](sessions/10-%E5%A6%82%E4%BD%95%E6%A8%A1%E6%8B%9F%E4%BB%96%E4%BA%BA%E5%BF%83%E6%99%BA%EF%BC%9A%E4%BA%8C%E9%98%B6%E6%A8%A1%E5%9E%8B%E4%B8%8E%E7%BE%A4%E4%BD%93%E8%87%AA%E6%88%91%E7%9A%84%E5%88%A4%E6%8D%AE.md)

### 语言怎样改变合作与跨世代积累？ · How does language change cooperation and cumulative culture?

1. [ABHI-011 Session 11 · 共同神话：合作规模的压缩协议与神的账本](sessions/11-%E5%85%B1%E5%90%8C%E7%A5%9E%E8%AF%9D%EF%BC%9A%E5%90%88%E4%BD%9C%E8%A7%84%E6%A8%A1%E7%9A%84%E5%8E%8B%E7%BC%A9%E5%8D%8F%E8%AE%AE%E4%B8%8E%E7%A5%9E%E7%9A%84%E8%B4%A6%E6%9C%AC.md)
2. [ABHI-012 Session 12 · 语言的征用：蜂巢式大脑、思想的复制子与文明的形态](sessions/12-%E8%AF%AD%E8%A8%80%E7%9A%84%E5%BE%81%E7%94%A8%EF%BC%9A%E8%9C%82%E5%B7%A2%E5%BC%8F%E5%A4%A7%E8%84%91%E3%80%81%E6%80%9D%E6%83%B3%E7%9A%84%E5%A4%8D%E5%88%B6%E5%AD%90%E4%B8%8E%E6%96%87%E6%98%8E%E7%9A%84%E5%BD%A2%E6%80%81.md)
3. [ABHI-013 Session 13 · 第六次突破的悬崖：八卦循环、残暴的账目与目标的初值](sessions/13-%E7%AC%AC%E5%85%AD%E6%AC%A1%E7%AA%81%E7%A0%B4%E7%9A%84%E6%82%AC%E5%B4%96%EF%BC%9A%E5%85%AB%E5%8D%A6%E5%BE%AA%E7%8E%AF%E3%80%81%E6%AE%8B%E6%9A%B4%E7%9A%84%E8%B4%A6%E7%9B%AE%E4%B8%8E%E7%9B%AE%E6%A0%87%E7%9A%84%E5%88%9D%E5%80%BC.md)

## 内容索引 · Content Index

### 具身感知与强化学习 · Embodied Perception and Reinforcement Learning

| ID | 中文文档 | English Title | 类型 · Type | 日期与口径 · Dates |
|---|---|---|---|---|
| ABHI-001 | [Session 01 · 线虫模拟环境详解](sessions/01-%E7%BA%BF%E8%99%AB%E6%A8%A1%E6%8B%9F%E7%8E%AF%E5%A2%83%E8%AF%A6%E8%A7%A3.md) | Session 01 · Embodied Worm Simulation Explained | 读书会笔记 · Reading session | 存档 2026-09-29；证据截止未注明 |
| ABHI-002 | [Session 02 · 第一个世界模型：空间定位与自我的诞生](sessions/02-%E7%AC%AC%E4%B8%80%E4%B8%AA%E4%B8%96%E7%95%8C%E6%A8%A1%E5%9E%8B%EF%BC%9A%E7%A9%BA%E9%97%B4%E5%AE%9A%E4%BD%8D%E4%B8%8E%E8%87%AA%E6%88%91%E7%9A%84%E8%AF%9E%E7%94%9F.md) | Session 02 · The First World Model: Spatial Localization and the Emergence of Self | 读书会笔记 · Reading session | 存档 2026-09-29；证据截止未注明 |
| ABHI-003 | [Session 03 · 第二次突破：强化——RL 组件的演化组装](sessions/03-%E7%AC%AC%E4%BA%8C%E6%AC%A1%E7%AA%81%E7%A0%B4%EF%BC%9A%E5%BC%BA%E5%8C%96%E2%80%94%E2%80%94RL%E7%BB%84%E4%BB%B6%E7%9A%84%E6%BC%94%E5%8C%96%E7%BB%84%E8%A3%85.md) | Session 03 · The Second Breakthrough: Reinforcement and the Evolutionary Assembly of RL Components | 读书会笔记 · Reading session | 存档 2026-09-29；证据截止未注明 |

### 模拟、生成模型与感知 · Simulation, Generative Models, and Perception

| ID | 中文文档 | English Title | 类型 · Type | 日期与口径 · Dates |
|---|---|---|---|---|
| ABHI-004 | [Session 04 · 第三次突破：模拟、生成模型与趋同原理](sessions/04-%E7%AC%AC%E4%B8%89%E6%AC%A1%E7%AA%81%E7%A0%B4%EF%BC%9A%E6%A8%A1%E6%8B%9F%E3%80%81%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E4%B8%8E%E8%B6%8B%E5%90%8C%E5%8E%9F%E7%90%86.md) | Session 04 · The Third Breakthrough: Simulation, Generative Models, and Convergence | 读书会笔记 · Reading session | 存档 2026-09-29；证据截止未注明 |
| ABHI-005 | [Session 05 · 亥姆霍兹：感知即推断](sessions/05-%E4%BA%A5%E5%A7%86%E9%9C%8D%E5%85%B9%EF%BC%9A%E6%84%9F%E7%9F%A5%E5%8D%B3%E6%8E%A8%E6%96%AD.md) | Session 05 · Helmholtz: Perception as Inference | 读书会笔记 · Reading session | 存档 2026-09-29；证据截止未注明 |
| ABHI-006 | [Session 06 · 幻觉、梦与想象：受约束的幻觉](sessions/06-%E5%B9%BB%E8%A7%89%E6%A2%A6%E4%B8%8E%E6%83%B3%E8%B1%A1%EF%BC%9A%E5%8F%97%E7%BA%A6%E6%9D%9F%E7%9A%84%E5%B9%BB%E8%A7%89.md) | Session 06 · Hallucinations, Dreams, and Imagination: Constrained Hallucination | 读书会笔记 · Reading session | 存档 2026-09-29；证据截止未注明 |
| ABHI-007 | [Session 07 · 预测一切：新皮质任务书与鸭子新皮质萌芽](sessions/07-%E9%A2%84%E6%B5%8B%E4%B8%80%E5%88%87%EF%BC%9A%E6%96%B0%E7%9A%AE%E8%B4%A8%E4%BB%BB%E5%8A%A1%E4%B9%A6%E4%B8%8E%E9%B8%AD%E5%AD%90%E6%96%B0%E7%9A%AE%E8%B4%A8%E8%90%8C%E8%8A%BD.md) | Session 07 · Predicting Everything: A Neocortical Specification and an Emerging Robot World Model | 读书会笔记 · Reading session | 存档 2026-10-02；证据截止未注明 |

### 回放、规划与意图 · Replay, Planning, and Intention

| ID | 中文文档 | English Title | 类型 · Type | 日期与口径 · Dates |
|---|---|---|---|---|
| ABHI-008 | [Session 08 · 想象世界的老鼠：回放、世界模型与前额叶的意志](sessions/08-%E6%83%B3%E8%B1%A1%E4%B8%96%E7%95%8C%E7%9A%84%E8%80%81%E9%BC%A0%EF%BC%9A%E5%9B%9E%E6%94%BE%E3%80%81%E4%B8%96%E7%95%8C%E6%A8%A1%E5%9E%8B%E4%B8%8E%E5%89%8D%E9%A2%9D%E5%8F%B6%E7%9A%84%E6%84%8F%E5%BF%97.md) | Session 08 · Replay, World Models, and Prefrontal Intention in Rats | 读书会笔记 · Reading session | 存档 2026-10-03；证据截止未注明 |
| ABHI-009 | [Session 09 · 意图的进化：习惯、阈值与运动分层](sessions/09-%E6%84%8F%E5%9B%BE%E7%9A%84%E8%BF%9B%E5%8C%96%EF%BC%9A%E4%B9%A0%E6%83%AF%E3%80%81%E9%98%88%E5%80%BC%E4%B8%8E%E8%BF%90%E5%8A%A8%E5%88%86%E5%B1%82.md) | Session 09 · The Evolution of Intention: Habits, Thresholds, and Motor Hierarchy | 读书会笔记 · Reading session | 存档 2026-10-05；证据截止未注明 |

### 心智化、合作与语言 · Mentalizing, Cooperation, and Language

| ID | 中文文档 | English Title | 类型 · Type | 日期与口径 · Dates |
|---|---|---|---|---|
| ABHI-010 | [Session 10 · 如何模拟他人心智：二阶模型与群体自我的判据](sessions/10-%E5%A6%82%E4%BD%95%E6%A8%A1%E6%8B%9F%E4%BB%96%E4%BA%BA%E5%BF%83%E6%99%BA%EF%BC%9A%E4%BA%8C%E9%98%B6%E6%A8%A1%E5%9E%8B%E4%B8%8E%E7%BE%A4%E4%BD%93%E8%87%AA%E6%88%91%E7%9A%84%E5%88%A4%E6%8D%AE.md) | Session 10 · Modeling Other Minds: Second-Order Models and Criteria for a Collective Self | 读书会笔记 · Reading session | 讨论 2026-10-05；证据截止未注明 |
| ABHI-011 | [Session 11 · 共同神话：合作规模的压缩协议与神的账本](sessions/11-%E5%85%B1%E5%90%8C%E7%A5%9E%E8%AF%9D%EF%BC%9A%E5%90%88%E4%BD%9C%E8%A7%84%E6%A8%A1%E7%9A%84%E5%8E%8B%E7%BC%A9%E5%8D%8F%E8%AE%AE%E4%B8%8E%E7%A5%9E%E7%9A%84%E8%B4%A6%E6%9C%AC.md) | Session 11 · Shared Myths: A Compression Protocol for Cooperation and the Divine Ledger | 读书会笔记 · Reading session | 存档 2026-10-07；证据截止未注明 |
| ABHI-012 | [Session 12 · 语言的征用：蜂巢式大脑、思想的复制子与文明的形态](sessions/12-%E8%AF%AD%E8%A8%80%E7%9A%84%E5%BE%81%E7%94%A8%EF%BC%9A%E8%9C%82%E5%B7%A2%E5%BC%8F%E5%A4%A7%E8%84%91%E3%80%81%E6%80%9D%E6%83%B3%E7%9A%84%E5%A4%8D%E5%88%B6%E5%AD%90%E4%B8%8E%E6%96%87%E6%98%8E%E7%9A%84%E5%BD%A2%E6%80%81.md) | Session 12 · Language Exaptation: Hive Minds, Replicating Ideas, and the Forms of Civilization | 读书会笔记 · Reading session | 存档 2026-10-07；证据截止未注明 |
| ABHI-013 | [Session 13 · 第六次突破的悬崖：八卦循环、残暴的账目与目标的初值](sessions/13-%E7%AC%AC%E5%85%AD%E6%AC%A1%E7%AA%81%E7%A0%B4%E7%9A%84%E6%82%AC%E5%B4%96%EF%BC%9A%E5%85%AB%E5%8D%A6%E5%BE%AA%E7%8E%AF%E3%80%81%E6%AE%8B%E6%9A%B4%E7%9A%84%E8%B4%A6%E7%9B%AE%E4%B8%8E%E7%9B%AE%E6%A0%87%E7%9A%84%E5%88%9D%E5%80%BC.md) | Session 13 · At the Edge of the Sixth Breakthrough: Gossip, Cruelty, and Initial Goals | 读书会笔记 · Reading session | 存档 2026-10-07；证据截止未注明 |

<!-- END GENERATED RESEARCH INDEX -->

## 新增主题与维护

所有未来新增主题均从 [templates/reading-session.zh-CN.md](templates/reading-session.zh-CN.md) 起步；模板是占位稿，不注册为正文。新增或实质修订笔记时，同步维护 `content-index.json` 的双语标题与主题、核心问题、2–3 条带标签摘要、日期、适用边界和关联 ID，再运行：

```bash
python3 scripts/build_reading_index.py
python3 scripts/build_reading_index.py --check
```

将正文、JSON 与生成结果放在同一次提交。生成器保留原 H1 和正文；正文观点修改需单独明确审阅。完整约定见 [AGENTS.md](AGENTS.md)。

## 关联

- 长期记忆条目：「自我演化阶梯」（具身智能体公式续篇）、「海洋三段论+趋同原理」、「意图四讲」
- 姊妹项目：[my-microduck](https://github.com/ReadbytheBeach/my-microduck)（MicroDuck 机器人学习笔记；鸭子新皮质正式设计文档将入其 docs/）
