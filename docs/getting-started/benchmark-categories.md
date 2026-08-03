# AI Benchmark Categories Overview

> **AI benchmarks are grouped by the capability they measure. Understanding these categories helps you choose the right evaluation for the right problem.**

---

## 🎯 What You'll Learn

After reading this chapter, you will understand:

- The major categories of AI benchmarks
- What capability each category measures
- Which benchmarks belong to each category
- Which categories matter for different AI products

---

# Why Do Benchmark Categories Matter?

AI is not one single capability.

A model can be:

- Excellent at coding
- Good at reasoning
- Average at conversation
- Weak at visual understanding

Looking at only one score gives an incomplete picture.

A useful mental model:

```
                 AI Capability

                      |
    -----------------------------------------
    |          |          |          |       |
Knowledge  Reasoning  Coding  Vision  Agents
```

Each category answers a different question.

---

# The Main AI Benchmark Categories

| Category | Main Question |
|---|---|
| Knowledge | Does the model know information? |
| Reasoning | Can the model solve complex problems? |
| Mathematics | Can the model perform advanced calculations? |
| Coding | Can the model write and fix software? |
| Multimodal | Can the model understand images and text together? |
| Long Context | Can the model process large amounts of information? |
| Agents | Can the model complete tasks using tools? |
| Safety & Reliability | Can the model behave correctly and safely? |
| Human Preference | Do people prefer its answers? |

---

# 1. Knowledge Benchmarks

## Main Question

> "Does the model know facts and concepts?"

Knowledge benchmarks test information recall and understanding.

Examples:

- History
- Science
- Law
- Medicine
- Economics
- Business

---

## Common Benchmarks

| Benchmark | What It Measures |
|---|---|
| MMLU | Broad academic knowledge |
| MMLU-Pro | More difficult professional knowledge |
| BIG-bench | Diverse language tasks |

---

## Useful For

Knowledge benchmarks matter for:

- Research assistants
- Educational products
- Enterprise search
- Information systems

---

## They Do NOT Tell You

A high knowledge score does not guarantee:

- Good reasoning
- Good writing
- Good decision making

Knowing facts is different from applying knowledge.

---

# 2. Reasoning Benchmarks

## Main Question

> "Can the model think through difficult problems?"

Reasoning benchmarks evaluate:

- Multi-step thinking
- Logical deduction
- Problem solving
- Complex analysis

---

## Common Benchmarks

| Benchmark | What It Measures |
|---|---|
| GPQA | Expert-level reasoning |
| ARC | Abstract reasoning |
| BIG-bench Hard | Difficult reasoning tasks |

---

## Useful For

Reasoning benchmarks matter for:

- Research assistants
- Decision support
- Scientific applications
- Complex analysis tools

---

## They Do NOT Tell You

A reasoning score does not automatically mean:

- Better user experience
- Better communication
- Better business outcomes

---

# 3. Mathematics Benchmarks

## Main Question

> "Can the model solve mathematical problems?"

Math benchmarks test:

- Arithmetic
- Algebra
- Geometry
- Advanced problem solving

---

## Common Benchmarks

| Benchmark | What It Measures |
|---|---|
| GSM8K | Grade-school math |
| MATH | Competition-style mathematics |
| AIME | Advanced mathematical reasoning |

---

## Useful For

- Education products
- Mathematical assistants
- Scientific computing

---

# 4. Coding Benchmarks

## Main Question

> "Can the model help developers build software?"

Coding benchmarks evaluate:

- Code generation
- Debugging
- Understanding existing code
- Software engineering workflows

---

## Common Benchmarks

| Benchmark | What It Measures |
|---|---|
| HumanEval | Code generation |
| SWE-bench | Real software engineering tasks |
| LiveCodeBench | Fresh coding problems |

---

## Useful For

- Coding assistants
- Developer tools
- Engineering automation

---

## Important Note

Writing code is different from building software.

Real software development requires:

- Understanding requirements
- Working with existing systems
- Testing
- Debugging
- Collaboration

