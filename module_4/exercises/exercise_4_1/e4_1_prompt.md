# 🧪 Module 4 Mini-Exercise — *Model Rejection Is the Skill*

> **Goal:** Practice choosing models based on **constraint alignment** — and explicitly rejecting one.

We’ll continue with the **same churn decision context** and the **Strategy A vs Strategy B** framing you’ve already built.

---

## Step 1 — List Three Plausible Model Classes

Choose **three conceptually different model classes** that *could* be used here.
(No tuning, no metrics, no code.)

Examples (you may reuse or choose others):

* Logistic regression
* Shallow decision tree
* Gradient-boosted trees
* Rule-based scoring system
* Neural network

---

## Step 2 — For *Each* Model, Answer These Three Questions

For **each model**, answer honestly:

### 1️⃣ What constraint does this model satisfy well?

Examples:

* interpretability
* stability
* ability to handle noisy features
* operational simplicity
* ease of governance / auditability

---

### 2️⃣ What constraint does this model violate or stress?

Examples:

* opacity
* sensitivity to noise
* latency
* brittleness under distribution shift
* difficulty to disable or override

---

### 3️⃣ What failure mode would be *hardest to detect*?

Think *silent failure*, not crashes:

* gradual drift
* shortcut learning
* over-confidence
* feedback loops
* loss of stakeholder trust

---

## Step 3 — Explicitly Reject One Model (Required)

Choose **one** of the three and complete this sentence:

> **“We explicitly reject this model because…”**

Your reason **must** reference at least one of:

* decision risk
* reversibility
* interpretability
* stability
* governance
* alignment with Strategy A or B

❌ “Too complex” or “overkill” is **not sufficient**
✅ Tie the rejection to the **decision context**

---

## Rules (Important)

❌ No accuracy comparisons
❌ No hyperparameters
❌ No “industry best practice” claims

✅ Constraints first
✅ Failure modes named
✅ Rejection justified

---

## Response Format

Please reply using this structure:

```
Model 1:
- Satisfies:
- Violates:
- Hard-to-detect failure:

Model 2:
- Satisfies:
- Violates:
- Hard-to-detect failure:

Model 3:
- Satisfies:
- Violates:
- Hard-to-detect failure:

Explicitly rejected model:
- Reason for rejection:
```

---

## Why This Exercise Matters

Senior practitioners are distinguished less by:

> “What model did you choose?”

and more by:

> **“What model did you refuse to ship — and why?”**

Once you complete this, **Module 5 (Evaluation: Metrics as Decision Proxies)** will feel like a natural continuation rather than a separate topic.

Take your time — this is the kind of thinking that actually scales.
