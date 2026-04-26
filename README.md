认可 [LINUX DO](https://linux.do/) 社区

# backend-interviewer

## 项目简介

`backend-interviewer` 是一个面向后端工程师的项目式模拟面试 Skill。  
它会基于你的真实项目背景进行多轮追问、结构化评分，并给出可执行的提升建议。

### 适用技术场景

- Java / Spring Boot
- Go / 微服务
- MySQL / Redis / MQ
- 云原生 / 稳定性 / 性能优化

---

## 项目声明

> 本项目初始版本由 **OpenAI Codex** 生成，并由仓库维护者整理发布与维护。

---

## 核心能力

- 项目化面试：围绕真实项目问，不做纯八股。
- 多轮追问：根据回答质量动态加深问题。
- 结构化评分：6 个维度量化评估（1-5 分）。
- 结果导向反馈：输出风险点、改进优先级、2 周训练计划。

---

## 面试流程

1. 收集项目上下文（角色、架构、规模、职责）
2. 选择模式（`full-loop` / `focus-topic` / `pressure-mode`）
3. 分轮提问（项目深挖 → 架构设计 → 性能并发 → 安全上线）
4. 生成最终报告（评分 + 改进建议 + 训练计划）

---

## 快速开始

### 方式一：安装脚本（推荐）

```powershell
& "$env:USERPROFILE\AppData\Local\Programs\Python\Launcher\py.exe" `
"$env:USERPROFILE\.codex\skills\.system\skill-installer\scripts\install-skill-from-github.py" `
--repo Ban-code-art/backend-interviewer-skill `
--path . `
--name backend-interviewer
```

安装后请重启 Codex。

---

### 方式二：手动安装

复制仓库到：

```bash
~/.codex/skills/backend-interviewer
```

然后重启 Codex。

---

## 使用示例

### 中文

```text
用 $backend-interviewer 基于我的项目做一场资深后端模拟面试，完整4轮，最后给评分和改进计划。
```

### English

```text
Use $backend-interviewer to run a senior backend mock interview for my project and give targeted feedback.
```

---

## 评分维度

- Project Ownership
- System Design
- Performance / Concurrency
- Database / Consistency
- Security / Reliability
- Communication / Trade-off Reasoning

详见：

```text
references/evaluation-rubric.md
```

---

## 仓库结构

```text
backend-interviewer-skill/
├─ SKILL.md
├─ agents/
│  └─ openai.yaml
├─ references/
│  ├─ project-intake-template.md
│  ├─ question-bank.md
│  └─ evaluation-rubric.md
├─ LICENSE
└─ README.md
```

---

## 开源许可

本项目使用：

```text
./LICENSE
```

---

## 致谢

- OpenAI Codex
- 使用并反馈改进建议的开发者
