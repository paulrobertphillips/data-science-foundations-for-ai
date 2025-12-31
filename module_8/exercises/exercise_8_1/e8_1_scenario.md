# 📘 Project Scenario Context

## Churn Early-Warning System — Strategy B

### Business Context

The company is a **subscription-based B2B SaaS platform** with:

* multi-year contracts
* high customer lifetime value
* long sales cycles
* a dedicated customer success (CS) team

Churn events are **rare but costly**, and by the time cancellation occurs, **intervention is often too late**.

Leadership has asked for an **early-warning system** to help prioritize proactive outreach.

---

## Decision Being Supported

> **Which customers should receive early human outreach due to elevated churn risk, given limited customer success capacity?**

This decision:

* is **repeated weekly**
* affects **real customers**
* has **cost and trust implications**
* is **partially reversible** (outreach can’t be undone, but no incentives are automatically applied)

---

## Strategic Orientation (Strategy B)

The system is explicitly designed to:

* prioritize **sensitivity over precision**
* surface **weak and early signals**
* tolerate false positives
* minimize missed churn cases

Leadership accepts:

* some unnecessary outreach
* some customer annoyance
  in exchange for **earlier detection and learning**.

---

## What Has Been Built So Far (Assume This Is True)

### 1️⃣ Decision Framing

* The decision statement is documented and approved.
* Stakeholders agree the system is **directional**, not definitive.
* Customer success leadership is the decision owner.

---

### 2️⃣ Data Sources

The system uses:

* **product usage telemetry** (logins, feature usage trends)
* **support interaction counts** (tickets, chat sessions)
* **billing & subscription metadata** (renewal dates, plan changes)

Known limitations:

* churn labels are **delayed**
* support interactions can reflect both engagement *and* dissatisfaction
* usage data is noisy and seasonal

---

### 3️⃣ Uncertainty & Cleaning Approach

* Ambiguity is **intentionally preserved**
* Short-term volatility is retained
* No aggressive label stabilization is applied
* Edge cases are not collapsed

This aligns with Strategy B’s goal of expanding churn signal coverage.

---

### 4️⃣ Representation & Features

Features are **conceptual**, not overly engineered:

* changes in usage patterns
* increases in support interactions
* proximity to renewal dates
* deviations from historical baselines

The system is designed to:

* detect **relative changes**, not absolute thresholds
* remain interpretable to CS teams

---

### 5️⃣ Modeling (If Used)

* A flexible, non-linear model has been prototyped
* The model outputs **risk scores**, not decisions
* No automated action is triggered by the model alone

Human review is required before outreach.

---

### 6️⃣ Evaluation & Thresholding

Evaluation emphasizes:

* recall
* coverage
* time-to-detection

Thresholding is:

* **capacity-constrained**
* tuned to surface more cases than CS can act on directly
* used as a prioritization mechanism, not a hard cutoff

---

### 7️⃣ Human Oversight

* Customer success managers review flagged accounts weekly
* No automatic incentives or penalties are applied
* Feedback from CS is captured informally but not yet systematized

---

### 8️⃣ Current Pressure

Leadership is asking:

> “Can we start using this to guide outreach next quarter?”

There is **no mandate to deploy**, but there is **momentum**.

---

## How to Use This Scenario for Module 8

When answering:

* **Step 1** → Treat this as the system being evaluated
* **Step 2** → Judge readiness *as-is*, not after improvements
* **Step 3** → Make a go/no-go call based on risk, not optimism
* **Step 4** → Name the most important readiness gap honestly

You are **not expected to say “Go.”**
A *Conditional Go* or *No-Go* is often the strongest answer.

---

## Final Reminder

This exercise is about **judgment**, not correctness.

There is no “right” outcome — only **defensible reasoning**.

When you’re ready, you can now complete **Module 8’s mini-exercise** using this scenario, and I’ll review it as if it were a real production readiness meeting.
