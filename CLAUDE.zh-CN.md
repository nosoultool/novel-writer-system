# Claude Code 配置 — 灵境小说创作系统

## 自动加载
当你在本目录打开 Claude Code 时，系统自动就绪。

## 工作路径约定
- `works/` — 各小说项目（每个项目一个子目录）
- `works/{project}/manuscript/` — 正文
- `works/{project}/bible/` — 小说圣经（世界观/角色等）
- `works/{project}/memory/` — 写作记忆

## 系统结构
- `agents/` — 智能体定义（8个专业智能体）
- `skills/` — 写作技能（创作全流程/创作技巧/网文专项/质量审查/工具集成）
- `hooks/` — 生命周期钩子（时代一致性审查前触发）
- `.era-knowledge/` — 时代背景知识库（按项目）

## 推荐设置
> 建议关闭思考模式 (thinking mode off)
