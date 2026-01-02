# 🎓 Capstone — Artifact 3

## **Evaluation & Policy Choices**

*(Module 5)*

> **Goal:** Demonstrate that you can translate decision values and risk tolerance into **explicit evaluation criteria and threshold policies** — without hiding behind metrics.

This is where many systems quietly encode values they never intended to.

---

## Context Reminder (Locked)

From Artifacts 1 & 2:

* **Decision:**
  Prioritize assets for proactive inspection or maintenance.

* **Risk Profile:**

  * False negatives → catastrophic failure
  * False positives → wasted budget and capacity

* **Pipeline Stance:**

  * All data is heuristic
  * Uncertainty is preserved
  * Rule-based / constrained decision mechanism
  * Humans retain final authority

Do **not** contradict these assumptions.

---

## What You Will Produce

You will produce **four sections**.

---

## Section 1 — Chosen Evaluation Metrics

Select **2–3 evaluation metrics** and, for each, explain:

* What behavior this metric *rewards*
* What behavior it *punishes*
* Why it fits this decision context

Focus on **decision consequences**, not statistical definitions.

Examples (do not copy):

* Recall
* Coverage
* Time-to-detection
* Stability over time
* Alert volume consistency

❌ No formulas
❌ No model comparison framing

---

## Section 2 — Hidden Failure Modes of Your Metrics

For **each metric**, answer:

* How could optimizing this metric mislead decision-makers?
* What failure might look like “success” under this metric?

This is where maturity shows.

---

## Section 3 — Threshold Strategy (Policy Choice)

Choose **one thresholding strategy** and describe it as **policy**:

Examples:

* Capacity-constrained
* Risk-tolerance based
* Tiered review
* Human-gated escalation

Then explain:

* What constraint this threshold enforces
* What risk it explicitly accepts

This must align with **limited maintenance capacity**.

---

## Section 4 — Explicitly Rejected Options

Explicitly reject:

* at least **one evaluation metric**
* at least **one threshold strategy**

For each rejection:

* state *why* it is inappropriate
* tie the rejection back to decision risk

Rejecting things well is a strength.

---

## Rules (Important)

❌ No accuracy / AUC
❌ No “best performing” language
❌ No optimization framing
❌ No thresholds as “tuning knobs”

✅ Metrics as value judgments
✅ Thresholds as policy
✅ Explicit tradeoffs

---

## Response Format (Use This)

```
Capstone — Artifact 3

1. Chosen evaluation metrics:
- Metric 1:
  - Rewards:
  - Punishes:
  - Why appropriate:
- Metric 2:
  - Rewards:
  - Punishes:
  - Why appropriate:
(etc.)

2. Hidden failure modes:
- Metric 1:
  - Hidden failure:
- Metric 2:
  - Hidden failure:
(etc.)

3. Threshold strategy:
- Strategy:
- Constraint enforced:
- Risk accepted:

4. Explicitly rejected options:
- Rejected metric:
  - Reason:
- Rejected threshold strategy:
  - Reason:
```

---

## How I’ll Review This

I’ll assess:

* whether your metrics encode the *right* values
* whether your threshold policy is realistic and defensible
* whether your rejections are principled
* whether your choices align with Artifacts 1 & 2

This artifact is where **many otherwise good systems fail** — take your time.

When you’re ready, send your **Artifact 3 submission**, and I’ll review it as a policy review, not a metrics review.
