# AI Concepts Every Product Manager Should Know

> **AI PMs do not need to build models, but they need to understand how AI systems work to make better product decisions.**

---

## 🎯 What You'll Learn

After reading this chapter, you will understand:

- How modern AI systems work at a high level
- Key AI concepts explained simply
- Important trade-offs in AI products
- How to communicate with technical teams

---

# The AI System Overview

A modern AI product usually looks like:

```
User

↓

Application

↓

AI Logic

↓

Model

↓

Infrastructure
```

---

Example:

AI customer support assistant:

```
Customer Question

↓

Product Interface

↓

Retrieve Company Information

↓

AI Model Generates Answer

↓

Response to Customer
```

---

# 1. AI Model

## What Is a Model?

A model is a system trained to recognize patterns and generate outputs.

Think of it as:

> A very advanced pattern recognition engine.

---

Example:

A language model learns patterns from:

- Text
- Code
- Documents
- Conversations

Then uses those patterns to generate responses.

---

# Simple Analogy

A model is like a person who has read millions of books.

The person does not memorize every sentence.

They learn patterns:

- Language
- Concepts
- Relationships

---

# 2. Training

## What Is Training?

Training is the process where an AI model learns from data.

Example:

```
Large Dataset

↓

Learning Process

↓

AI Model
```

---

During training, the model learns:

- Patterns
- Relationships
- Representations

---

# Training Analogy

Teaching a student:

Input:

Thousands of examples.

Learning:

Finding patterns.

Result:

Ability to solve new problems.

---

# 3. Inference

## What Is Inference?

Inference is when a trained model is used to generate an answer.

Training:

```
Learning phase
```

Inference:

```
Using phase
```

---

Example:

Training:

Model learns language.

---

Inference:

User asks:

"Explain AI benchmarks."

Model answers.

---

# Product Importance

Inference affects:

- Speed
- Cost
- User experience

---

# 4. Tokens

## What Is a Token?

AI models do not read text exactly like humans.

They process smaller pieces called tokens.

---

Example:

Sentence:

```
AI is powerful
```

May become:

```
AI

is

power

ful
```

(tokens are not always words)

---

# Why Tokens Matter

Tokens affect:

## Cost

More tokens:

Higher cost.

---

## Speed

More tokens:

Longer processing time.

---

## Context

More tokens:

More information the model can consider.

---

# 5. Context Window

## What Is Context Window?

The amount of information an AI model can consider at one time.

---

Example:

Small context:

```
Short conversation
```

Large context:

```
Long documents

+

Conversation history
```

---

# Product Impact

Larger context enables:

- Document analysis
- Longer conversations
- More complex tasks

---

Trade-off:

More context can increase:

- Cost
- Latency

---

# 6. Parameters

## What Are Parameters?

Parameters are internal values learned during training.

They represent what the model has learned.

---

Simple analogy:

Human brain:

Millions of connections.

AI model:

Millions or billions of learned parameters.

---

# Do More Parameters Always Mean Better AI?

No.

A larger model may be:

- More capable
- More expensive
- Slower

A smaller optimized model may be better for some products.

---

# 7. Embeddings

## What Are Embeddings?

Embeddings convert information into numbers that represent meaning.

---

Example:

Words:

```
King

Queen
```

are represented as numerical patterns.

---

The model understands that:

```
King

and

Queen
```

are related concepts.

---

# Why Embeddings Matter

Used in:

- Search
- Recommendations
- RAG systems

---

# Example

User searches:

> "How do I reset my password?"

Embedding search finds:

> "Account recovery instructions"

because they have similar meaning.

---

# 8. Vector Databases

## What Are Vector Databases?

A database designed to store and search embeddings.

---

Traditional database:

Search exact values.

Example:

```
Customer ID = 123
```

---

Vector database:

Search similar meaning.

Example:

```
Find documents related to password recovery
```

---

# Why They Matter

They enable:

- AI search
- Knowledge assistants
- RAG applications

---

# 9. RAG (Retrieval-Augmented Generation)

