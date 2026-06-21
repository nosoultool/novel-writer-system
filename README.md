# 📚 灵境 · 小说创作智能体系统

> **LingJing** — 一个集多智能体协作、模块化 Skills、知识图谱于一体的 AI 小说创作系统。

整合 GitHub 上最优秀的开源小说写作项目精华，为你量身打造的统一创作工具箱。

---

## ✨ 系统特色

| 特性 | 说明 |
|------|------|
| 🧠 **多 Agent 协作** | 7 个专业智能体分工协作 |
| 🧩 **模块化 Skills** | 30+ 独立 skill 覆盖创作全流程 |
| 📖 **双模式支持** | 长篇小说流水线 + 短篇快速创作 |
| 🎭 **去AI化引擎** | 多层检测与润色，输出自然流畅 |
| 📊 **知识图谱** | 角色/地点/事件关系持久化 |
| 🌐 **多平台适配** | 起点/番茄/晋江等平台优化 |

---

## 🚀 快速安装

### Windows
```powershell
# 方式一：使用安装脚本
iex "& { $(irm https://raw.githubusercontent.com/nosoultool/novel-writer-system/main/install.ps1) }"

# 方式二：手动克隆
git clone https://github.com/nosoultool/novel-writer-system.git
cd novel-writer-system
```

### macOS / Linux
```bash
# 方式一：使用安装脚本
bash <(curl -s https://raw.githubusercontent.com/nosoultool/novel-writer-system/main/install.sh)

# 方式二：手动克隆
git clone https://github.com/nosoultool/novel-writer-system.git
cd novel-writer-system
```

---

## 📖 使用方式（多平台）

### 🥇 Claude Code（推荐 · 全功能）

Claude Code 是本系统的最佳运行环境，支持完整的 Agent 和 Skill 调用。

```bash
cd novel-writer-system
claude
# 在 Claude Code 中输入 /novel:start
```

**支持的命令：**
| 命令 | 功能 |
|------|------|
| `/novel:start` | 🚀 启动创作向导 |
| `/novel:new` | 新建小说项目 |
| `/novel:discuss` | 创作讨论/头脑风暴 |
| `/novel:world` | 🌍 世界观搭建 |
| `/novel:characters` | 👤 角色管理 |
| `/novel:outline` | 📋 大纲规划 |
| `/novel:write` | ✍️ 正文写作 |
| `/novel:review` | 🔍 章节审查 |
| `/novel:anti-ai` | 🎨 去AI化润色 |
| `/novel:check` | 🔗 一致性检查 |
| `/novel:booming` | 💥 剧情引爆（卡文时） |
| `/novel:archive` | 📦 存档更新 |
| `/novel:progress` | 📈 查看进度 |
| `/novel:help` | 📖 显示帮助 |

---

### 🥈 Codex CLI（OpenAI · macOS/Linux）

