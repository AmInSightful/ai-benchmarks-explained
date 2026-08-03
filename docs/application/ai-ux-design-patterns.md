# AI UX Design Patterns for Product Managers

> **AI UX design is the practice of creating user experiences that help people effectively collaborate with AI systems while understanding their capabilities and limitations.**

---

## 🎯 What You'll Learn

After reading this chapter, you will understand:

- Why AI UX is different from traditional UX
- Common AI product design patterns
- How to design trust and transparency
- When to use chat, copilot, or agent experiences
- How PMs should think about human-AI interaction

---

# Why AI UX Is Different

Traditional software is predictable.

Example:

```
Click Button

↓

Same Result Every Time
```

AI systems are probabilistic.

Example:

```
Ask Question

↓

AI Generates Response

↓

Response May Vary
```

This creates new UX challenges:

- How much should users trust AI?
- How should users correct AI?
- When should humans approve actions?
- How should uncertainty be communicated?

---

# The Core AI UX Principle

The goal is not:

> "Make AI look intelligent."

The goal is:

> "Help users accomplish their goals effectively with AI."

---

# The AI UX Framework

Good AI experiences balance:

```
Capability

+

Control

+

Trust

+

Feedback

+

Transparency
```

---

# Pattern 1: AI Assistant

## What It Is

A conversational AI that helps users complete tasks.

Examples:

- Chat assistants
- Research assistants
- Customer support bots

---

## User Experience

```
User asks

↓

AI responds

↓

User decides next action
```

---

## Best For

- Questions
- Information retrieval
- Brainstorming
- Explanations

---

## Risks

Problems:

- Users may trust incorrect answers
- Conversations can become inefficient

---

# Pattern 2: Copilot Experience

## What It Is

AI works alongside humans.

The human remains in control.

---

Examples:

- Coding assistants
- Writing assistants
- Design assistants

---

## User Experience

```
Human creates

↓

AI suggests

↓

Human edits

↓

Final output
```

---

## Why Copilots Work Well

They combine:

Human:

- Judgment
- Context
- Decision making

AI:

- Speed
- Suggestions
- Automation

---

# Pattern 3: AI Agent Experience

## What It Is

AI performs actions on behalf of users.

---

Example:

User:

> "Prepare my weekly sales report."

Agent:

```
Collect data

↓

Analyze trends

↓

Create report

↓

Send draft
```

---

## Design Challenge

Agents need more control.

Users need:

- Approval steps
- Visibility
- Ability to stop actions

---

# Pattern 4: AI Suggestions

AI provides recommendations without taking action.

Examples:

- Product recommendations
- Next best action
- Search suggestions

---

Benefits:

- Low risk
- Easy adoption
- Human control

---

# Pattern 5: AI Automation

AI completes repetitive tasks.

Examples:

- Email classification
- Document processing
- Data extraction

---

Important:

Automation requires:

- High reliability
- Clear success criteria

---

# Trust Design in AI Products

Trust is one of the most important AI UX problems.

Users ask:

> "Can I trust this?"

---

# Trust Pattern 1: Show Sources

Example:

AI answer:

```
According to:
- HR Policy Document
- Security Guidelines
```

---

Useful for:

- Enterprise AI
- Research assistants
- RAG systems

---

# Trust Pattern 2: Explain Decisions

Example:

AI recommendation:

```
Recommended because:

- Similar customers purchased this
- Price fits your budget
```

---

# Trust Pattern 3: Communicate Uncertainty

Avoid:

> "This is definitely correct."

Better:

> "Based on available information..."

---

# Trust Pattern 4: Allow Verification

Users should easily:

- Check sources
- Review changes
- Undo actions

---

# Human Control Patterns

---

# Pattern 1: Review Before Action

Useful for:

- Emails
- Financial actions
- Customer communication

Example:

```
AI drafts

↓

Human approves

↓

Action happens
```

---

# Pattern 2: Approval Thresholds

Example:

Low risk:

AI completes automatically.

High risk:

Human approval required.

---

# Pattern 3: Undo and Recovery

AI mistakes will happen.

Good products allow:

- Undo
- Edit
- Retry
- Restore

---

# Designing AI Errors

Traditional software:

Error:

> "Something went wrong."

AI errors need more context.

---

Bad:

```
I don't know.
```

---

Better:

```
I could not find reliable information.

Here are possible sources:
...
```

---

# Feedback Loops

AI products improve through user feedback.

Common patterns:

---

## Explicit Feedback

Examples:

- 👍 Helpful
- 👎 Not helpful

---

## Correction Feedback

User edits AI output.

The edit becomes valuable data.

---

## Behavioral Feedback

Observe:

- Acceptance
- Regeneration
- Abandonment

---

# AI UX Anti-Patterns

---

# Anti-Pattern 1: Fake Intelligence

Making AI appear more capable than it is.

Problem:

Creates false trust.

---

# Anti-Pattern 2: Fully Open Chat for Everything

Not every problem needs a chatbot.

Sometimes better:

- Forms
- Workflows
- Suggestions

---

# Anti-Pattern 3: No Human Escape

Users need alternatives.

Example:

"Talk to human support."

---

# Anti-Pattern 4: Hidden AI Actions

Users should know:

- What AI did
- Why it did it
- What happens next

---

# Choosing the Right AI Interaction Model

| User Need | Best Pattern |
|-|-|
| Ask questions | Assistant |
| Create content | Copilot |
| Complete tasks | Agent |
| Simple recommendations | Suggestions |
| Repetitive work | Automation |

---

# Example: AI Sales Assistant

Poor design:

```
Chat window only
```

---

Better design:

```
Customer information

↓

AI recommendations

↓

Suggested email

↓

Human approval

↓

CRM update
```

---

# PM AI UX Checklist

Before launching:

## User Goal

☐ What job is the user trying to complete?

---

## Interaction

☐ Is chat really the best interface?

---

## Trust

☐ Can users understand AI limitations?

---

## Control

☐ Can users review and correct AI?

---

## Feedback

☐ How does AI learn from users?

---

## Failure

☐ What happens when AI is wrong?

---

# The Mental Model

AI UX is not:

```
Put AI in the product

↓

Add a chat box
```

It is:

```
Understand user workflow

↓

Choose right AI interaction

↓

Design trust and control

↓

Measure outcomes

↓

Improve experience
```

---

# Key Takeaways

- AI UX is about collaboration between humans and machines.
- Chat is only one AI interface pattern.
- Trust, transparency, and control are essential.
- Copilots are often safer than full automation.
- The best AI products fit AI into existing workflows.

---

# Related Chapters

- [Copilot vs Agent vs Automation](./copilot-vs-agent-vs-automation.md)
- [AI Product Metrics](../product/ai-product-metrics.md)
- [AI Safety & Responsible AI](../product/ai-safety-responsible-ai.md)
- [Prompt Engineering for Product Managers](./prompt-engineering-for-pms.md)
