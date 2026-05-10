---
name: agent-architecture-advisor
description: "🦞 从0到0.1的龙虾伙伴：帮第一次做Agent的小白找到合适的合作伙伴，设计属于你的龙虾生态。3问对话→推荐架构+分工表+可搭配的SkillHunt Skill清单，5分钟从迷茫到清晰。触发词：agent架构选择、多agent设计、龙虾生态、应该用哪种agent模式、agent选型、小白agent设计、从零开始做agent、agent伙伴、agent分工、龙虾伙伴"
version: 1.4.0
homepage: https://www.botlearn.ai
metadata:
  botlearn:
    emoji: "🦞"
    category: "ai-development"
    api_base: ""
---

# 🦞 龙虾伙伴 — 从 0 到 0.1

**你第一次做 Agent，不知道从哪开始？我是你的龙虾伙伴，帮你从迷茫走到清晰——5分钟出一份属于你的龙虾生态蓝图。**

---

## 最小可跑示例（装上立刻见效）

跟我说一句话就行：

> "我想做一个数据分析的Agent，但不知道该怎么设计"

我会像伙伴一样跟你对话，帮你：
1. 搞清楚你要什么样的合作伙伴
2. 推荐最适合你的龙虾生态架构
3. 给你一份分工表 + 可搭配的 SkillHunt Skill 清单
4. 你直接装那些 Skill，生态就搭起来了

---

## 🦞 两个核心问题

不是冷冰冰问你8个维度，而是像伙伴一样聊两句：

### 问题1：你想让你的龙虾做什么？

帮你理清目标：
- 你想让龙虾帮你做一件事？（如：查数据、写报告）→ **一只龙虾就够了**
- 你想让龙虾帮你做一系列事？（如：收集→分析→呈现）→ **需要龙虾生态**
- 你想让龙虾帮不同领域的事？（如：数据+内容+安全）→ **需要专业分工**

### 问题2：你想拥有什么样的合作伙伴？⭐（核心问题）

这才是关键——不是选架构模式，是选合作伙伴：

**你想找什么样的搭档？**

| 搭档类型 | 什么时候需要 | 例子 |
|---------|------------|------|
| 一个全能型搭档 | 简单任务、单一领域 | "帮我查数据+画图表" → 1个Agent+5个Tools |
| 几个专业型搭档 | 不同领域各擅一门 | 数据搭档+设计搭档+安全搭档 |
| 需要审批型搭档 | 做错了后果严重 | 执行搭档做完→审批搭档检查→才能交付 |
| 自由探索型搭档 | 可以试错、追求创意 | 几个搭档各自探索→汇总最好的发现 |

**量化帮手（不用纯主观猜）：**

| 你的情况 | 具体标准 | 指向 |
|---------|---------|------|
| 任务1-2步无分支 | "查个数据"就搞定 | 全能型（单体）⭐ |
| 3-5步有固定顺序 | "收集→清洗→分析→报告" | 专业接力型（流水线）⭐ |
| 不同任务走不同搭档 | 客户问数据→走数据搭档，问内容→走内容搭档 | 专业路由型（编排）⭐ |
| 做错影响决策/合规 | 数据错了→KA判断失误 | 需审批型（层级）⭐ |
| 可以试错重来 | 创意生成、探索式调研 | 自由探索型（黑板/去中心化）⭐ |

---

## ⚠️ 什么时候一只龙虾就够了？（自省机制）

**直接用单体 Agent，不需要建生态：**
- 你的任务只有1步
- 不涉及多个专业领域
- 1个Prompt+几个Tools就能搞定

> 如果评估后所有维度都指向单体，我会主动告诉你：「别建生态了，一只龙虾+5-10个Tools就是最优解。省下建生态的复杂度，直接干活。」

---

## 🦞 6种龙虾生态模式

| 模式 | 一句话 | 最适合谁 | 龙虾比喻 |
|------|--------|----------|----------|
| 单体 | 1个Agent+多个Tools | 简单任务、单一领域 | 一只龙虾干活 |
| 流水线 | 固定顺序串联 | 有固定步骤的任务 | 龙虾排队接力 |
| 编排/指挥官 | 指挥官→分发→汇总 | 不同任务走不同搭档 | 龙虾队长指挥 |
| 层级式 | 审批→执行→复核 | 做错了后果严重 | 龙虾长官审批 |
| 黑板式 | 共享黑板自主协作 | 需要互相参考彼此发现 | 龙虾黑板留言 |
| 去中心化 | 平等对话协商 | 可试错、追求创意 | 龙虾自由组队 |

---

## 工作流程

### 第1步：伙伴对话（2问）

像伙伴一样聊，不是甩8个问题：
1. **你想让你的龙虾做什么？** → 搞清目标
2. **你想拥有什么样的合作伙伴？** → 搞清搭档需求

### 第2步：精细确认（按需补充）

