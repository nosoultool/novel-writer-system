# Agent 专用知识库

> 每个智能体的"生存本领"。调用 Agent 时自动加载对应的知识库作为上下文。

## 结构

```
agents/knowledge/
├── README.md                          ← 本文件
│
├── writer/                            ← 写手智能体专用
│   ├── chapter-craft.md              章节构建、场景、对话技法（核心知识）
│   └── learned/                      从作品学习的写作技法 + 自我提升方案
│
├── reviewer/                          ← 审查官智能体专用
│   └── review-standards.md           审查标准、错误拦截、严重度分级
│
├── character-designer/                ← 角色设计师智能体专用
│   ├── character-evolution.md        角色状态管理、弧光设计（核心知识）
│   └── learned/                      从作品学习的角色设计技法
│
├── plot-architect/                    ← 剧情架构师智能体专用
│   ├── arc-management.md             伏笔管理、节奏控制（核心知识）
│   └── learned/                      从作品学习的情节设计技法
│
├── worldbuilding-architect/           ← 世界观架构师智能体专用
│   ├── world-rules.md                世界观一致性、力量体系（核心知识）
│   └── learned/                      从作品学习的世界观构建技法
│
├── polish/                            ← 润色师智能体专用
│   ├── ai-detection-signals.md       AI痕迹检测与去AI化（核心知识）
│   └── learned/                      从作品学习的文风技法
│
├── era-consistency/                   ← 时代审查官智能体专用
│   └── era-check-standards.md        时代审查标准
│
├── short-story/                       ← 短故事专项智能体专用
│   └── short-story-craft.md          短故事创作技法
│
├── story-setup/                       ← 创作设定智能体专用
│   └── setup-standards.md            设定协调指南
│
└── setting-qa/                        ← 设定质检员智能体专用
    ├── logic-consistency.md          逻辑自洽性检查（核心知识）
    ├── power-balance.md              力量平衡检查
    ├── timeline-integrity.md         时间线完整性检查
    ├── causality-chain.md            因果链检查
    ├── resource-economy.md           资源经济检查
    └── learned/                      从作品学习的设定技法
```

## 三层知识体系

| 层次 | 内容 | 来源 | 更新机制 |
|:----|:-----|:-----|:---------|
| **核心知识** | Agent 完成本职工作必需的标准 | 系统设计、迭代优化 | 每次创作后审视优化 |
| **学习知识** | 从优秀作品中学到的技法 | `/novel:learn` | 用户分享作品后自动沉淀 |
| **自我提升** | 技法转化为 Agent 能力的改进方案 | 学习过程中的"对照分析" | 记录在 learned/ 的笔记中 |

### 核心知识 vs 学习知识的区别

| 维度 | 核心知识 | 学习知识 |
|:-----|:---------|:---------|
| 文件名 | `<agent>-craft.md` 等 | `learned/<技法名>.md` |
| 来源 | 系统设计、手动优化 | 从作品自动学习 |
| 稳定性 | 相对稳定，低频修改 | 持续积累，高频增长 |
| 用途 | 本职工作必需 | 能力扩展和提升 |

## 更新规则

所有知识库均标注 `updatable: true`，可在使用后根据经验优化：

| 触发时机 | 谁负责更新 |
|:--------|:----------|
| 发现新的写作技巧 | 写手智能体 → 更新 `writer/chapter-craft.md` |
| 发现新的审查标准 | 审查官智能体 → 更新 `reviewer/review-standards.md` |
| 角色管理经验总结 | 角色设计师 → 更新 `character-designer/character-evolution.md` |
| 剧情管理经验总结 | 剧情架构师 → 更新 `plot-architect/arc-management.md` |
| 设定发现或修正 | 世界观架构师 → 更新 `worldbuilding-architect/world-rules.md` |
| 用户分享作品学习 | `/novel:learn` → 各 Agent 写入 `learned/` 目录 |

## 通用 vs 专用

| 类型 | 位置 | 内容 | 谁用 |
|:----|:-----|:-----|:-----|
| 通用知识 | `knowledge/` | 标点、写作技巧、知识分类 | 所有 Agent |
| Agent 核心 | `agents/knowledge/<agent>/` | 各 Agent 的核心专长 | 对应 Agent |
| Agent 学习 | `agents/knowledge/<agent>/learned/` | 从作品吸收的技法+自我提升 | 对应 Agent，后续创作中应用 |
