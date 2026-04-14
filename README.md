# CIE A2 经济学 Paper 4 作文生成器

一个 Claude Code skill，用于生成 **CIE 9708 A2 经济学 Paper 4** 的考试级作文，严格遵循 **AO1/AO2/AO3** 评分标准。

---

## 这个 Skill 能做什么

这个 skill 可以写出 20 分经济学作文，质量达到剑桥官方范文水平。它专门解决 AI 生成作文常见的丢分问题：

* **逻辑链不完整**：从原因直接跳到结果，没有中间步骤。
* **评价过于浅显**：泛泛地说 “it depends” 而不说明具体取决于什么。
* **缺少图表整合**：没有一步一步解释图表。
* **结论薄弱**：只是重述题目而没有权衡论点。

---

## 主要功能

* ✅ **精准的 AO1 定义**：所有经济学概念都给出准确定义。
* ✅ **完整的 AO2 分析**：包含至少 3 步的因果传导机制。
* ✅ **具体的 AO3 评价**：使用时间、弹性、经济状态、政府失灵等具体维度。
* ✅ **详细的图表描述**：包含坐标轴、曲线、移动、均衡点、福利区域等。
* ✅ **有权重的结论**：综合论点而不是简单重复题目。
* ✅ **自我检查清单**：提交前可验证作文质量。

---

## 安装方法

