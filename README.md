<p align="center">
  <img src="https://img.shields.io/github/stars/real-ljs/paper-deep-reading-skill?style=social" alt="GitHub stars">
  <img src="https://img.shields.io/github/license/real-ljs/paper-deep-reading-skill" alt="License">
  <img src="https://img.shields.io/badge/version-1.0.0-blue" alt="Version">
  <img src="https://img.shields.io/badge/platform-Claude%20Code%20%7C%20Cursor%20%7C%20Continue-purple" alt="Platforms">
</p>

<h1 align="center">📖 Paper Deep Reading Skill</h1>

<p align="center">
  <strong>不只是「读」论文，而是「读懂」论文。</strong>
</p>

<p align="center">
  一个系统化的学术论文精读 Skill，帮助你还原作者的问题意识、方法设计逻辑、证据链和适用边界。<br/>
  适用于 AI / ML / NLP / LLM 领域研究者、工程师和学生。
</p>

---

## 🧭 为什么需要这个 Skill？

读论文时，你是否有过这些困扰：

- 读完摘要和结论，就觉得「懂了」，但讲不清楚方法到底怎么运作；
- 陷入公式和实验表格，看不清论文的主线逻辑；
- 分不清作者「证明了什么」和「声称了什么」；
- 写论文笔记时不知道从何下手，只能摘抄原文。

**这个 Skill 就是为此设计的。** 它提供了一套完整的精读框架，让你从「被动阅读」变成「主动解构」。

---

## ✨ 核心特性

<table>
  <tr>
    <td width="50%">
      <h4>🔗 因果链阅读法</h4>
      <p>将论文从「现实背景 → 核心问题 → 方法设计 → 实验验证 → 结论局限」读成一条完整的论证链条。</p>
    </td>
    <td width="50%">
      <h4>🧩 四层方法拆解</h4>
      <p>从方法总览、模块分工、算法流程到关键设计理由，逐层深入理解方法。</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h4>📊 实验结构化分析</h4>
      <p>主实验、消融实验、Case Study — 每种实验都有对应的拆解模板和分析问题。</p>
    </td>
    <td width="50%">
      <h4>✅ 精读自检清单</h4>
      <p>读完论文后，用 11 个问题检查自己是否真正读懂。</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h4>📝 标准化输出模板</h4>
      <p>从论文基本信息到方法细节、实验结果、局限与个人理解，11 个模块完整覆盖。</p>
    </td>
    <td width="50%">
      <h4>🎯 批判性思维</h4>
      <p>区分「事实」「论证」「推测」三类信息，培养对论文的批判性阅读能力。</p>
    </td>
  </tr>
</table>

---

## 📦 快速开始

### 安装

#### Claude Code

```bash
# 克隆本仓库
git clone https://github.com/real-ljs/paper-deep-reading-skill.git

# 将 skill 添加到 Claude Code
cp -r skills/paper-deep-reading ~/.claude/skills/
```

#### Cursor

```bash
# 克隆本仓库
git clone https://github.com/real-ljs/paper-deep-reading-skill.git

# 将 SKILL.md 的内容复制到 .cursor/rules/ 目录下
mkdir -p .cursor/rules
cp skills/paper-deep-reading/SKILL.md .cursor/rules/paper-deep-reading.md
```

#### Continue (VS Code / JetBrains)

将 `skills/paper-deep-reading/SKILL.md` 的内容配置为 Continue 的系统提示词或规则文件。

### 使用

```
请使用 paper-deep-reading skill 帮我精读这篇论文：[论文内容/链接/arXiv ID]
```

或者直接发送论文 PDF 或 URL，AI 会自动按照精读框架展开分析。

---

## 📖 Skill 概览

### 三大阅读原则

| # | 原则 | 说明 |
|:---:|:---|:---|
| 1 | **先读问题，再读方法** | 不陷入细节，先搞清论文想解决什么问题 |
| 2 | **把论文读成因果链** | 每一节都在论证链条中扮演角色 |
| 3 | **区分证明与声称** | 辨认事实、论证、推测三类信息 |

### 八步精读流程

```
快速定位 → 一句话摘要 → 拆任务背景 → 拆论文动机
    → 拆核心方法(四层) → 拆实验设计 → 拆结论局限 → 自检清单
```

### 六问精读法

每篇论文都要回答：

1. 它研究的**任务**是什么？
2. 为什么这个任务**重要**？
3. 已有方法为什么**不够**？
4. 作者提出了什么**新方法**？
5. 实验如何证明方法**有效**？
6. 真正**贡献**在哪里，又有什么**局限**？

---

## 🗂 仓库结构

```
paper-deep-reading-skill/
├── README.md                           # 本文件
├── LICENSE                             # MIT License
├── CONTRIBUTING.md                     # 贡献指南
├── skills/
│   └── paper-deep-reading/
│       └── SKILL.md                    # Skill 定义文件
└── examples/
    └── example-output.md               # 精读输出示例
```

---

## 📋 输出模板

精读完论文后，Skill 会引导你输出以下结构化笔记：

```
论文精读笔记
├── 1. 论文基本信息
├── 2. 一句话总结
├── 3. 任务背景
├── 4. 研究动机
├── 5. 方法总览
├── 6. 方法细节（模块逐一拆解）
├── 7. 实验设计
├── 8. 主要结果
├── 9. 为什么有效
├── 10. 局限
└── 11. 我的理解与批判性思考
```

---

## 🤝 贡献

欢迎贡献！你可以：

- **提交新的 Skill 变体** — 针对特定领域（如 CV、系统、理论）的精读变体；
- **改进现有 Skill** — 优化框架、补充模板、修正错误；
- **分享使用案例** — 提交你用这个 Skill 做的精读笔记；
- **翻译** — 提供其他语言的版本。

详见 [CONTRIBUTING.md](./CONTRIBUTING.md)。

---

## 🌟 社区

如果这个 Skill 对你有帮助，请给一个 ⭐ Star！

- 💬 **提问 & 讨论**：[GitHub Issues](https://github.com/real-ljs/paper-deep-reading-skill/issues)
- 📬 **联系作者**：[GitHub @real-ljs](https://github.com/real-ljs)

---

## 📄 License

MIT License © 2025 [real-ljs](https://github.com/real-ljs)

---

<p align="center">
  <sub>精读论文 = 还原作者的问题意识、方法设计逻辑、证据链和适用边界。</sub>
</p>