## What Is RAG?

RAG gives AI access to external information before generating an answer.

---

Without RAG:

```
User Question

↓

AI Model

↓

Answer
```

---

With RAG:

```
User Question

↓

Search Relevant Information

↓

AI Model

↓

Answer Using Information
```

---

# Why RAG Matters

It helps with:

- Accuracy
- Enterprise knowledge
- Up-to-date information

---

# 10. Fine-Tuning

## What Is Fine-Tuning?

Fine-tuning adapts a model using additional training data.

---

Example:

General model:

Writes normally.

---

Fine-tuned model:

Writes like a specific brand.

---

# Fine-Tuning Is Good For:

- Style adaptation
- Specialized behavior
- Specific tasks

---

# Fine-Tuning Is Not Good For:

Adding constantly changing information.

For that:

Use RAG.

---

# 11. Temperature

## What Is Temperature?

A setting controlling how predictable or creative model outputs are.

---

Low temperature:

More consistent.

Example:

Data extraction.

---

High temperature:

More creative.

Example:

Brainstorming.

---

# Product Examples

Customer support:

Lower temperature.

Creative writing:

Higher temperature.

---

# 12. Latency

## What Is Latency?

The time AI takes to respond.

---

Users care about:

```
Waiting Time
```

---

AI latency depends on:

- Model size
- Prompt length
- Infrastructure
- Processing complexity

---

# 13. Model Size

Models come in different sizes.

---

Large Models:

Advantages:

- More capability

Disadvantages:

- Higher cost
- Slower

---

Small Models:

Advantages:

- Faster
- Cheaper

Disadvantages:

- Lower capability

---

# Product Decision

The best model is not always the biggest model.

It is:

> The model that creates the best user value at acceptable cost.

---

# 14. Multimodal AI

## What Is Multimodal AI?

AI that understands multiple types of information.

Examples:

- Text
- Images
- Audio
- Video

---

Example:

User uploads image:

AI explains what is shown.

---

# 15. AI Agents

## What Are Agents?

Systems that can:

- Understand goals
- Plan steps
- Use tools
- Take actions

---

Example:

Instead of:

"Here is a sales report template."

Agent:

"Here is the completed sales report."

---

# How These Concepts Connect

A modern AI product:

```
User

↓

Application

↓

Prompt

↓

RAG / Tools

↓

Model

↓

Inference

↓

Output
```

---

# PM Technical Checklist

When discussing an AI feature, ask:

## Model

☐ Which model is used?

---

## Data

☐ What information does AI access?

---

## Context

☐ How much information does it need?

---

## Cost

☐ How expensive is each interaction?

---

## Quality

☐ How do we evaluate output?

---

## Risk

☐ What happens when AI fails?

---

# Common PM Mistakes

---

# Mistake 1: Thinking Bigger Models Always Win

Product value matters more than model size.

---

# Mistake 2: Ignoring Cost

AI usage creates variable costs.

---

# Mistake 3: Confusing RAG and Fine-Tuning

RAG:

Adds knowledge.

Fine-tuning:

Changes behavior.

---

# Mistake 4: Ignoring User Experience

A powerful model can still create a bad product.

---

# The Mental Model

AI PMs do not need to become ML engineers.

They need to understand:

```
What AI can do

+

How AI fails

+

What trade-offs exist

+

How to create user value
```

---

# Key Takeaways

- Models learn patterns from data.
- Training creates models; inference uses them.
- Tokens affect cost and speed.
- Embeddings enable semantic search.
- RAG adds knowledge to AI systems.
- Fine-tuning changes behavior.
- Bigger models are not always better.
- AI PMs need enough technical knowledge to make good product decisions.

---

# Related Chapters

- [Fine-Tuning vs RAG vs Prompt Engineering](../application/fine-tuning-vs-rag-vs-prompts.md)
- [RAG Architecture](../architecture/rag-architecture.md)
- [AI Agent Architecture](../architecture/agent-architecture.md)
- [AI Product Metrics](../product/ai-product-metrics.md)