### 前置要求
* 已安装 [Claude Code](https://claude.ai/code)
* 对 CIE 9708 A2 经济学大纲有基本了解

### 安装步骤
1.  **克隆本仓库**：
    ```bash
    git clone https://github.com/CLFY521/cie-a2-essay-writer.git
    ```
2.  **将 skill 复制到 Claude Code 的 skills 目录**：
    ```bash
    cp -r cie-a2-essay-writer ~/.claude/skills/
    ```

3.  **重要：准备参考语料库（`references/` 文件夹）** 本 skill 需要高质量的 CIE 9708 Paper 4 范文才能发挥最佳效果。请在仓库中创建 `references/` 文件夹，并放入以下文件：
    * `model-essays.md` （至少 6 篇覆盖主要主题的范文）
    * `AO3_EVALUATION_ANGLES.md` （按主题整理的评价角度数据库）
    * `TOPIC_INDEX.md` （主题与范文对应索引）

> **参考材料来源建议**：
> * 你自己的高分练习作文
> * 老师提供的范文
> * 市面上的 CIE 9708 范文书籍
> * 剑桥官网的过去试卷考官报告

---

## 使用方法

安装完成后，当你执行以下操作时，技能会自动激活并生成高质量作文：
1.  粘贴一道 CIE A2 经济学作文题目。
2.  让 Claude “写”、“起草”或“回答”经济学作文。
3.  提到相关经济概念（通胀、市场失灵、垄断等）。

**示例：**
> **用户**：Discuss whether a monopoly is always against the public interest. [20]  
> **Claude**：生成一篇完整的、符合考试标准的 20 分作文（包含 AO1/AO2/AO3 结构）。

---

## 作文结构（强制执行）

每篇作文都严格按照以下结构生成：

1.  **[AO1] 知识与理解**（150-250 字）
2.  **[AO2] 分析**（300-500 字）—— 完整因果链 + 图表描述
3.  **[AO3] 评价**（250-400 字）—— 使用具体评价维度
4.  **结论**（80-150 字）—— 有权重的判断

---

## 覆盖主题

* 市场失灵与外部性
* 市场结构（垄断、寡头、完全竞争）
* 全球化与国际贸易
* 宏观经济政策（货币、财政、供给侧）
* 无差异曲线与消费者理论
* 劳动力市场
* 经济增长与发展
* 汇率
* 国际收支

---

## 为什么要做这个 Skill

作为 CIE A2 经济学学生，我发现普通 AI 生成的作文经常因为以下问题丢分：
* 分析跳步
* 评价模糊
* 图表整合不当
* 结论无力

因此我根据高分范文结构开发了这个 skill，帮助生成更接近剑桥标准的作文。

---

## 局限性

* 本 skill 提供的是**框架和方法论**，不能替代你对经济学的理解。
* 你仍需**验证事实准确性**并根据具体题目调整。
* 效果最好时需要提供**高质量的参考范文**。
* 生成的作文请务必**自己阅读理解后再使用**。

---

## 贡献

欢迎贡献！如果你有：
* 更多高质量范文（请确保有权限）
* 更好的 AO 结构改进
* 更丰富的评价角度数据库
* Bug 修复或功能增强

欢迎提交 Issue 或 Pull Request。

---

## 免责声明

本 skill **仅供教育用途**，旨在帮助学生：
* 理解高分作文的特点
* 学习正确的 AO1/AO2/AO3 结构
* 练习撰写考试级答案

**请勿用于**：
* 在正式考试中提交 AI 生成的内容作为自己的作品
* 违反学校学术诚信政策
* 取代真正的学习过程

目标是帮助你**学会自己写出更好的作文**，而非绕过学习。

# CIE A2 Economics Paper 4 Essay Writer

A Claude Code skill that generates exam-grade essays for CIE 9708 A2 Economics Paper 4, following strict AO1/AO2/AO3 marking criteria.

## What This Skill Does

This skill writes 20-mark economics essays that match the quality of official Cambridge model answers. It addresses the common problem where AI-generated essays lose marks due to:

- **Incomplete logic chains** (jumping from cause to effect without intermediate steps)
- **Shallow evaluation** (generic "it depends" without specifying what it depends on)
- **Missing diagram integration** (not explaining diagrams step-by-step)
- **Weak conclusions** (restating the question instead of weighing arguments)

## Features

- ✅ **Precise AO1 definitions** for all economic terms
- ✅ **Complete AO2 analysis** with full transmission mechanisms (minimum 3-step causal chains)
- ✅ **Specific AO3 evaluation** using concrete dimensions (time, elasticity, economic state, government failure, etc.)
- ✅ **Detailed diagram descriptions** (axes, curves, shifts, equilibria, welfare areas)
- ✅ **Weighted conclusions** that synthesize arguments rather than repeat the question
- ✅ **Self-critique checklist** to verify essay quality before submission

## Installation

### Prerequisites

- [Claude Code](https://claude.ai/code) installed
- Basic understanding of CIE 9708 A2 Economics syllabus

### Setup

1. Clone this repository:
```bash
git clone https://github.com/YOUR_USERNAME/cie-a2-essay-writer.git
```

2. Copy the skill to your Claude Code skills directory:
```bash
cp -r cie-a2-essay-writer ~/.claude/skills/
```

3. **IMPORTANT: Prepare your reference corpus**

This skill requires a reference corpus of CIE 9708 Paper 4 model essays to function optimally. You need to create a `references/` folder with:

```
cie-a2-essay-writer/
├── SKILL.md
└── references/
    ├── model-essays.md          # 6+ exemplar essays covering key topics
    ├── AO3_EVALUATION_ANGLES.md # Database of evaluation dimensions by topic
    └── TOPIC_INDEX.md           # Index mapping topics to relevant essays
```

**Where to get reference materials:**
- Your own high-scoring practice essays
- Teacher-provided model answers
- Commercially available CIE 9708 model answer books
- Past paper examiner reports (available on Cambridge website)

**Reference file format examples:**

`model-essays.md`:
```markdown
## Essay 1: Market Failure and Externalities

**Question:** Discuss whether government intervention can correct market failure caused by negative externalities. [20]

**Model Answer:**
[Full essay text...]

---

## Essay 2: Monopoly vs Perfect Competition
...
```

`AO3_EVALUATION_ANGLES.md`:
```markdown
# Evaluation Angles by Topic

## Market Failure
- Time dimension (short run vs long run)
- Government failure risk
- Information asymmetry
- Magnitude of intervention
...

## Inflation
- Type of inflation (demand-pull vs cost-push)
- Elasticity of demand/supply
- Economic cycle stage
...
```

## Usage

Once installed, the skill activates automatically when you:

1. Paste a CIE A2 Economics essay question
2. Ask Claude to "write", "draft", or "answer" an economics essay
3. Provide a question mentioning economic concepts (inflation, market failure, monopoly, etc.)

**Example:**

```
User: Discuss whether a monopoly is always against the public interest. [20]

Claude: [Generates full exam-grade essay with AO1/AO2/AO3 structure]
```

## Essay Structure

Every essay follows this mandatory structure:

1. **[AO1] Knowledge & Understanding** (150-250 words)
   - Precise definitions of all key terms
   - Theoretical framework setup

2. **[AO2] Analysis** (300-500 words)
   - Complete causal chains (minimum 3 steps)
   - Detailed diagram descriptions if required
   - Full transmission mechanisms

3. **[AO3] Evaluation** (250-400 words)
   - Specific evaluative dimensions (time, elasticity, type, magnitude, etc.)
   - Counter-arguments with "However..."
   - Real-world relevance

4. **Conclusion** (80-150 words)
   - Weighted judgement
   - Conditional synthesis
   - No simple restatement

## Topics Covered

- Market failure & externalities
- Market structures (monopoly, oligopoly, perfect competition)
- Globalisation & international trade
- Macroeconomic policies (monetary, fiscal, supply-side)
- Indifference curves & consumer theory
- Labour markets
- Economic growth & development
- Exchange rates
- Balance of payments

## Why This Skill Was Built

As a CIE A2 Economics student, I noticed that generic AI answers consistently lost marks because they:
- Skipped logical steps in analysis
- Used vague evaluation ("it depends on circumstances")
- Didn't integrate diagrams properly
- Had weak conclusions

After analyzing the structure of high-scoring model essays, I built this skill to replicate the exact patterns that Cambridge examiners reward.

## Limitations

- This skill provides a **framework and methodology**, not a substitute for understanding economics
- You still need to **verify factual accuracy** and adapt answers to specific question wording
- The skill works best when you provide a **quality reference corpus** of model essays
- Always **review and understand** the generated essay before using it for revision

## Contributing

Contributions welcome! If you have:
- Additional model essays to share (with proper permissions)
- Improvements to the AO structure
- Better evaluation angle databases
- Bug fixes or enhancements

Please open an issue or submit a pull request.

## License

MIT License - see LICENSE file for details

## Disclaimer

This skill is for **educational purposes only**. It's designed to help students:
- Understand what makes a high-quality economics essay
- Learn proper AO1/AO2/AO3 structure
- Practice writing exam-grade answers

**Do not use this to:**
- Submit AI-generated work as your own in actual exams
- Violate your school's academic integrity policies
- Replace genuine learning and understanding

The goal is to help you **learn how to write better essays yourself**, not to bypass the learning process.

---

Built by a CIE A2 Economics student using Claude Code. If you find this helpful, consider starring the repo or sharing it with other economics students who might benefit.
