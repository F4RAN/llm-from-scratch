# Words as Numbers — The Foundation (Article 1 Summary)

Computers do not understand language directly; they operate on numbers. This article explains the core idea that powers modern language models: converting words into numerical representations that preserve meaning.

## The Core Problem
A naive approach is to assign each word an ID (e.g., `"cat" = 1`, `"dog" = 2`).  
This fails because numeric IDs do not encode relationships—math on IDs produces meaningless “similarities.”

## The Breakthrough: Words as Vectors
Instead of a single ID, represent each word as a **vector**: a list of numbers (e.g., 128–4096 dimensions in real systems).  
Each vector is a point in space, and **meaning emerges from geometry**:

- Similar words end up close together
- Concepts form clusters
- Relationships become measurable using distance/angle metrics

## A 2D Intuition
To make the idea visible, the article uses a toy 2D embedding space:

- **Animals** (“cat”, “dog”) cluster in the top-right
- **Emotions** spread left–right (“hate” vs “love”)
- **Objects/food** (“pizza”, “car”) fall in the bottom half

Important note: in real embeddings, axes are not directly interpretable—what matters is **relative distance and clustering**, not the axis labels.

## What You Build (Code Walkthrough)
You implement a tiny embedding system and explore it with three steps:

1. **Define vectors** for a small vocabulary (cat, dog, love, hate, pizza, car).
2. **Measure similarity**
   - Euclidean distance: “How far apart are two points?”
   - Cosine similarity: “How aligned are two vectors?” (angle-based)
3. **Find similar words**
   - Compute cosine similarity from a target word to all others
   - Sort and return the top matches (e.g., “dog” is most similar to “cat”)
4. **Visualize the space**
   - Plot vectors on a 2D graph to show clusters forming

## Why This Matters for LLMs
This “words as vectors” concept is foundational because:

- Attention compares token vectors
- Predictions are computed from vector representations
- Higher-level behaviors (like analogies) depend on vector geometry
- Context changes meaning (e.g., “bank” in “river bank” vs “bank account”)

## Takeaways
- Word IDs are labels, not meaning
- Word vectors encode meaning through geometry
- Similarity becomes measurable (distance/angle)
- In real models, vectors are **learned from data**, not hand-coded
- This is the first building block toward sequences, attention, and transformers

## What’s Next (Article 2 Preview)
Next, the series moves from individual words to **sequences**:
Why `"I love pizza"` is not the same as `"pizza love I"`, and how models represent order using positional information.
