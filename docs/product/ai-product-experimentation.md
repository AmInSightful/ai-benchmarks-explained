# AI Product Experimentation: How to Run AI A/B Tests

> **AI experimentation is the process of measuring whether AI capabilities improve user outcomes compared with existing experiences.**

---

## 🎯 What You'll Learn

After reading this chapter, you will understand:

- Why AI experimentation is different from traditional software testing
- How to design AI product experiments
- The difference between offline and online evaluation
- Important AI experiment metrics
- How PMs should measure incremental AI value

---

# Why AI Products Need Experimentation

A common mistake:

> "The AI model is better, so the product must be better."

This is not always true.

A better model can fail because:

- Users do not understand it
- It is too slow
- It is too expensive
- Users do not trust it
- It does not solve the real problem

Product experiments answer:

> "Does this AI capability create better outcomes for users?"

---

# Traditional Product Experimentation

A typical software A/B test:

```
Users

↓

Random Assignment

↓

Version A vs Version B

↓

Measure Outcome
```

Example:

Version A:

Existing search

Version B:

AI-powered search

Measure:

- Conversion
- Retention
- Engagement

---

# Why AI Experiments Are Different

AI outputs are not deterministic.

Example:

Same question:

```
"What laptop should I buy?"
```

Response 1:

Different answer

Response 2:

Different answer

Response 3:

Different answer

---

Therefore, AI experiments must measure:

- Output quality
- User behavior
- Business impact

---

# The AI Experimentation Framework

A strong AI experiment has four layers:

```
AI Quality

+

User Experience

+

Business Impact

+

Risk / Safety
```

---

# Layer 1: Define the Hypothesis

Every experiment starts with a clear hypothesis.

Bad:

> "AI will improve the product."

Good:

> "AI recommendations will increase checkout conversion by helping users choose products faster."

---

# Example Hypotheses

## Customer Support

"AI assistance will reduce resolution time without lowering satisfaction."

---

## Coding Assistant

"AI suggestions will reduce developer task completion time."

---

## Search Product

"AI summaries will improve successful searches."

---

# Layer 2: Choose the Control Group

A/B tests require comparison.

Example:

## Control Group

Users receive:

```
Current experience
```

---

## Treatment Group

Users receive:

```
AI-powered experience
```

---

The difference shows AI's incremental value.

---

# Layer 3: Select Metrics

AI experiments need multiple metric types.

---

# Primary Metrics

The main success measure.

Examples:

## Support AI

Resolution rate

---

## Search AI

Successful search completion

---

## Writing AI

Time saved

---

# Secondary Metrics

Additional indicators.

Examples:

- Engagement
- Retention
- Feature usage

---

# Guardrail Metrics

Metrics that prevent harmful optimization.

Examples:

- Customer complaints
- Error rate
- Cost increase
- Safety incidents

---

# Example:

AI support improves:

Resolution rate:

+20%

But:

Customer satisfaction:

-15%

The experiment is not successful.

---

# Offline vs Online Evaluation

AI teams use both.

---

# Offline Evaluation

Before exposing users.

```
Historical Data

↓

AI System

↓

Measure Quality
```

---

Examples:

- Test datasets
- Human review
- Benchmark comparison

---

Benefits:

- Fast
- Safe
- Repeatable

---

Limitations:

May not represent real user behavior.

---

# Online Evaluation

With real users.

```
Real Users

↓

AI Feature

↓

Measure Outcomes
```

---

Examples:

- A/B tests
- Beta programs
- User feedback

---

Benefits:

Measures real impact.

---

Limitations:

- More risk
- Requires monitoring

---

# Example: AI Search Experiment

A company adds AI summaries.

---

## Hypothesis

AI summaries help users find answers faster.

---

## Experiment

Control:

Traditional search results

---

Treatment:

Search + AI summary

---

## Measure

Primary:

Task completion rate

---

Secondary:

- Search time
- User satisfaction

---

Guardrails:

- Incorrect answers
- Support complaints

---

# AI-Specific Experiment Metrics

---

# Acceptance Rate

How often users accept AI suggestions.

Example:

Writing assistant:

```
100 suggestions

↓

60 accepted

↓

60% acceptance
```

---

# Correction Rate

How often users modify AI output.

High correction may indicate:

- Low trust
- Poor quality

---

# Regeneration Rate

How often users ask AI to retry.

Example:

User clicks:

"Generate again"

Repeatedly.

---

# Human Override Rate

How often users ignore AI recommendations.

Important for:

- Decision systems
- Agents

---

# Cost Per Successful Outcome

A very important business metric.

Example:

AI completes:

1000 tasks

Cost:

$100

Successful tasks:

500

Cost per success:

$0.20

---

# AI Experiment Design Challenges

---

# Challenge 1: Measuring Quality Automatically

Some AI qualities are subjective.

Examples:

- Creativity
- Helpfulness
- Tone

Solutions:

- Human evaluation
- User feedback
- Model-based evaluation

---

# Challenge 2: Sample Size

AI improvements may be small.

Need enough users to detect impact.

---

# Challenge 3: Learning Effects

Users may improve as they learn AI tools.

Example:

A coding assistant may become more valuable after developers understand how to use it.

---

# Challenge 4: Trust Effects

A poor early experience can permanently reduce adoption.

---

# AI Experimentation Mistakes

---

# Mistake #1: Measuring Usage Only

High usage does not mean high value.

Users may use AI because they have no alternative.

---

# Mistake #2: Ignoring Quality

More AI interactions can create more mistakes.

---

# Mistake #3: No Baseline Comparison

Always ask:

> "Better than what?"

---

# Mistake #4: Optimizing One Metric

Example:

Reducing response time but increasing wrong answers.

Balance metrics.

---

# PM AI Experiment Checklist

Before running an experiment:

## Problem

☐ What user problem are we solving?

---

## Hypothesis

☐ What improvement do we expect?

---

## Comparison

☐ What is the control experience?

---

## Metrics

☐ What defines success?

---

## Safety

☐ What could go wrong?

---

## Decision

☐ What happens if results are positive or negative?

---

# The AI Product Experiment Loop

```
Identify Problem

↓

Create Hypothesis

↓

Build AI Experience

↓

Evaluate Offline

↓

Run User Experiment

↓

Measure Impact

↓

Improve
```

---

# The Mental Model

AI experimentation is not:

```
Launch AI Feature

↓

Check Usage
```

It is:

```
Define User Value

↓

Test AI Capability

↓

Measure Outcomes

↓

Balance Quality, Cost, Risk

↓

Improve Continuously
```

---

# Key Takeaways

- AI experiments measure value, not just model quality.
- A/B testing remains important for AI products.
- AI experiments need quality, business, and safety metrics.
- Offline evaluation and online experiments work together.
- The goal is better user outcomes, not more AI usage.

---

# Related Chapters

- [AI Product Metrics](./ai-product-metrics.md)
- [AI Evaluation Strategy](./ai-evaluation-strategy.md)
- [Building Evaluation Datasets](./building-evaluation-datasets.md)
- [Evaluating AI Agents](../agents/evaluating-ai-agents.md)
