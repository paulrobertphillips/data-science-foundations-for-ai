# 🎓 DS Foundations Capstone Project

## **Designing, Evaluating, and Defending a Decision System**

---

## Capstone Objective

Demonstrate that you can **design a coherent, decision-first data science system**, reason about its risks, and make defensible go / no-go judgments — *without hiding behind models or metrics*.

By the end, you should be able to answer:

> **“Should this system be trusted to influence real decisions — and why?”**

---

## Capstone Scenario (New)

### **Infrastructure Maintenance Prioritization System**

A large organization operates **hundreds of geographically distributed physical assets** (e.g., power grid components, transportation infrastructure, industrial equipment).

Maintenance budgets and field crews are limited, and **reactive repairs are extremely costly**. However, performing maintenance too early or unnecessarily also has significant cost and operational impact.

Leadership wants a **decision-support system** to help prioritize which assets should receive **proactive inspection or maintenance** in the coming planning cycle.

---

### Decision Being Supported

> **Which assets should be prioritized for proactive inspection or maintenance in the next planning window, given limited maintenance capacity and uncertainty about whether observed signals indicate true failure risk or temporary anomalies?**

---

### Why This Decision Is Hard

* Asset failures are **rare but high impact**
* Signals are **weak, noisy, and heterogeneous**
* Failures may occur long after early warning signs
* Interventions are **costly and partially irreversible**
* Incorrect prioritization can lead to:

  * catastrophic failure
  * unnecessary shutdowns
  * wasted budget
  * safety and reputational risk

---

### Strategic Orientation (Implicit)

The organization is considering an **early-warning, risk-sensitive strategy**, where:

* Missing a true failure risk is more costly than unnecessary inspection
* Some false positives are acceptable
* Human engineers retain final authority over actions
* The system is **directional**, not prescriptive

(You may make this strategy explicit or challenge it in your capstone.)

---

## What You Will Produce (Final Artifacts)

You will produce **four tightly scoped artifacts**. Each maps directly to a set of modules.

---

### 📄 Artifact 1 — Decision & Risk Framing

*(Modules 0–1)*

**Deliverables:**

* Decision statement (1–2 sentences)
* Decision owner
* Why the decision is risky or irreversible
* What “being wrong” looks like

> This anchors everything else.

---

### 📄 Artifact 2 — Pipeline Design (Decision-First)

*(Modules 2–4)*

**Deliverables:**

* Data trust boundaries (what is / isn’t acceptable evidence)
* Uncertainty shaping strategy (what ambiguity is preserved vs suppressed)
* Feature *concepts* (not implementations)
* Modeling stance (including explicit rejection if applicable)

> Focus on **intent and alignment**, not mechanics.

---

### 📄 Artifact 3 — Evaluation & Policy Choices

*(Module 5)*

**Deliverables:**

* Chosen evaluation metrics (with justification)
* Chosen threshold strategy (as policy)
* Explicit tradeoffs accepted
* Explicit options rejected (and why)

> This is where values become behavior.

---

### 📄 Artifact 4 — Readiness & Go / No-Go Decision

*(Modules 6–8)*

**Deliverables:**

* Readiness assessment across five dimensions
* Go / Conditional Go / No-Go call
* Primary blocking risk (if not Go)
* Human oversight boundaries

> This is the capstone judgment.

---

## How This Will Be Evaluated

I’ll assess your capstone on:

* **Coherence** — do all choices align end-to-end?
* **Judgment** — do you surface and own risk?
* **Restraint** — do you avoid over-automation?
* **Clarity** — could a stakeholder understand and trust this?
* **Defensibility** — could you stand by this decision later?

There is **no penalty** for choosing:

* simple approaches
* conservative stances
* No-Go outcomes

---

## How We’ll Work Through This

We’ll do this **iteratively**, not all at once.

### Step 1 (Start Here)

Let’s begin with **Artifact 1**.

Reply with:

```
Capstone — Artifact 1

Decision statement:
Decision owner:
Why this decision is risky:
What being wrong looks like:
```

Once we lock Artifact 1, we’ll move forward **one artifact at a time**, just like a real project review.

---

## Final Reminder

> **This capstone is not about proving technical capability.
> It’s about proving judgment under uncertainty.**

When you’re ready, send **Artifact 1** for the **Infrastructure Maintenance Prioritization System**, and we’ll begin the capstone review.