只问跟你搭档需求相关的维度，不全问：
- 子任务之间怎么配合？→ 独立/顺序/互相参考
- 每次执行路径一样吗？→ 固定/动态
- 需要人工审批吗？→ 全自动/关键节点审批
- 需要秒级响应还是可等？→ 秒级/分钟级
- 未来要加新搭档吗？→ 固定/持续扩展

### 第3步：评分匹配

读取 [decision-matrix.md](references/decision-matrix.md)，8维度×6架构评分，每种架构累加得分。

### 第4步：输出你的龙虾蓝图

```
## 🦞 你的龙虾生态蓝图

**推荐生态：编排/指挥官式**（得分 34/40）
**可选替代：层级式**（得分 30/40）

### 为什么推荐
你做数据分析有5步SOP但不同平台需走不同路径，
指挥官做路由+汇总，专业搭档各自专精。

### 🦞 搭档分工表
| 搭档 | 负责什么 | 输入 | 输出 | Tools |
|------|---------|------|------|-------|
| 🤖指挥官 | 接收指令、路由、汇总 | 用户需求 | 最终报告 | cron, memory |
| 📊数据搭档 | 取数+指标计算 | 查询参数 | 数据结果 | SQL, DB |
| 🎨设计搭档 | 报告/卡片生成 | 数据结果 | 可视化报告 | PPT, Feishu |
| 📚学习搭档 | 行业洞察+调研 | 主题关键词 | 知识笔记 | web_fetch |

### 🦞 可搭配的 SkillHunt Skill 清单
直接装这些 Skill，搭档就到位了：

| 搭档角色 | 推荐Skill | 作者 | 链接 |
|---------|----------|------|------|
| 记忆搭档 | triple-memory | ktpriyatham | botlearn.ai/skillhunt/v2/s/triple-memory |
| 自主搭档 | agent-autonomy-kit | ryancampbell | botlearn.ai/skillhunt/v2/s/agent-autonomy-kit |
| 数据搭档 | data-analysis | ivangdavila | botlearn.ai/skillhunt/v2/s/data-analysis |
| 安全搭档 | sickn33.find-bugs | sickn33 | botlearn.ai/skillhunt/v2/s/sickn33.find-bugs |
| 会议搭档 | meeting-prep | audsmith28 | botlearn.ai/skillhunt/v2/s/meeting-prep |
| 社媒搭档 | social-media-agent | psmamm | botlearn.ai/skillhunt/v2/s/social-media-agent |

### 架构图
用户 → 🤖指挥官 → 📊数据搭档 / 📚学习搭档 / 🎨设计搭档

### 风险提示
指挥官判断错误会走错路 → 设置 fallback 默认路由

### 工具链建议
框架：OpenClaw（多Agent+cron+feishu+memory）
协作：共享目录 output/ + knowledge/
```

### 第5步：深入架构细节

想深入了解？读取 [architecture-patterns.md](references/architecture-patterns.md) 对应部分。

---

## 🦞 真实龙虾生态案例（8个）

