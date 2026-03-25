# 🦐 Business Data Analysis Starter

一套完整的 OpenClaw Agent 设定，开箱即用的**业务数据精密分析团队**。

给你的 Agent 发送这套文件，它会自动读取并融入自己的能力体系，无需手动配置。

## 这套东西包含什么

### 🧠 Agent 人格设定（`workspace/`）

| 文件 | 说明 |
|------|------|
| `SOUL.md` | 核心人格 — 团队 Leader 的角色定位、工作原则、上下文管理策略 |
| `IDENTITY.md` | 身份卡片 — 名称、人设、风格 |
| `AGENTS.md` | 运行规范 — Session 启动流程、记忆管理、安全边界 |
| `USER.md` | 用户画像 — 需要新用户自行填写 |
| `TOOLS.md` | 工具备忘 |
| `HEARTBEAT.md` | 心跳检查 — 任务进度监控规则 |

### 🛠️ 团队成员 Skills（`skills/`）

| 成员 | 能力 |
|------|------|
| 自动化数据分析虾 | 数据清洗、KPI 计算、差异/趋势/多维分析 |
| 历史数据比对虾 | 同比、环比、累计对比、差异归因 |
| 财务报表渲染虾 | 生成 PDF/Word/HTML 等正式报告，含专业图表 |
| 战略参谋虾 | 综合数据输出可执行的行动建议 |
| PowerPoint 制作 | 创建和编辑 PPT 演示文稿 |

## 快速上手

### 1. 前提条件

- 已安装并运行 OpenClaw
- 已有一个可用的 Agent（任何 agent 都行，它会自己融入新设定）

### 2. 环境依赖

Agent 的 Python 脚本需要以下依赖：

```bash
pip install pandas openpyxl matplotlib seaborn
```

### 3. 把文件给 Agent

把整个 `business-data-analysis-starter/` 目录放到你的 Agent 可以访问的位置，然后对 Agent 说：

> 请读取 `business-data-analysis-starter/AGENT-SETUP.md`，按照里面的指引完成接入。

Agent 会自动：
1. 读取所有设定文件
2. 将团队设定融入自己的人格体系
3. 安装 Skills
4. 引导你设置用户信息

### 4. 开始使用

接入完成后，你可以：

- 📊 **上传数据文件**，Agent 自动执行深度分析
- 📈 **多期数据对比**，同比/环比/累计一目了然
- 📋 **生成专业报告**，PDF/Word/PPT/HTML 随你选
- 🎯 **获取战略建议**，不只是数据，更是决策

## 目录结构

```
business-data-analysis-starter/
├── README.md                          ← 你正在看的这份
├── AGENT-SETUP.md                     ← Agent 接入指引（给 Agent 看的）
├── workspace/                         ← 人格设定文件
│   ├── SOUL.md
│   ├── IDENTITY.md
│   ├── AGENTS.md
│   ├── USER.md                        ← ⚠️ 使用前需填写用户信息
│   ├── TOOLS.md
│   └── HEARTBEAT.md
└── skills/                            ← 团队成员 Skills
    ├── auto-data-analysis-claw/
    ├── historical-data-compare-claw/
    ├── financial-report-render-claw/
    ├── strategy-advisor-claw/
    └── powerpoint-pptx/
```

## 自定义建议

拿到手后你可以按需修改：

- **`workspace/USER.md`** — 填写你的名字和偏好，Agent 接入时会读取
- **`workspace/IDENTITY.md`** — 不喜欢"精析队长"可以改成你想要的名字
- **`workspace/SOUL.md`** — 调整工作风格（比如要不要每步都汇报进度）
- **各 Skill 的 `SKILL.md`** — 微调每个团队成员的专业行为

## 许可

自由使用，随意修改。🦞
