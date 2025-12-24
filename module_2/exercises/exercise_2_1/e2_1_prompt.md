# 🧪 Module 2 Mini-Exercise — Competing Cleaning Strategies

We will **reuse the same input** you analyzed in Module 1:

> **Historical churn labels (classified as heuristic, low-confidence)**

Your task is **not** to find the “right” strategy — it’s to surface **tradeoffs**.

---

## Step 1 — Define Two Conflicting Cleaning Strategies

Create **two plausible but incompatible approaches**:

### 🔹 Strategy A — *Aggressively Reduce Noise*

Intent example (you can adapt):

* remove ambiguous labels
* collapse edge cases
* enforce stricter definitions of churn

### 🔹 Strategy B — *Preserve Ambiguity*

Intent example:

* keep uncertain labels
* encode uncertainty explicitly
* accept messiness to avoid false certainty

You don’t need implementation details — just intent.

---

## Step 2 — For *Each* Strategy, Answer These Three Questions

For **Strategy A** *and* **Strategy B**, answer:

1. **What assumption does this strategy make about churn?**
   (What must be true for this to be safe?)

2. **What bias does this strategy introduce?**
   (Who or what does it favor or suppress?)

3. **When would this strategy be *dangerous*?**
   (What kind of real-world situation would it fail badly in?)

Be explicit. No hedging.

---

## Rules (Important)

❌ No models
❌ No metrics
❌ No “best practices”
❌ No fixing both sides

✅ Tradeoffs only
✅ Decision-linked reasoning
✅ Honest failure modes

---

## Why This Matters

Senior data scientists are not judged by:

> “Did they clean the data well?”

They are judged by:

> **“Did they choose the *right kind of wrong* for this decision?”**

---

## What I’ll Do After You Reply

I’ll:

* surface hidden assumptions
* show how AI would *interpret* each strategy
* identify which risks are being accepted vs ignored
* connect this directly to **feature engineering choices in Module 3**

When you’re ready, reply with:

* **Strategy A** (short description + 3 answers)
* **Strategy B** (short description + 3 answers)

Take your time — this exercise is meant to stretch judgment, not speed.
