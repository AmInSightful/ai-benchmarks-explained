# AI Build vs Buy Decision Framework

> **The build vs buy decision determines whether a company should create custom AI capabilities internally or use existing AI platforms, models, and tools.**

---

## 🎯 What You'll Learn

After reading this chapter, you will understand:

- Why build vs buy is different for AI products
- When companies should use existing AI models
- When customization creates strategic value
- How to evaluate AI vendors
- How PMs should make AI architecture decisions

---

# Why Build vs Buy Matters More in AI

In traditional software:

Building internally often means:

- More control
- More customization
- Higher development effort

Buying means:

- Faster deployment
- Lower initial investment

---

AI adds new considerations:

- Model capability changes quickly
- AI infrastructure is expensive
- Data can create differentiation
- AI vendors evolve rapidly

---

# The Core Question

The wrong question:

> "Can we build this ourselves?"

---

The better question:

> "Where can we create unique value that competitors cannot easily copy?"

---

# The AI Capability Stack

Modern AI products usually contain multiple layers:

```
Application Layer

↓

Workflow Layer

↓

AI System Layer

↓

Model Layer

↓

Infrastructure Layer
```

---

Different layers may have different build/buy decisions.

---

# Layer 1: Foundation Models

Examples:

- Large language models
- Vision models
- Speech models

---

Usually:

BUY

---

Why?

Because training foundation models requires:

- Massive datasets
- Expensive infrastructure
- Specialized research teams

---

# Layer 2: AI Infrastructure

Examples:

- Model hosting
- Monitoring
- Deployment systems

---

Decision:

Depends on scale.

---

Early stage:

Buy.

---

Large AI companies:

Build more internally.

---

# Layer 3: AI Application Logic

Examples:

- Workflows
- Agents
- User experience
- Business rules

---

This is often where companies differentiate.

---

Usually:

BUILD.

---

# Layer 4: Data Advantage

Examples:

- Customer data
- Industry knowledge
- Proprietary information

---

Often:

BUILD.

---

Data can become a competitive advantage.

---

# The AI Build vs Buy Matrix

| Capability | Usually Better Choice |
|-|-|
| Foundation model | Buy |
| AI APIs | Buy |
| Generic chatbot | Buy/Customize |
| Company knowledge assistant | Build |
| Industry workflow automation | Build |
| Proprietary AI experience | Build |

---

# When to Buy

Use existing AI solutions when:

---

## 1. The Capability Is Not Differentiating

Example:

Adding:

"AI email summary"

to a productivity app.

---

Users care about:

The workflow.

Not the underlying model.

---

## 2. Speed Matters

Buying enables:

- Faster experiments
- Faster launches
- Lower risk

---

## 3. The Technology Changes Quickly

AI models improve rapidly.

Building today may become outdated.

---

# When to Build

Build when AI creates strategic advantage.

---

## 1. Unique Customer Experience

Example:

An AI system deeply integrated into a company's workflow.

---

## 2. Proprietary Data Advantage

Example:

A financial company using unique market data.

---

## 3. Specialized Requirements

Examples:

- Industry-specific reasoning
- Compliance needs
- Security requirements

---

## 4. Economics at Scale

At high usage:

Building may reduce long-term costs.

---

# Customization Options

AI customization is not binary.

There are levels:

```
Use API

↓

Prompt Engineering

↓

RAG

↓

Fine-Tuning

↓

Custom Model

```

---

# Level 1: API Usage

Example:

Use a general AI model.

---

Best for:

- Fast experiments
- Common use cases

---

# Level 2: Prompt Engineering

Change instructions.

---

Best for:

- Output style
- Formatting
- Behavior adjustments

---

# Level 3: RAG

Connect AI to company knowledge.

---

Best for:

- Enterprise assistants
- Search
- Documentation

---

# Level 4: Fine-Tuning

Train model on examples.

---

Best for:

- Specialized behavior
- Consistent outputs

---

# Level 5: Custom Model

Build your own model.

---

Best for:

- Unique capabilities
- Very large scale
- Strategic advantage

---

# Vendor Evaluation Framework

When buying AI capabilities, evaluate:

---

# 1. Quality

Questions:

- How accurate is the model?
- Does it solve our problem?

---

# 2. Cost

Questions:

- What is cost per request?
- How does cost scale?

---

# 3. Reliability

Questions:

- Is service stable?
- Are there uptime guarantees?

---

# 4. Security

Questions:

- How is data handled?
- Are there privacy controls?

---

# 5. Flexibility

Questions:

- Can we switch models?
- Are we locked in?

---

# 6. Strategic Fit

Questions:

- Does this create advantage?
- Or does everyone have the same capability?

---

# The AI Vendor Lock-In Problem

Using external AI creates dependency.

Risks:

- Price changes
- API changes
- Product direction changes

---

# Mitigation:

Design systems with flexibility:

```
Application

↓

AI Layer

↓

Multiple Model Options
```

---

# Example Decision

## Problem:

Build AI customer support assistant.

---

Option A:

Build custom model.

Cost:

Very high.

Time:

Long.

---

Option B:

Use existing model + RAG.

Cost:

Lower.

Time:

Faster.

---

Better approach:

Start with:

```
Existing Model

+

RAG

+

Good UX
```

Then customize if needed.

---

# Common Build vs Buy Mistakes

---

# Mistake 1: Building Models Too Early

Many companies build before proving value.

---

# Mistake 2: Buying Without Differentiation Strategy

Using the same AI capability as competitors creates no advantage.

---

# Mistake 3: Ignoring Data

Data is often more valuable than the model.

---

# Mistake 4: Optimizing Technology Instead of Outcomes

The goal is:

Better customer results.

Not:

Better AI architecture.

---

# PM Decision Checklist

Before choosing:

## Customer Value

☐ What problem are we solving?

---

## Differentiation

☐ Does this create unique advantage?

---

## Speed

☐ How quickly do we need results?

---

## Economics

☐ What is the long-term cost?

---

## Data

☐ Do we have unique data?

---

## Risk

☐ What dependencies are created?

---

# The Mental Model

AI build vs buy is not:

```
Build everything

or

Buy everything
```

---

It is:

```
Buy commodity capabilities

+

Build strategic differentiation
```

---

# Key Takeaways

- Most companies should buy foundation models.
- Differentiation usually comes from data, workflows, and user experience.
- AI customization exists on a spectrum.
- Speed and learning matter during early stages.
- Build where AI creates competitive advantage.
- Buy where AI is a commodity.

---

# Related Chapters

- [AI Product Strategy Framework](./ai-product-strategy-framework.md)
- [AI Product Roadmapping](./ai-product-roadmapping.md)
- [AI Product Economics](../business/ai-product-economics.md)
- [AI Platform Strategy](../platform/ai-platform-strategy.md)
