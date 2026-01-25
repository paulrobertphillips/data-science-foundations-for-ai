# 📄 Data Science Project Kickoff Checklist

*A senior-practitioner tool for decision-first, low-rework project starts*

> **Purpose:** Ensure early decisions align the entire pipeline before any irreversible choices are made.

You do **not** need all answers perfectly.
You **do** need them explicitly acknowledged.

---

## 1️⃣ Decision Being Supported (Required)

**Decision statement:**

> *We are deciding **[action]** under **[constraints]** with uncertainty about **[unknowns]***.

**Who makes this decision?**

* [] Human
* [] System
* [] Hybrid
  Role / team: ______________________

**Decision frequency:**

* [] One-time
* [] Periodic
* [] Continuous

🔴 **Red flag:** “We’re not sure yet — we just want insights.”

---

## 2️⃣ Why This Decision Matters (Risk Surface)

**If the decision is wrong, what happens?**
[] Financial cost
[] Trust / credibility loss
[] Opportunity cost
[] Compliance / reputational risk
[] Other: ______________________

**Which mistake is worse?**

* [] Acting when we shouldn’t (false positives)
* [] Not acting when we should (false negatives)

**What cannot be undone once action is taken?**

🔴 **Red flag:** “We’ll know it when we see it.”

---

## 3️⃣ Constraints (Design Inputs)

**Hard constraints (non-negotiable):**

* [] Budget
* [] Time
* [] People / operations
* [] Policy / legal
* [] Other: ______________________

**Actions explicitly out of scope (even if data suggests them):**


**Decisions that must remain human:**


🔴 **Red flag:** “Let’s see what the data says first.”

---

## 4️⃣ Evidence & Data (Trust Calibration)

| Evidence Source | Type (Authoritative / Proxy / Heuristic) | Owner | Confidence (High / Med / Low) |
| --------------- | ---------------------------------------- | ----- | ----------------------------- |
|                 |                                          |       |                               |
|                 |                                          |       |                               |

**Evidence currently trusted most (even if imperfect):**

🔴 **Red flag:** “The data should be fine — it’s in the system.”

---

## 5️⃣ Uncertainty & Assumptions (Make Them Visible)

**What do we *not* know that materially affects the decision?**
[] Timing
[] Causality
[] Coverage gaps
[] Biases

**What assumptions are currently being made implicitly?**
[] About behavior
[] About labels
[] About stability over time

**Which assumptions would be dangerous if wrong?**

🔴 **Red flag:** “We’ll clean that up later.”

---

## 6️⃣ Success Criteria (Without Metrics Yet)

**What would make you confident enough to use this?**
[] Clear explanations
[] Comparisons / baselines
[] Guardrails
[] Known failure modes
[] Other: ______________________

**What would make you *not* trust it?**

**What does ‘good enough’ look like for a first version?**

🔴 **Red flag:** “High accuracy.”

---

## 7️⃣ Explicit Non-Goals (This Prevents Scope Creep)

This system will **not**:

* [] Make automated decisions
* [] Optimize for all use cases
* [] Replace human judgment
* [] Answer unrelated questions

**Explicitly out of scope:**


🔴 **Red flag:** “Let’s keep it flexible.”

---

## 8️⃣ End-of-Kickoff Sanity Check (Always Do This)

**Before leaving the conversation, confirm:**
[] Decision can be stated in one sentence
[] Risks and constraints are acknowledged
[] Uncertainty is acceptable and expected
[] This is decision support, not an oracle

If any box is unchecked → **do not move downstream yet**.

---

## 🧠 How to Use This in Practice (Low-Friction)

* You do **not** need to ask every question verbatim
* Many answers come from listening, not interrogating
* You can fill this out **after** the meeting based on notes
* Treat it as a *thinking tool*, not a form to hand over

Even completing **60–70%** of this checklist dramatically reduces redesign risk.

---

## Why This Works

This checklist:

* locks alignment *before* irreversible pipeline choices
* forces risk to surface early
* naturally guides cleaning, features, modeling, and evaluation
* gives you cover later when tradeoffs are questioned

Most DS project failures happen **before code exists**.
This is how you prevent that — quietly and professionally.