[Codex CLI](https://github.com/openai/codex) 是 OpenAI 的命令行 AI 编程工具，可以加载 SKILL.md 来理解系统。

```bash
cd novel-writer-system
# 方式一：直接加载 SKILL.md 作为 system prompt
codex --system SKILL.md

# 方式二：先让 Codex 阅读系统说明
codex "请阅读 README.md 和 SKILL.md，然后执行 /novel:start"
```

> ⚠️ Codex CLI 基于 OpenAI 模型，对中文创作的理解力略逊于 Claude。
> 使用时建议在 prompt 中明确说明「你是一位小说创作助手」。

---

### 🥉 Cursor IDE（跨平台）

[Cursor](https://cursor.com) 是集成 AI 的代码编辑器，Agent 模式可以加载整个项目。

```bash
# 用 Cursor 打开项目目录
cursor novel-writer-system
```

**使用方法：**
1. 打开后按 `Cmd+I` (macOS) 或 `Ctrl+I` (Windows/Linux) 打开 Composer
2. 选择 **Agent** 模式
3. 输入：
   ```
   请阅读 SKILL.md，你现在是一个小说创作智能体系统。执行 /novel:start
   ```

> 💡 提示：在 Cursor 的 Rules 设置中添加 `@SKILL.md` 可以让 AI 自动加载系统配置。

---

### 🏅 Windsurf（跨平台）

[Windsurf](https://codeium.com/windsurf) 是 Codeium 推出的 AI IDE。

```bash
# 用 Windsurf 打开项目目录
windsurf novel-writer-system
```

在 Cascade 中输入：
```
请阅读 SKILL.md，启动小说创作模式 /novel:start
```

---

### 📱 ChatGPT / DeepSeek / Kimi（Web 或 App）

对于无法加载本地文件的 AI 聊天工具，可以使用**复制粘贴法**：

1. 打开项目中的 `SKILL.md`，复制全部内容
2. 粘贴到 ChatGPT/DeepSeek/Kimi 等对话中
3. 然后开始对话，例如：
   ```
   我想写一本玄幻小说，帮我规划世界观
   ```

> ⚠️ 这些工具不支持 `/novel:xxx` 命令，直接描述你的需求即可。
> 系统 Skill 文件可以作为你的 prompt 参考，告诉 AI 你的创作需求。

**推荐 Skill 文件速查：**
| 你的需求 | 参考 Skill 文件 |
|----------|----------------|
| 想搭建世界观 | `skills/00-创作全流程/worldbuilding.md` |
| 想设计角色 | `skills/00-创作全流程/character-design.md` |
| 需要大纲 | `skills/00-创作全流程/plot-outline.md` |
| 去AI味 | `skills/00-创作全流程/anti-ai-polish.md` |
| 网文开篇 | `skills/02-网文专项/webnovel-hook.md` |
| 爽点设计 | `skills/02-网文专项/webnovel-shuang.md` |

你可以对 AI 说：「请按照 `skills/00-创作全流程/worldbuilding.md` 的框架帮我搭建世界观。」

---

### 📄 纯手动阅读

所有 Skill 都是 Markdown 文件，可以直接用任何文本编辑器打开阅读。

```bash
# Linux/macOS
cat skills/00-创作全流程/worldbuilding.md | less

# Windows PowerShell
Get-Content skills\00-创作全流程\worldbuilding.md
```

---

## 🔧 系统配置说明

### Claude Code 自动加载
项目中的 `CLAUDE.md` 会在 Claude Code 启动时自动加载，无需额外配置。

### Codex CLI 配置
```bash
# 在项目目录中创建 .claude-plugin/ 目录（如果使用 Claude Code 插件系统）
mkdir -p .claude-plugin/skills
# 将需要的 skill 链接过去
```

### VSCode + Continue.dev
如果你使用 [Continue.dev](https://continue.dev) 插件，可以添加本系统作为自定义指令：
```json
{
  "commands": [
    {
      "name": "novel-start",
      "description": "启动灵境小说创作系统",
      "prompt": "请阅读项目根目录的 SKILL.md，然后执行 /novel:start"
    }
  ]
}
```

---

## 📁 项目结构

```
novel-writer-system/
├── install.ps1       # Windows 安装脚本
├── install.sh        # Linux/macOS 安装脚本
├── SKILL.md          # ✨ 入口文件 — 从这里开始
├── CLAUDE.md         # Claude Code 自动配置
├── agents/           # 🧠 7 个专业写作智能体
├── skills/           # 🧩 28 个 Skill 模块
│   ├── 00-创作全流程/  # 初始化 → 写作 → 审查 → 存档
│   ├── 01-创作技巧/    # 剧情引爆/雪花法/解耦写作
│   ├── 02-网文专项/    # 黄金三章/爽点/扫榜/投稿
│   ├── 03-质量审查/    # 一致性/质量门禁/去AI化
│   └── 04-工具集成/    # 知识图谱/记忆/进度/Obsidian
├── protocols/        # ⚙️ 核心协议与规则
├── knowledge/        # 📚 写作知识库
├── templates/        # 📄 项目模板
└── tools/            # 🔧 辅助工具
```

---

## 📜 完整命令一览（Claude Code 模式）

```
🚀 创作流程
  /novel:start      启动创作向导
  /novel:new        新建小说项目
  /novel:discuss    创作讨论 / 头脑风暴

🌍 设定管理
  /novel:world      世界观搭建
  /novel:characters 角色管理

📋 大纲规划
  /novel:outline    规划大纲
  /novel:snowflake  雪花法大纲
  /novel:save-the-cat  Save the Cat 节拍表

✍️ 写作
  /novel:write      正文写作
  /novel:decoupled  解耦写作法

🔍 质量审查
  /novel:review     章节审查
  /novel:check      一致性检查
  /novel:quality    质量门禁检查
  /novel:deslop     去AI化审查
  /novel:banned     违禁词检查
  /novel:plot-hole  漏洞检测

🎨 润色 & 技巧
  /novel:anti-ai    去AI化润色
  /novel:booming    剧情引爆（卡文救星）
  /novel:style-learn 风格学习

📦 网文专项
  /novel:hook       黄金三章 / 钩子设计
  /novel:shuang     爽点设计
  /novel:trend      扫榜 / 趋势分析
  /novel:goldfinger 金手指设计
  /novel:submit     投稿 / 平台适配

🛠️ 工具
  /novel:archive    存档与知识更新
  /novel:knowledge  知识图谱管理
  /novel:memory     记忆系统
  /novel:progress   进度追踪
  /novel:obsidian   Obsidian 同步
```

---

## 🤝 致谢

汲取自以下开源项目：

- [awesome-novel-skill](https://github.com/modoojunko/awesome-novel-skill) — 多 Agent 协作工作流
- [tianming-skill](https://github.com/zy-zmc/tianming-skill) — 天命模块化提示词工程
- [chinese-webnovel-skills](https://github.com/tance-mang/chinese-webnovel-skills) — 33 个网文 Skills 工具包
- [claude-novel-skills](https://github.com/fnb666888/claude-novel-skills) — 解耦写作法
- [story-skills](https://github.com/ati9527/story-skills) — 网文 AI Agent 工具集
- [vibe-noveling](https://github.com/TulanCN/vibe-noveling) — 网文创作工作流

---

## 📄 许可证

MIT License
