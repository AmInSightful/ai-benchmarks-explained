# Building Evaluation Datasets for AI Products

> **An evaluation dataset is a collection of real-world examples used to measure whether an AI system performs well for a specific product and user need.**

---

## 🎯 What You'll Learn

After reading this chapter, you will understand:

- Why companies need their own evaluation datasets
- What makes a good AI evaluation dataset
- How to create a golden dataset
- How to label and measure AI outputs
- How PMs can use evaluation datasets during product development

---

# Why Do Companies Need Their Own Evaluation Dataset?

Public benchmarks answer questions like:

> "How good is this model generally?"

But product teams need to answer:

> "How good is this AI feature for our users?"

These are different questions.

---

# Simple Example

Imagine building an AI customer support assistant.

A public benchmark may tell you:

```
Model A:

Excellent reasoning score
```

But your real question is:

```
Can this model correctly answer:

- Our pricing questions?
- Our refund policies?
- Our technical issues?
- Our customer complaints?
```

A company-specific dataset answers this.

---

# What Is an Evaluation Dataset?

An evaluation dataset contains:

```
User Input

+

Expected Behavior

+

Evaluation Criteria
```

Example:

```
Customer:

"I want to cancel my subscription."

Expected:

Explain cancellation process
Ask for confirmation
Avoid unauthorized actions
```

---

# The Simple Mental Model

Think about exams.

Public benchmark:

> Standardized national exam

Your evaluation dataset:

> The exact exam for your class

The second is usually more relevant.

---

# Types of Evaluation Examples

A strong dataset contains different categories.

---

# 1. Common Cases

These represent normal user behavior.

Example:

Customer asks:

> "How do I change my password?"

Expected:

Correct instructions.

---

# 2. Edge Cases

Rare situations that still matter.

Example:

Customer asks:

> "Can I transfer my account to another person after my death?"

The system needs careful handling.

---

# 3. Failure Cases

Examples where the AI previously failed.

Example:

AI gave incorrect refund information.

The example is added to prevent regression.

---

# 4. Safety Cases

Examples involving risk.

Example:

User requests:

- Private information
- Unsafe instructions
- Unauthorized actions

---

# What Makes a Good Evaluation Dataset?

A good dataset should be:

---

# Representative

It should reflect real user behavior.

Bad:

```
Artificial benchmark questions
```

Good:

```
Real customer conversations
```

---

# Diverse

Include different scenarios:

- Easy questions
- Difficult questions
- Ambiguous requests
- Rare cases

---

# High Quality

Examples should be:

- Correctly labeled
- Reviewed
- Updated

---

# Actionable

Each failure should help improve the system.

---

# Building a Golden Dataset

A golden dataset is a trusted evaluation set used repeatedly.

Process:

```
Collect Examples

↓

Clean Data

↓

Label Expected Results

↓

Review Quality

↓

Create Evaluation Set
```

---

# Step 1: Collect Real Data

Sources:

## User Conversations

Examples:

- Support chats
- Sales conversations
- Assistant interactions

---

## Product Feedback

Examples:

- User complaints
- Failed tasks
- Low ratings

---

## Internal Knowledge

Examples:

- Documents
- Policies
- Workflows

---

# Step 2: Remove Sensitive Information

Before using data:

Remove:

- Personal information
- Confidential data
- Private details

Protect user privacy.

---

# Step 3: Create Labels

Labels define what success means.

Example:

Customer support AI:

```
Question:

"How do I get a refund?"

Answer:

Correct? Yes/No

Helpful? Yes/No

Safe? Yes/No

Complete? Yes/No
```

---

# Step 4: Define Evaluation Criteria

Different products need different measures.

---

## Accuracy

Did AI provide correct information?

---

## Completeness

Did AI answer the entire request?

---

## Relevance

Did AI stay focused?

---

## Safety

Did AI avoid harmful behavior?

---

## Style

Did AI match the expected communication style?

---

# Human Evaluation

Many AI outputs cannot be judged automatically.

Humans may evaluate:

- Helpfulness
- Clarity
- Tone
- Usefulness

---

# Example Human Rating

A reviewer scores:

```
Response Quality

1 - Poor

2 - Needs improvement

3 - Acceptable

4 - Good

5 - Excellent
```

---

# Automated Evaluation

Some metrics can be measured automatically.

Examples:

## Exact Match

Did the answer match the expected output?

---

## Keyword Checking

Did the answer contain required information?

---

## Model-Based Evaluation

Another AI model evaluates the response.

Example:

"Rate this answer from 1-5 for helpfulness."

---

# The Evaluation Dataset Lifecycle

Evaluation datasets should evolve.

```
Create Dataset

↓

Launch Product

↓

Observe Failures

↓

Add New Examples

↓

Improve Dataset

↓

Repeat
```

---

# Example: Building a Coding Assistant Dataset

A coding assistant team creates:

```
1000 Developer Tasks
```

Categories:

## Code Generation

"Create a login function."

---

## Debugging

"Fix this error."

---

## Code Explanation

"Explain this module."

---

## Refactoring

"Improve this code."

---

Then they measure:

- Correctness
- Test success
- Developer acceptance

---

# Example: Building a RAG Evaluation Dataset

For an enterprise assistant:

Dataset:

```
500 Employee Questions
```

Each example contains:

```
Question

+

Relevant Documents

+

Expected Answer
```

Evaluation:

- Did retrieval find the right document?
- Did AI answer correctly?
- Did AI cite sources?

---

# Common Mistakes

---

# Mistake #1: Using Only Easy Examples

A dataset with only simple questions creates false confidence.

---

# Mistake #2: Ignoring Failures

Failures are the most valuable examples.

---

# Mistake #3: Never Updating the Dataset

User behavior changes.

Products change.

Datasets must evolve.

---

# Mistake #4: Measuring Only Accuracy

A response can be accurate but:

- Too slow
- Too expensive
- Hard to understand

---

# Product Manager Role

PMs do not need to label every example.

But PMs should define:

- User success criteria
- Important scenarios
- Business impact
- Acceptable failure levels

---

# The AI Evaluation Dataset Framework

A PM should ask:

## Question 1

"What are the most important user tasks?"

---

## Question 2

"What does success look like?"

---

## Question 3

"What failures are unacceptable?"

---

## Question 4

"How will we measure improvement?"

---

# The Mental Model

A public benchmark asks:

> "How smart is the AI generally?"

Your evaluation dataset asks:

> "Can this AI do the job our users hired it to do?"

The second question is usually more important.

---

# Key Takeaways

- Every AI product should have its own evaluation dataset.
- Real user examples are more valuable than generic tests.
- A golden dataset creates consistent measurement.
- Failure cases are essential for improvement.
- Evaluation datasets should continuously evolve.

---

# Continue Learning

Next:

➡️ [AI Product Metrics: Measuring AI Success](./ai-product-metrics.md)

Related:

- [AI Evaluation Strategy](./ai-evaluation-strategy.md)
- [RAG Evaluation](../rag/rag-evaluation.md)
- [AI Benchmark Limitations](../getting-started/benchmark-limitations.md)