---

# 5. Multimodal Benchmarks

## Main Question

> "Can the model understand more than text?"

Modern AI systems can process:

- Images
- Charts
- Documents
- Videos
- Audio

---

## Common Benchmarks

| Benchmark | What It Measures |
|---|---|
| MMMU | Multimodal reasoning |
| DocVQA | Document understanding |
| ChartQA | Chart interpretation |

---

## Useful For

- Document AI
- Medical imaging
- Design tools
- Visual assistants

---

# 6. Long Context Benchmarks

## Main Question

> "Can the model understand very large amounts of information?"

Long-context evaluation measures:

- Large document understanding
- Memory
- Information retrieval

---

## Common Benchmarks

| Benchmark | What It Measures |
|---|---|
| LongBench | Long-context tasks |
| Needle-in-a-Haystack | Information retrieval |

---

## Useful For

- Enterprise knowledge assistants
- Legal AI
- Research tools

---

# 7. Agent Benchmarks

## Main Question

> "Can the AI complete tasks independently?"

Agents are different from chatbots.

A chatbot:

```
Question
   ↓
Answer
```

An agent:

```
Goal
 ↓
Plan
 ↓
Use Tools
 ↓
Take Actions
 ↓
Complete Task
```

---

## Common Benchmarks

| Benchmark | What It Measures |
|---|---|
| GAIA | Real-world assistant tasks |
| AgentBench | Agent abilities |
| WebArena | Browser-based tasks |

---

## Useful For

- AI assistants
- Workflow automation
- Autonomous systems

---

# 8. Safety & Reliability Benchmarks

## Main Question

> "Can the model behave safely and reliably?"

These evaluate:

- Harmful outputs
- Bias
- Truthfulness
- Reliability

---

## Common Benchmarks

| Benchmark | What It Measures |
|---|---|
| TruthfulQA | Factual accuracy |
| HarmBench | Safety behavior |
| RealToxicityPrompts | Toxicity risk |

---

## Useful For

- Enterprise AI
- Healthcare
- Financial applications
- Public-facing products

---

# 9. Human Preference Benchmarks

## Main Question

> "Do humans prefer this model's answers?"

Some qualities are difficult to measure automatically.

Humans evaluate:

- Helpfulness
- Style
- Clarity
- Instruction following

---

## Common Examples

| Evaluation | What It Measures |
|---|---|
| LM Arena | Human preference comparisons |
| Chatbot Arena | Head-to-head model comparisons |

---

# How Categories Work Together

A real AI product usually needs multiple capabilities.

Example:

## AI Research Assistant

Needs:

```
Knowledge
    +
Reasoning
    +
Long Context
    +
Truthfulness
```

---

## Coding Assistant

Needs:

```
Coding
    +
Reasoning
    +
Long Context
    +
Instruction Following
```

---

## Customer Support Agent

Needs:

```
Knowledge
    +
Conversation
    +
Tool Use
    +
Safety
```

---

# The Product Manager Framework

When evaluating an AI capability:

Ask:

## 1. What job is the AI doing?

Example:

"Help developers write software."

---

## 2. What capability enables that job?

Example:

"Coding ability."

---

## 3. Which benchmark measures that capability?

Example:

"SWE-bench."

---

## 4. What business outcome matters?

Example:

"Developer productivity."

---

# Key Takeaways

- AI benchmarks measure different capabilities.
- No benchmark measures all of AI intelligence.
- Different products require different benchmark categories.
- Benchmark selection should start from the user problem.
- Real AI evaluation usually combines multiple benchmark types.

---

# Continue Learning

Next:

➡️ [Knowledge Benchmarks: Understanding MMLU](./knowledge/mmlu.md)

Related:

- [What Is an AI Benchmark?](../getting-started/what-is-an-ai-benchmark.md)
- [Choosing the Right AI Benchmark](../getting-started/choosing-the-right-ai-benchmark.md)
- [AI Benchmark Limitations](../getting-started/benchmark-limitations.md)
