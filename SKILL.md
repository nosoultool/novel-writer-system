# 🎭 灵境 · 小说创作智能体系统 / LingJing — Novel Creation Multi-Agent System

> 🇨🇳 入口文件 — 加载此文件即启动灵境创作系统。
>
> 🇬🇧 Entry file — Load this file to launch the LingJing creation system.

---

## 📋 System Loading / 系统加载

### Quick Start / 快速启动
🇬🇧 Enter any of the following commands in Claude Code to start a workflow:
🇨🇳 在 Claude Code 中输入以下任一命令进入工作流：

| 🇬🇧 Command / 🇨🇳 命令 | 🇬🇧 Function / 🇨🇳 功能 |
|:--|:--|
| `/novel:start` | 🚀 🇬🇧 Launch creation wizard (new project or resume) / 🇨🇳 **启动创作向导** — 新建项目或继续已有作品 |
| `/novel:help` | 📖 🇬🇧 Show full command list / 🇨🇳 显示完整命令列表 |

---

## 🧠 Agent System / 智能体系统

🇬🇧 The system includes 7 specialized agents working in collaboration:
🇨🇳 系统包含 7 个专业智能体，分工协作：

| 🇬🇧 Agent / 🇨🇳 智能体 | 🇬🇧 Responsibility / 🇨🇳 职责 | 🇬🇧 Invocation / 🇨🇳 调用方式 |
|:--|:--|:--|
| **Commander / 总指挥** | 🇬🇧 Task distribution, workflow orchestration, quality control / 🇨🇳 任务分发、流程编排、质量把关 | Auto / 自动激活 |
| **World Architect / 世界观架构师** | 🇬🇧 Worldbuilding, geography, power systems / 🇨🇳 世界观设定、地理/势力/力量体系设计 | `/novel:world` |
| **Character Designer / 角色设计师** | 🇬🇧 Character creation, relationships, growth arcs / 🇨🇳 角色创建、关系网、成长弧光 | `/novel:characters` |
| **Plot Architect / 剧情架构师** | 🇬🇧 Outline planning, volume structure, plot design / 🇨🇳 大纲规划、分卷、情节设计 | `/novel:outline` |
| **Writer / 写手** | 🇬🇧 Body text writing, scene description, dialogue / 🇨🇳 正文写作、场景描写、对话 | `/novel:write` |
| **Reviewer / 审查官** | 🇬🇧 Consistency check, quality assessment, logic validation / 🇨🇳 一致性检查、质量评估、逻辑校验 | `/novel:review` |
| **Polisher / 润色师** | 🇬🇧 De-AI polish, style unification, language optimization / 🇨🇳 去AI化、文风统一、语言优化 | `/novel:anti-ai` |

---

## 📂 Skills Index / Skills 索引

### 00 — Full Creative Workflow / 创作全流程
| 🇬🇧 File / 🇨🇳 文件 | 🇬🇧 Description / 🇨🇳 说明 |
|:--|:--|
| `skills/00-创作全流程/novel-setup.md` | 🇬🇧 Project initialization / 🇨🇳 项目初始化 |
| `skills/00-创作全流程/novel-discuss.md` | 🇬🇧 Creative discussion / 🇨🇳 创作讨论 |
| `skills/00-创作全流程/worldbuilding.md` | 🇬🇧 Worldbuilding / 🇨🇳 世界观搭建 |
| `skills/00-创作全流程/character-design.md` | 🇬🇧 Character design / 🇨🇳 角色设计 |
| `skills/00-创作全流程/plot-outline.md` | 🇬🇧 Plot outline / 🇨🇳 大纲规划 |
| `skills/00-创作全流程/chapter-writing.md` | 🇬🇧 Chapter writing / 🇨🇳 章节写作 |
| `skills/00-创作全流程/chapter-review.md` | 🇬🇧 Chapter review / 🇨🇳 章节审查 |
| `skills/00-创作全流程/anti-ai-polish.md` | 🇬🇧 De-AI polish / 🇨🇳 去AI化润色 |
| `skills/00-创作全流程/archive.md` | 🇬🇧 Archive & knowledge update / 🇨🇳 存档与知识更新 |

