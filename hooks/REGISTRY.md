---
id: hooks-registry
name: 钩子注册表
type: registry
description: 所有Hook的索引表——按stage/phase分类
updated: 2026-06-25
---

# 钩子注册表 (Hooks Registry)

> 总计：9 个钩子

## 注册表

| id | 名称 | stage | phase | 触发时机 | 文件 |
|:---|:-----|:------|:------|:---------|:-----|
| pre-write | 写作前准备钩子 | pre | write | before-write | hooks/pre-write.md |
| post-write | 写作后处理钩子 | post | write | after-write | hooks/post-write.md |
| post-all-check | 全流程完整性检查钩子 | post | write | after-all-checks | hooks/post-all-check.md |
| pre-review | 时代审查前准备钩子 | pre | review | before-review | hooks/pre-review.md |
| post-review | 审查后处理钩子 | post | review | after-review | hooks/post-review.md |
| pre-archive | 存档前验证钩子 | pre | archive | before-archive | hooks/pre-archive.md |
| post-archive | 存档后更新钩子 | post | archive | after-archive | hooks/post-archive.md |
| pre-discuss | 讨论前检索钩子 | pre | discuss | before-discuss | hooks/pre-discuss.md |
| session-init | 会话初始化钩子 | session | session | session-start | hooks/session-init.md |

## 生命周期

```
pre-* → [action] → post-*
session-* (会话级别)
```

- **pre**：执行前的准备/检查/加载
- **post**：执行后的验证/更新/存档
- **session**：会话生命周期管理

## 添加新钩子

参见 `templates/hook-template.md` 和 `templates/EXTENDING.md`
