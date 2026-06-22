# Claude Code Configuration — LingJing Novel Creation System

## Auto-Load
When you open Claude Code in this directory, the system is ready automatically.

## Working Directory Convention
- `works/` — Novel projects (each project in its own subdirectory)
- `works/{project}/manuscript/` — Body text
- `works/{project}/bible/` — Novel bible (worldbuilding, characters, etc.)
- `works/{project}/memory/` — Writing memory

## System Structure
- `agents/` — Agent role definitions (8 agents)
- `skills/` — Skill playbooks (创作全流程/创作技巧/网文专项/质量审查/工具集成)
- `hooks/` — Lifecycle hooks (pre-review era consistency check)
- `era-knowledge/` — Era consistency knowledge base (per-project)

## Recommended Settings
> It is recommended to disable thinking mode (thinking mode off)
