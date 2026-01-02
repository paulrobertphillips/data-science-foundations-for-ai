# 🎓 Capstone — Artifact 2

## **Pipeline Design (Decision-First)**

*(Modules 2–4)*

> **Goal:** Show that every pipeline choice is **intentionally shaped by the decision**, not by modeling convenience.

You are designing a **decision system**, not a data pipeline.

---

## Context Reminder (Locked from Artifact 1)

* **Decision:**
  Prioritize assets for proactive inspection or maintenance in the next planning window.

* **Decision Owner:**
  Human engineers retain final authority.

* **Risk Profile:**

  * False negatives → catastrophic failure
  * False positives → wasted budget and capacity
  * Signals are noisy and heterogeneous

Do **not** re-litigate this — design from it.

---

## What You Will Produce

You will produce **four sections**, each short but explicit.

---

## Section 1 — Data Trust Boundaries

Describe **what counts as acceptable evidence** and what does not.

Answer in bullets:

* What kinds of data are trusted as *directional signals*?
* What kinds of data are explicitly **not** treated as ground truth?
* Where is human judgment required to contextualize data?

❌ No data schemas
❌ No sources list unless conceptually important

---

## Section 2 — Uncertainty Shaping Strategy

Describe how uncertainty is handled **by design**.

Answer:

* What ambiguity is intentionally **preserved**?
* What ambiguity (if any) is intentionally **suppressed**?
* Why does this align with the risk profile of the decision?

This is a **values choice**, not a technical one.

---

## Section 3 — Representation & Feature Concepts

Describe **feature concepts**, not features.

For each (2–4 total):

* What behavior or condition does it make visible?
* What assumption does it encode?

Examples (do not copy):

* “Deviation from historical baseline”
* “Frequency of minor anomalies”
* “Time since last inspection relative to peers”

❌ No formulas
❌ No importance ranking

---

## Section 4 — Modeling Stance

Take a clear position.

Choose **one**:

* Modeling is justified
* Modeling is not justified (rules / heuristics instead)
* Modeling is conditionally justified

Then explain:

* Why this stance fits the decision risk
* What modeling *will not* be allowed to do
* What role humans retain regardless

You may explicitly reject modeling options here — that is a strength.

---

## Rules (Important)

❌ No algorithms
❌ No metrics
❌ No thresholds
❌ No “we’ll figure this out later”

✅ Intentional constraints
✅ Decision-aligned reasoning
✅ Explicit rejections

---

## Response Format (Use This)

```
Capstone — Artifact 2

1. Data trust boundaries:
- …

2. Uncertainty shaping strategy:
- …

3. Representation & feature concepts:
- Feature concept 1:
  - Makes visible:
  - Assumption:
- Feature concept 2:
  - Makes visible:
  - Assumption:
(etc.)

4. Modeling stance:
- Position:
- Rationale:
- Explicit constraints / rejections:
```

---

## How I’ll Review This

I’ll be looking for:

* internal consistency with Artifact 1
* whether uncertainty is treated intentionally
* whether representation choices encode the right worldview
* whether modeling restraint is justified, not reflexive

This artifact is where **most weak systems quietly fail** — take your time.

When you’re ready, send your **Artifact 2 submission**, and I’ll review it as a design review, not a homework assignment.