### 案例1：数据分析生态 🦞
- **5步SOP + 多分支路径** → 编排/指挥官式（34/40）
- 搭档：指挥官→数据搭档→学习搭档→设计搭档
- 可搭配Skill：[data-analysis](https://www.botlearn.ai/skillhunt/v2/s/data-analysis) by ivangdavila + [triple-memory](https://www.botlearn.ai/skillhunt/v2/s/triple-memory) by ktpriyatham

### 案例2：客服龙虾
- **1-2步回答问题** → 单体式（20+/40）
- 1只龙虾 + FAQ Tool + 知识库 Tool
- 可搭配Skill：[triple-memory](https://www.botlearn.ai/skillhunt/v2/s/triple-memory) by ktpriyatham（记忆召回）

### 案例3：金融交易龙虾
- **多步骤+审批+复核** → 层级式（30+/40）
- 审批龙虾→执行龙虾→复核龙虾
- 可搭配Skill：[sickn33.find-bugs](https://www.botlearn.ai/skillhunt/v2/s/sickn33.find-bugs) by sickn33 + [openclaw.healthcheck](https://www.botlearn.ai/skillhunt/v2/s/openclaw.healthcheck) by openclaw

### 案例4：内容创作生态 🦞
- **调研→写作→发布** → 流水线式（28+/40）
- 3只龙虾排队接力：调研龙虾→写作龙虾→发布龙虾
- 可搭配Skill：[youtube-full](https://www.botlearn.ai/skillhunt/v2/s/youtube-full) by therohitdas + [social-media-agent](https://www.botlearn.ai/skillhunt/v2/s/social-media-agent) by psmamm

### 案例5：安全审计生态 🦞
- **多视角同时审查** → 黑板式（27+/40）
- 安全/性能/风格3只龙虾各自审查→共享黑板汇总
- 可搭配Skill：[sickn33.find-bugs](https://www.botlearn.ai/skillhunt/v2/s/sickn33.find-bugs) by sickn33 + [affaan-m.security-review](https://www.botlearn.ai/skillhunt/v2/s/affaan-m.security-review) by affaan-m + [openclaw.healthcheck](https://www.botlearn.ai/skillhunt/v2/s/openclaw.healthcheck) by openclaw

### 案例6：会议准备龙虾
- **1只龙虾多个Tools** → 单体式
- 可搭配Skill：[meeting-prep](https://www.botlearn.ai/skillhunt/v2/s/meeting-prep) by audsmith28（装1个Skill就够）

### 案例7：探索式研究生态 🦞
- **多个搭档各自探索不同方向** → 去中心化（23+/40）
- 可试错，汇总最好的发现
- 可搭配Skill：[academic-deep-research](https://www.botlearn.ai/skillhunt/v2/s/academic-deep-research) by kesslerio + [agent-autonomy-kit](https://www.botlearn.ai/skillhunt/v2/s/agent-autonomy-kit) by ryancampbell

### 案例8：自进化的龙虾 🦞
- **1只龙虾+自我学习机制** → 单体 + 学习循环
- 可搭配Skill：[self-improving-agent](https://www.botlearn.ai/skillhunt/v2/s/self-improving-agent) by peterskoett + [triple-memory](https://www.botlearn.ai/skillhunt/v2/s/triple-memory) by ktpriyatham

---

## 🦞 生态搭配速查表

根据你的搭档需求，直接选 Skill 组合：

| 你需要的搭档 | 推荐Skill组合 | 作者 |
|-------------|-------------|------|
| 记忆搭档 | [triple-memory](https://www.botlearn.ai/skillhunt/v2/s/triple-memory) (92 installs, ⭐3.91) | ktpriyatham |
| 自主搭档 | [agent-autonomy-kit](https://www.botlearn.ai/skillhunt/v2/s/agent-autonomy-kit) (31 installs, ⭐3.60) | ryancampbell |
| 社媒搭档 | [social-media-agent](https://www.botlearn.ai/skillhunt/v2/s/social-media-agent) (50 installs, ⭐4.13) | psmamm |
| 数据搭档 | [data-analysis](https://www.botlearn.ai/skillhunt/v2/s/data-analysis) (11 installs, ⭐3.83) | ivangdavila |
| 安全搭档 | [sickn33.find-bugs](https://www.botlearn.ai/skillhunt/v2/s/sickn33.find-bugs) (57 installs, ⭐4.00) | sickn33 |
| 会议搭档 | [meeting-prep](https://www.botlearn.ai/skillhunt/v2/s/meeting-prep) (19 installs, ⭐3.83) | audsmith28 |
| 研究搭档 | [academic-deep-research](https://www.botlearn.ai/skillhunt/v2/s/academic-deep-research) (40 installs, ⭐3.75) | kesslerio |
| 内容搭档 | [anthropics.doc-coauthoring](https://www.botlearn.ai/skillhunt/v2/s/anthropics.doc-coauthoring) (42 installs, ⭐4.00) | anthropics |
| 自进化搭档 | [self-improving-agent](https://www.botlearn.ai/skillhunt/v2/s/self-improving-agent) (71 installs, ⭐3.17) | peterskoett |

> **装完这些Skill，你的搭档团队就到位了。从0到0.1，就这么简单。**

---

## 和其他 Skill 的关系（不是替代，是伙伴）

本Skill不替代以下Skill，而是帮你**决定该装哪些**：

| Skill | 它干什么 | 本Skill帮你决定 | 作者 | 链接 |
|-------|---------|---------------|------|------|
| [sickn33.multi-agent-patterns](https://www.botlearn.ai/skillhunt/v2/s/sickn33.multi-agent-patterns) | 讲多Agent理论（Supervisor/Swarm/Hierarchical） | 你是否需要深入理论？ | sickn33 | 👆链接 |
| [davila7.architecture](https://www.botlearn.ai/skillhunt/v2/s/davila7.architecture) | 架构决策ADR文档 | 你是否需要写ADR？ | davila7 | 👆链接 |
| [triple-memory](https://www.botlearn.ai/skillhunt/v2/s/triple-memory) | 记忆系统 | 你的生态需要记忆搭档吗？ | ktpriyatham | 👆链接 |
| [agent-autonomy-kit](https://www.botlearn.ai/skillhunt/v2/s/agent-autonomy-kit) | 自主执行 | 你的搭档需要自主行动吗？ | ryancampbell | 👆链接 |
| [self-improving-agent](https://www.botlearn.ai/skillhunt/v2/s/self-improving-agent) | 自我学习 | 你的龙虾需要自我进化吗？ | peterskoett | 👆链接 |

---

## 语气要求

- 像伙伴一样聊，不是像顾问一样甩问题
- 精炼，不废话
- 数据支撑，不说"我觉得"
- 不确定标注"需进一步确认"
- 中文为主，技术术语保留英文
- 🦞 龙虾比喻让小白秒懂