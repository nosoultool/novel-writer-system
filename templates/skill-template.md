---
id: skill-template
name: 技能创建模板
type: template
description: 用于创建新的技能文件，包含标准frontmatter和工作流章节
---

# <emoji> <名称> Skill

## 元数据

```yaml
---
id: <skill-id>                     # 唯一标识，小写英文，连字符分隔
name: <中文名> Skill                # 完整名称
category: <NN-类别>                # 所属分类目录
command: <命令>                    # /novel:xxx
description: <一行功能说明>          # 最多20字
created: <YYYY-MM-DD>
updated: <YYYY-MM-DD>
---
```

## 命令

`<命令>`

## 功能

<技能的核心功能和用途说明>

## 工作流程

1. <步骤一>
2. <步骤二>
3. <步骤三>

## 输出

<技能产生的输出>

---

> **扩展说明：**
> - 新建 Skill 后，在 `skills/REGISTRY.md` 对应类别下添加一行
> - 确保文件放在 `skills/<NN-类别>/` 目录下
> - 如果该 Skill 对应某 Agent 的前端命令，在 CLAUDE.md 中同步更新
