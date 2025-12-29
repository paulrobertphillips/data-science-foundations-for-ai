# 🧪 Module 3 Mini-Exercise — Feature Engineering as Constraint Selection

We’ll continue using the **same churn scenario** and the **Strategy A vs Strategy B lens** you’ve already built.

> **Reminder:**
> You are not designing “good features.”
> You are choosing **what the system is allowed to notice**.

---

## Step 1 — Propose Three Candidate Features

Come up with **three plausible features** derived from any of:

* usage logs
* billing / tenure data
* support interactions

Keep them **conceptual**, not mathematical.

Examples of acceptable granularity:

* “Recent change in weekly usage”
* “Time since last support interaction”
* “Deviation from typical usage baseline”

❌ No formulas
❌ No metrics
❌ No modeling talk

---

## Step 2 — For *Each* Feature, Answer These Three Questions

For **each feature**, explicitly answer:

### 1️⃣ What relationship does this feature make visible?

* What behavior or pattern does the model now get to “see”?

### 2️⃣ What assumption does this feature encode?

* What must be true about the world for this feature to be meaningful?

### 3️⃣ What risk does this feature introduce?

Choose one or more:

* leakage risk
* shortcut learning
* bias amplification
* false confidence
* timing sensitivity
* intervention feedback

Be concrete — name the risk.

---

## Step 3 — Strategy Alignment Check (Critical)

For each feature, add **one line**:

* Does this feature align more with **Strategy A (stability / precision)**
  **or** **Strategy B (sensitivity / early warning)**?
* Why?

This forces you to acknowledge that **features are policy choices**.

---

## Rules (Important)

❌ Do not propose “balanced” features
❌ Do not hedge (“it depends”)
❌ Do not fix risks

✅ Explicit assumptions
✅ Explicit risks
✅ Clear strategy alignment

---

## What I’ll Do After You Reply

I’ll review your features by:

* identifying hidden leakage or timing risks
* showing how each feature *constrains* model behavior
* calling out where representation quietly encodes decisions
* connecting this directly to **Module 4 (Modeling as Constraint Satisfaction)**

---

## When You’re Ready

Reply with:

```
Feature 1:
- Relationship:
- Assumption:
- Risk:
- Strategy alignment:

Feature 2:
- Relationship:
- Assumption:
- Risk:
- Strategy alignment:

Feature 3:
- Relationship:
- Assumption:
- Risk:
- Strategy alignment:
```

Take your time — this exercise is where representation turns into power.
