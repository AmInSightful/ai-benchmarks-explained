# Fine-Tuning vs RAG vs Prompt Engineering: Choosing the Right AI Approach

> **Prompt engineering, RAG, and fine-tuning are different ways to improve AI systems. The right choice depends on whether you need better instructions, more knowledge, or different behavior.**

---

## 🎯 What You'll Learn

After reading this chapter, you will understand:

- The difference between prompts, RAG, and fine-tuning
- When to use each approach
- The trade-offs between speed, cost, and control
- How PMs should make AI architecture decisions

---

# The Core Question

When an AI product does not perform well, ask:

> "What exactly needs to improve?"

Possible answers:

1. The AI does not understand the task.
2. The AI does not have the right information.
3. The AI does not behave in the desired way.

Each problem requires a different solution.

---

# The Three Main Approaches

```
Prompt Engineering

↓

RAG

↓

Fine-Tuning
```

They solve different problems.

---

# Approach 1: Prompt Engineering

## What Is Prompt Engineering?

Changing the instructions given to the model.

---

Example:

Basic:

```
Summarize this document.
```

Improved:

```
Summarize this document for a CEO.

Include:
- Key insights
- Risks
- Recommendations

Use simple language.
```

---

# When to Use Prompt Engineering

Use prompts when you need:

- Better instructions
- Better output format
- Different response style

---

Examples:

## Customer Support

Need:

More polite answers.

Solution:

Improve prompt.

---

## Data Extraction

Need:

Structured output.

Solution:

Define JSON format.

---

# Advantages

Benefits:

- Fast
- Cheap
- Easy to test
- No model changes

---

# Limitations

Does not solve:

- Missing information
- Lack of domain knowledge
- Complex behavior changes

---

# Approach 2: RAG (Retrieval-Augmented Generation)

## What Is RAG?

RAG gives AI access to external information before answering.

---

Without RAG:

```
Question

↓

AI Model

↓

Answer
```

---

With RAG:

```
Question

↓

Search Knowledge

↓

Retrieve Relevant Information

↓

AI Model

↓

Answer
```

---

# Example

Question:

> "What is our company's refund policy?"

---

Without RAG:

AI may guess.

---

With RAG:

AI retrieves:

```
Company Refund Policy Document

↓

Creates Answer
```

---

# When to Use RAG

Use RAG when AI needs:

- Private company information
- Updated knowledge
- Domain-specific documents

---

Examples:

## Enterprise Assistant

Need:

Answer questions from internal documents.

Solution:

RAG.

---

## Customer Support AI

Need:

Use company policies.

Solution:

RAG.

---

# Advantages

Benefits:

- Uses current information
- Reduces hallucinations
- Easier updates

---

# Limitations

Challenges:

- Retrieval quality matters
- Documents must be clean
- More system complexity

---

# Approach 3: Fine-Tuning

## What Is Fine-Tuning?

Fine-tuning trains an existing model on additional examples to change its behavior.

---

Example:

General model:

Writes normally.

---

Fine-tuned model:

Writes like a company's brand voice.

---

# When to Use Fine-Tuning

Use fine-tuning when you need:

- Specific behavior
- Consistent style
- Specialized task performance

---

Examples:

## Legal Document Generation

Need:

Specific legal writing style.

Solution:

Fine-tuning.

---

## Classification

Need:

Consistent category decisions.

Solution:

Fine-tuning.

---

# Advantages

Benefits:

- More consistent behavior
- Specialized performance
- Can reduce prompt complexity

---

# Limitations

Challenges:

- Requires training data
- More expensive
- Requires maintenance

---

# The Simple Decision Tree

Ask these questions:

---

## Question 1:

Does AI lack information?

Example:

"The model does not know our company policies."

Solution:

```
RAG
```

---

## Question 2:

Does AI understand information but answer incorrectly?

Example:

"The response format is wrong."

Solution:

```
Prompt Engineering
```

---

## Question 3:

Does AI need a different behavior?

Example:

"Always write like a financial analyst."

Solution:

```
Fine-Tuning
```

---

# Comparison Table

| Approach | Solves | Example |
|-|-|-|
| Prompt Engineering | Better instructions | Better summaries |
| RAG | Missing knowledge | Company Q&A |
| Fine-Tuning | Behavior changes | Brand-specific writing |

---

# Cost Comparison

Generally:

## Prompt Engineering

Lowest cost.

---

## RAG

Medium cost.

Requires:

- Data pipeline
- Retrieval system

---

## Fine-Tuning

Higher cost.

Requires:

- Training data
- Training process
- Maintenance

---

# Speed Comparison

Fastest:

```
Prompt Engineering
```

↓

Medium:

```
RAG
```

↓

Slowest:

```
Fine-Tuning
```

---

# Example: Building an AI Sales Assistant

Goal:

Help sales teams answer customer questions.

---

## Option 1: Prompt Engineering

Instruction:

"You are a helpful sales assistant."

Problem:

No company knowledge.

---

## Option 2: RAG

Connect:

- Product documentation
- Pricing information
- Customer policies

Better solution.

---

## Option 3: Fine-Tuning

Train AI on:

Thousands of successful sales conversations.

Useful for:

Consistent communication style.

---

# Common Mistakes

---

# Mistake 1: Fine-Tuning Too Early

Many teams fine-tune before trying simpler solutions.

Better order:

```
Prompt

↓

RAG

↓

Fine-tuning
```

---

# Mistake 2: Using RAG for Everything

RAG does not fix:

- Poor instructions
- Wrong behavior

---

# Mistake 3: Using Prompts for Knowledge

A prompt cannot replace a knowledge system.

---

Example:

Bad:

"Remember all company documents."

Better:

Use RAG.

---

# Mistake 4: Ignoring Data Quality

RAG and fine-tuning both depend on good data.

---

# PM Decision Framework

Before choosing an approach:

## Problem

☐ What exactly is failing?

---

## Knowledge

☐ Does AI need external information?

---

## Behavior

☐ Does AI need a different style?

---

## Complexity

☐ Is the improvement worth the engineering effort?

---

## Measurement

☐ How will we know it improved?

---

# The AI Improvement Ladder

Most teams should start here:

```
1. Improve Prompt

↓

2. Add Better Context

↓

3. Add RAG

↓

4. Improve Data Pipeline

↓

5. Fine-Tune Model

↓

6. Build Custom Model
```

---

# The Mental Model

Choosing between prompt, RAG, and fine-tuning is not:

```
Which technology is most advanced?
```

It is:

```
What problem are we solving?

↓

What is the simplest effective solution?

↓

How do we measure improvement?
```

---

# Key Takeaways

- Prompt engineering improves instructions.
- RAG improves access to knowledge.
- Fine-tuning changes model behavior.
- Start with the simplest solution.
- Most AI products need good prompts and RAG before fine-tuning.
- The best architecture depends on the product problem.

---

# Related Chapters

- [Prompt Engineering for Product Managers](./prompt-engineering-for-pms.md)
- [RAG Architecture](../architecture/rag-architecture.md)
- [AI Product Metrics](../product/ai-product-metrics.md)
- [AI Technical Concepts for PMs](../fundamentals/ai-concepts-for-pms.md)