### 01 — Creative Techniques / 创作技巧
| 🇬🇧 File / 🇨🇳 文件 | 🇬🇧 Description / 🇨🇳 说明 |
|:--|:--|
| `skills/01-创作技巧/booming-plot.md` | 🇬🇧 Plot acceleration / 🇨🇳 剧情引爆 |
| `skills/01-创作技巧/snowflake-method.md` | 🇬🇧 Snowflake method / 🇨🇳 雪花法大纲 |
| `skills/01-创作技巧/save-the-cat.md` | 🇬🇧 Save the Cat beat sheet / 🇨🇳 Save the Cat 节拍表 |
| `skills/01-创作技巧/decoupled-writing.md` | 🇬🇧 Decoupled writing / 🇨🇳 解耦写作法 |
| `skills/01-创作技巧/style-learning.md` | 🇬🇧 Style learning / 🇨🇳 风格学习 |

### 02 — Web Novel Specialties / 网文专项
| 🇬🇧 File / 🇨🇳 文件 | 🇬🇧 Description / 🇨🇳 说明 |
|:--|:--|
| `skills/02-网文专项/webnovel-hook.md` | 🇬🇧 Golden three chapters / hooks / 🇨🇳 黄金三章/钩子 |
| `skills/02-网文专项/webnovel-shuang.md` | 🇬🇧 Shuang point design / 🇨🇳 爽点设计 |
| `skills/02-网文专项/webnovel-trend.md` | 🇬🇧 Trend analysis / scouting / 🇨🇳 扫榜/趋势分析 |
| `skills/02-网文专项/webnovel-goldfinger.md` | 🇬🇧 Golden finger design / 🇨🇳 金手指设计 |
| `skills/02-网文专项/webnovel-submit.md` | 🇬🇧 Submission / platform adaptation / 🇨🇳 投稿/平台适配 |

### 03 — Quality Review / 质量审查
| 🇬🇧 File / 🇨🇳 文件 | 🇬🇧 Description / 🇨🇳 说明 |
|:--|:--|
| `skills/03-质量审查/consistency-check.md` | 🇬🇧 Consistency check / 🇨🇳 一致性检查 |
| `skills/03-质量审查/quality-gates.md` | 🇬🇧 Quality gates / 🇨🇳 质量门禁 |
| `skills/03-质量审查/deslop-check.md` | 🇬🇧 De-AI review / 🇨🇳 去AI化审查 |
| `skills/03-质量审查/banned-words.md` | 🇬🇧 Banned words check / 🇨🇳 违禁词检查 |
| `skills/03-质量审查/plot-hole-check.md` | 🇬🇧 Plot hole detection / 🇨🇳 漏洞检测 |

### 04 — Tool Integration / 工具集成
| 🇬🇧 File / 🇨🇳 文件 | 🇬🇧 Description / 🇨🇳 说明 |
|:--|:--|
| `skills/04-工具集成/knowledge-graph.md` | 🇬🇧 Knowledge graph management / 🇨🇳 知识图谱管理 |
| `skills/04-工具集成/memory-system.md` | 🇬🇧 Memory system / 🇨🇳 记忆系统 |
| `skills/04-工具集成/progress-track.md` | 🇬🇧 Progress tracking / 🇨🇳 进度追踪 |
| `skills/04-工具集成/obsidian-sync.md` | 🇬🇧 Obsidian sync / 🇨🇳 Obsidian 同步 |

---

## 🔄 General Workflow / 通用工作流

| Step | 🇬🇧 Command / 🇨🇳 命令 | 🇬🇧 Action / 🇨🇳 操作 |
|:--|:--|:--|
| 1 | `/novel:discuss` | 🇬🇧 Discuss ideas, set direction / 🇨🇳 讨论创意、确定方向 |
| 2 | `/novel:world` | 🇬🇧 Build the world / 🇨🇳 搭建世界观 |
| 3 | `/novel:characters` | 🇬🇧 Design characters / 🇨🇳 设计角色 |
| 4 | `/novel:outline` | 🇬🇧 Plan outline / 🇨🇳 规划大纲 |
| 5 | `/novel:write` | 🇬🇧 Write chapter by chapter / 🇨🇳 逐章写作 |
| 6 | `/novel:review` | 🇬🇧 Review and revise / 🇨🇳 审查修改 |
| 7 | `/novel:anti-ai` | 🇬🇧 De-AI polish / 🇨🇳 去AI化 |
| 8 | `/novel:archive` | 🇬🇧 Update knowledge base / 🇨🇳 更新知识库 |
|   | ↻ | 🇬🇧 Repeat 5-8 / 🇨🇳 重复 5-8 |
