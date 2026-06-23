---
name: post-archive
hook: post-archive
description: 存档后更新 RAG 索引和知识图谱
---

# 存档后更新钩子

## 触发时机
存档完成后自动触发。

## 执行流程
1. 调用 RAG 引擎将新章节编入索引
2. 更新角色状态快照
3. 更新伏笔跟踪记录
4. 清理临时文件
5. 生成存档摘要
