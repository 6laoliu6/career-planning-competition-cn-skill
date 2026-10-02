# 全国大学生职业规划大赛指导 Skill

[![GitHub stars](https://img.shields.io/github/stars/6laoliu6/career-planning-competition-cn-skill?style=social)](https://github.com/6laoliu6/career-planning-competition-cn-skill/stargazers)
[![MIT License](https://img.shields.io/github/license/6laoliu6/career-planning-competition-cn-skill)](LICENSE)

![全国大学生职业规划大赛指导 Skill](assets/banner.png)

一个面向全国大学生职业规划大赛的免费开源 Codex Skill，支持成长赛道和就业赛道备赛。它会按官方评分标准帮助参赛者梳理真实经历、建立证据链，并完成或审核生涯发展报告、求职简历、展示 PPT、陈述稿、证明材料和答辩内容。

**适用关键词：** 全国大学生职业规划大赛、职规赛、成长赛道、就业赛道、生涯发展报告、求职简历、展示 PPT、答辩训练、Codex Skill、职业规划。

## 主要能力

- 判断赛道、组别、比赛层级和适用规则
- 建立“评分项—主张—证据—材料位置—缺口”矩阵
- 按评分项诊断材料、保守估分并给出具体修改动作
- 指导成长赛道的目标形成、学习实践、成果验证与动态调整
- 指导就业赛道的岗位调研、胜任力证明、求职适配与发展潜力展示
- 生成或修改报告、简历、PPT 大纲、陈述稿、证明材料目录
- 模拟评委提问，开展答辩训练和终稿一致性审查
- 区分已证实成果、待核实信息和计划目标，避免虚构经历与数据

## 评分基线

Skill 默认采用第三届全国大学生职业规划大赛（2025—2026）国家方案作为基线：

- 成长赛道：职业目标 30 分，学习实践行动 50 分，优化改进 20 分
- 就业赛道：职业目标 10 分，综合素质 40 分，专业能力 40 分，发展潜力 10 分

校赛、省赛或后续届次的通知与评分表优先于默认基线。涉及资格、材料要求、比赛流程或权重时，应以当届主办方正式文件为准。

官方参考：

- [教育部关于举办第三届全国大学生职业规划大赛的通知](https://hudong.moe.gov.cn/srcsite/A15/s7063/202510/t20251021_1417550.html)
- [全国大学生职业规划大赛平台](https://zgs.chsi.com.cn/)

## 安装

使用 Git 克隆到 Codex 的 Skills 目录：

```powershell
git clone https://github.com/6laoliu6/career-planning-competition-cn-skill.git "$HOME/.codex/skills/career-planning-competition"
```

也可以下载仓库后手动复制，并确保最终路径如下：

```text
~/.codex/skills/career-planning-competition/SKILL.md
```

安装后重新打开 Codex 会话，或在新的对话中使用。

## 使用示例

可以直接描述任务，例如：

```text
请用 career-planning-competition 帮我按成长赛道评分标准审核这份生涯发展报告。
```

```text
我要参加职业规划大赛就业赛道，目标岗位是数据分析师。请先帮我建立评分项和证据矩阵，再设计 7 分钟展示 PPT。
```

```text
请模拟国赛评委，对我的陈述稿进行追问，并指出哪些成果缺少证明材料。
```

## 文件结构

```text
全国大学生职业规划大赛指导-Skill/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── official-baseline.md
    ├── growth-track.md
    ├── employment-track.md
    ├── deliverables.md
    └── defense-and-audit.md
```

## 使用原则

- 参赛者提供的当届通知、评分表和学校要求优先。
- 所有奖项、排名、数据、访谈结论和岗位信息都应有真实依据。
- 评分时区分官方权重与内部诊断，不把自定义细分分值说成官方标准。
- 先修复报告、简历、PPT、陈述稿之间的事实冲突，再优化表达和视觉呈现。

## 参与改进

欢迎通过 Issue 提交规则更新、材料问题和改进建议。如果这个项目对你有帮助，可以点一个 Star，让更多参赛同学看到它。

## 许可证

本项目采用 [MIT License](LICENSE)。
