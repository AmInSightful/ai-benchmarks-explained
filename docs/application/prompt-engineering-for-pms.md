# Prompt Engineering for Product Managers

> **Prompt engineering is the process of designing instructions and context that guide AI models to produce useful, reliable, and consistent outputs.**

---

## 🎯 What You'll Learn

After reading this chapter, you will understand:

- What prompts actually do
- Why prompts affect AI product quality
- Different prompt patterns
- How PMs should think about prompt design
- How to evaluate and improve prompts

---

# What Is a Prompt?

A prompt is the input given to an AI model.

It tells the model:

- What task to perform
- What information to use
- What format to return
- What constraints to follow

---

Example:

Simple prompt:

```
Write an email.
```

Better prompt:

```
Write a professional email declining a meeting invitation.

Audience:
Senior executive

Tone:
Polite and concise

Length:
Under 100 words
```

The second prompt gives clearer guidance.

---

# The Simple Explanation

Think of AI like a smart employee.

A weak instruction:

> "Prepare a report."

A better instruction:

> "Prepare a monthly sales report for executives. Include revenue trends, risks, and three recommendations."

The employee will produce a better result because the request is clearer.

---

# Why PMs Should Care About Prompts

Prompts influence:

- Product quality
- User experience
- AI reliability
- Cost
- Safety

A small prompt change can significantly change AI behavior.

---

# Prompt Components

A production AI prompt usually contains several parts:

```
Role

+

Task

+

Context

+

Instructions

+

Examples

+

Output Format
```

---

# 1. Role

Defines who the AI should behave as.

Example:

```
You are a customer support specialist.
```

---

Why it helps:

The model understands the expected perspective.

---

# 2. Task

Defines what needs to be done.

Example:

```
Summarize this customer complaint.
```

---

Weak:

```
Analyze this.
```

Strong:

```
Identify the customer's main issue,
sentiment, and recommended next action.
```

---

# 3. Context

Provides relevant information.

Example:

```
The customer is a premium enterprise customer.
```

Without context:

AI may produce generic answers.

---

# 4. Instructions

Define rules.

Examples:

```
Use simple language.

Do not invent information.

Ask questions when information is missing.
```

---

# 5. Examples

Examples teach the expected pattern.

This is called:

## Few-Shot Prompting

---

Example:

Input:

```
Customer is angry about delayed delivery.
```

Output:

```
Category: Delivery Issue
Priority: High
```

Then provide a new example.

---

# 6. Output Format

Defines how the response should look.

Example:

```
Return JSON:

{
 "summary":"",
 "priority":"",
 "next_action":""
}
```

---

# Prompt Types

---

# Zero-Shot Prompting

No examples.

Example:

```
Translate this text into French.
```

Useful for:

- Simple tasks
- General requests

---

# Few-Shot Prompting

Provide examples.

Example:

```
Classify these customer messages:

Example 1:
Message: "I forgot password"
Category: Account

Example 2:
Message: "Payment failed"
Category: Billing
```

Useful for:

- Classification
- Structured outputs

---

# Chain-of-Thought (High Level)

Some tasks require multi-step reasoning.

Example:

Complex question:

```
A company has 20% growth for three years.
What is the final growth?
```

The model benefits from reasoning through steps.

---

Important:

For product teams:

You usually evaluate the final answer, not expose private reasoning.

---

# Prompt Templates

Production AI systems rarely use one fixed prompt.

They use templates.

Example:

```
You are a sales assistant.

Customer:
{{customer_message}}

Company information:
{{knowledge}}

Provide:
{{required_output}}
```

---

# Why Prompt Templates Matter

They allow:

- Consistency
- Testing
- Version control
- Experimentation

---

# Prompt Versioning

Prompts should be managed like software.

Example:

Version 1:

```
Answer customer questions.
```

---

Version 2:

```
Answer customer questions using company policy.
If information is unavailable, say so.
```

---

Then compare:

- Quality
- Cost
- User feedback

---

# Prompt Evaluation

A good prompt should be tested.

Do not ask:

> "Does this prompt look good?"

Ask:

> "Does this prompt improve outcomes?"

---

# Evaluation Dimensions

## Accuracy

Does AI produce correct answers?

---

## Consistency

Does it behave similarly?

---

## Format Compliance

Does it follow requirements?

---

## Cost

Does it require too many tokens?

---

## Latency

Does it respond quickly enough?

---

# Example: Customer Support Prompt Improvement

## Version 1

```
Answer the customer question.
```

Problem:

- Generic answers
- Hallucinations

---

## Version 2

```
You are a customer support agent.

Use only the provided company knowledge.

If information is missing, ask for clarification.

Include:
1. Answer
2. Next step
3. Source
```

Improvement:

- Better accuracy
- Better trust
- Easier evaluation

---

# Prompt Engineering vs Product Engineering

Prompt engineering alone does not solve everything.

A product needs:

```
Good Prompt

+

Good Data

+

Good Retrieval

+

Good UX

+

Good Evaluation
```

---

# Common Prompt Mistakes

---

# Mistake #1: Being Too Vague

Bad:

```
Make this better.
```

Better:

```
Rewrite this email to sound professional and concise.
```

---

# Mistake #2: Adding Too Many Instructions

More instructions do not always improve results.

Too much complexity can confuse the model.

---

# Mistake #3: Ignoring Real User Inputs

A prompt that works in demos may fail with real users.

Test:

- Different languages
- Different user styles
- Edge cases

---

# Mistake #4: Treating Prompts as Permanent

AI models change.

Prompts need continuous improvement.

---

# PM Prompt Checklist

Before launching an AI feature:

## Goal

☐ What user problem does this solve?

---

## Instructions

☐ Are instructions clear?

---

## Context

☐ Does AI have enough information?

---

## Output

☐ Is the expected format defined?

---

## Evaluation

☐ How will we measure quality?

---

## Failure

☐ What happens when AI is wrong?

---

# The Mental Model

Prompt engineering is not:

```
Finding magic words

↓

Getting perfect AI answers
```

It is:

```
Define desired behavior

↓

Provide useful context

↓

Create constraints

↓

Evaluate results

↓

Improve continuously
```

---

# Key Takeaways

- Prompts are product design tools.
- Clear instructions improve AI performance.
- Production prompts need testing and versioning.
- Prompt quality alone cannot replace good data and architecture.
- PMs should treat prompts as part of the product experience.

---

# Related Chapters

- [AI UX Design Patterns](./ai-ux-design-patterns.md)
- [Fine-Tuning vs RAG vs Prompt Engineering](./fine-tuning-vs-rag-vs-prompts.md)
- [AI Product Experimentation](../product/ai-product-experimentation.md)
- [AI Evaluation Strategy](../product/ai-evaluation-strategy.md)
