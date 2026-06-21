# 📚 灵境 · 小说创作智能体系统

> **LingJing** — 集多智能体协作、模块化 Skills、知识图谱于一体的 AI 小说创作系统。

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
iex "& { $(irm https://raw.githubusercontent.com/nosoultool/novel-writer-system/main/install.ps1) }"
```

### macOS / Linux
```bash
bash <(curl -s https://raw.githubusercontent.com/nosoultool/novel-writer-system/main/install.sh)
```

---

## 📖 7 种使用方式

### 🥇 Reasonix

[Reasonix](https://reasonix.dev) AI 编程代理环境，本系统已注册为内置 skill。

```bash
# 直接调用
/novel-writer 我想写一本修仙小说

# 或使用特定命令
/novel-writer /novel:world    搭建世界观
/novel-writer /novel:write    写正文
/novel-writer /novel:anti-ai  去AI化
```

> 详细用法见 [REASONIX.md](REASONIX.md)

---

### 🥇 Claude Code（全功能推荐）

```bash
cd novel-writer-system
claude
# 输入 /novel:start
```

支持全部 `/novel:xxx` 命令。

---

### 🥈 Codex CLI

```bash
codex --system SKILL.md
```

---

### 🥉 Cursor IDE

用 Cursor 打开项目目录，在 Composer 中选择 Agent 模式，输入 `/novel:start`。

---

### 🏅 Windsurf

用 Windsurf 打开项目目录，在 Cascade 中输入「请阅读 SKILL.md，启动小说创作模式」。

---

### 📱 ChatGPT / DeepSeek / Kimi

复制 `SKILL.md` 内容粘贴到对话中，然后直接描述你的创作需求。

---

### 📄 手动阅读

```bash
cat skills/00-创作全流程/worldbuilding.md
```

---

## 📁 项目结构

```
novel-writer-system/
├── install.ps1         Windows 安装脚本
├── install.sh          Linux/macOS 安装脚本
├── SKILL.md            入口文件
├── CLAUDE.md           Claude Code 配置
├── REASONIX.md         Reasonix 使用指南
├── agents/             7 个写作智能体
├── skills/             28 个 Skill 模块
│   ├── 00-创作全流程/
│   ├── 01-创作技巧/
│   ├── 02-网文专项/
│   ├── 03-质量审查/
│   └── 04-工具集成/
├── protocols/          核心协议
├── knowledge/          写作知识库
└── templates/          项目模板
```

---

## 📜 完整命令一览

```
🚀 创作流程
  /novel:start      启动创作向导
  /novel:discuss    创作讨论

🌍 设定管理
  /novel:world      世界观搭建
  /novel:characters 角色管理

📋 大纲
  /novel:outline    规划大纲
  /novel:snowflake  雪花法

✍️ 写作
  /novel:write      正文写作
  /novel:decoupled  解耦写作

🔍 审查
  /novel:review     章节审查
  /novel:check      一致性检查
  /novel:quality    质量门禁
  /novel:deslop     去AI审查
  /novel:plot-hole  漏洞检测

🎨 润色
  /novel:anti-ai    去AI化
  /novel:booming    剧情引爆
  /novel:style-learn 风格学习

📦 网文
  /novel:hook       黄金三章
  /novel:shuang     爽点设计
  /novel:trend      扫榜分析
  /novel:goldfinger 金手指
  /novel:submit     投稿适配

🛠️ 工具
  /novel:archive    存档更新
  /novel:knowledge  知识图谱
  /novel:memory     记忆系统
  /novel:progress   进度追踪
```

---

## 🙏 致谢

汲取自：awesome-novel-skill / tianming-skill / chinese-webnovel-skills / claude-novel-skills / story-skills / vibe-noveling

---

## 📄 许可证 · MIT
