# 🧠 End-to-End Pipeline Diagnostic Template

**For AI / Data Science Decision Systems**

> **Purpose:**
> Diagnose unexpected outcomes by tracing failures to **pipeline-level assumptions**, not individual components.

---

## 1️⃣ Decision Context (Anchor First)

**Decision being supported:**

> *What action does the system influence?*

**Why this decision matters:**

* What makes it costly, irreversible, or trust-sensitive?
* Who bears the downside of mistakes?

**What success means (in decision terms):**

> *Not metrics — real-world outcomes.*

---

## 2️⃣ Observed Failure or Concern

**What is going wrong?**
(Check all that apply or describe)

* [] Rising cost
* [] Missed critical cases
* [] Uneven impact across groups
* [] Stakeholder distrust
* [] Operational overload
* [] System feels “right” but outcomes feel wrong

**How was this detected?**

* Metric movement?
* Stakeholder feedback?
* Operational signal?
* External event?

---

## 3️⃣ Forward Pipeline Reconstruction (Intent, Not Mechanics)

Describe what the system was *designed* to do at each stage.

### Data Trust

* What data was considered valid evidence?
* What data was excluded or discounted?

### Uncertainty Shaping

* Was ambiguity reduced, preserved, or ignored?
* Which kinds of noise were treated as harmless?

### Representation

* What patterns could the system “see”?
* What patterns were implicitly invisible?

### Decision Mechanism

* How did evidence become action?
* Where did discretion exist (human or automated)?

### Error Tolerance

* Which mistakes were considered acceptable?
* Which mistakes were prioritized against?

---

## 4️⃣ Backward Diagnosis (This Is the Core)

Start from the failure and reason backward.

**Where did this failure *originate*?**
(Not where it surfaced.)

Choose the *earliest* stage where a different assumption would have changed the outcome:

* [] Decision framing
* [] Data trust
* [] Uncertainty shaping
* [] Representation
* [] Decision mechanism
* [] Evaluation / thresholds

---

## 5️⃣ Violated Assumption (Name It Explicitly)

Complete this sentence:

> **“This system assumed that __________ would remain true.”**

Examples:

* user behavior would be stable
* labels represented reality
* noise was random
* cohorts were homogeneous
* costs were symmetric
* early signals were unreliable

**Why is this assumption no longer valid?**

* Environmental change?
* Business change?
* Scale change?
* Feedback loop?

---

## 6️⃣ Why the Failure Was Hard to See

**What made this failure silent?**

* [] Headline metrics masked it
* [] Aggregation hid cohort effects
* [] Thresholds constrained visibility
* [] Feedback loops reinforced behavior
* [] Trust assumptions discouraged questioning

This explains *why good teams missed it*.

---

## 7️⃣ Scope Check (Prevent Overreaction)

Before proposing changes, answer:

* Is this failure **systemic or localized**?
* Is it **temporary or structural**?
* Does it invalidate the whole pipeline or just one assumption?

This prevents panic-driven redesign.

---

## 8️⃣ (Optional) Decision-Safe Next Steps

*(Only if explicitly requested — otherwise stop at diagnosis)*

If needed:

* Which assumption would you test first?
* Which change would be lowest risk?
* What should *not* be changed yet?

---

## 🔑 One-Line Diagnostic Summary

End with:

> **“The system failed because __________, not because __________.”**

Example:

> “The system failed because we suppressed early volatility, not because the model was inaccurate.”

This sentence is gold in stakeholder conversations.

---

## How to Use This Template in Practice

* **Design reviews:**
  Run sections 1–5 *before* building anything.

* **Incidents / retrospectives:**
  Run sections 2–6 *after* something goes wrong.

* **Stakeholder alignment:**
  Use sections 1, 5, and the one-line summary.

---

## Why This Template Is Powerful

It:

* shifts blame away from models
* makes tradeoffs explicit
* preserves trust
* supports calm, senior-level reasoning
* scales across domains and tools

Most teams debug **components**.
This template debugs **systems**.

---
