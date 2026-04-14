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
