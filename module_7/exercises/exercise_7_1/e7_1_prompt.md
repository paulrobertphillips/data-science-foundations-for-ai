# 🧪 Module 7 Mini-Exercise — Human–AI Co-Design Review

> **Goal:** Demonstrate that you can **collaborate with AI safely** by constraining its role, inserting human review points, and preventing over-automation.

We’ll continue using your **churn early-warning (Strategy B)** context.

---

## Step 1 — Pipeline Context (Brief)

In 3–5 bullets, restate:

* the **decision** being supported
* the **strategy** (e.g., early warning / sensitivity-first)
* the **high-level pipeline** (data → representation → decision)
* the **primary risk if wrong**

*No tools, no metrics, no models.*

---

## Step 2 — Write the AI Design Review Prompt

Write **one prompt** you would give AI to **review** (not build) the pipeline.

Your prompt must:

* assign AI the **Reviewer** role
* ask for **assumptions**, **risks**, and **failure modes**
* explicitly forbid AI from proposing fixes or making decisions

> You are **not** running the prompt — only writing it.

---

## Step 3 — Mandatory Human Review Checkpoints

List **three pipeline stages** where:

* AI input is allowed
* **human judgment is mandatory**
* humans retain final authority

For each checkpoint, explain **why automation would be dangerous** there.

Examples of stages (choose any three):

* decision framing
* data trust & sourcing
* cleaning / uncertainty shaping
* feature inclusion
* model class selection (if any)
* metric & threshold definition

---

## Step 4 — Explicit Delegation Boundary

Complete this sentence **precisely**:

> **“AI is allowed to ___, but must never ___ in this system.”**

Be concrete (e.g., “choose thresholds,” “approve deployment,” “redefine success”).

---

## Rules (Important)

❌ No production tooling
❌ No governance frameworks
❌ No model details

✅ Role-constrained AI
✅ Explicit human ownership
✅ Clear automation boundaries

---

## Response Format (Use This)

```
Step 1 — Pipeline context:
- …

Step 2 — AI design review prompt:
“…”

Step 3 — Human review checkpoints:
1. …
2. …
3. …

Step 4 — Delegation boundary:
AI is allowed to ___, but must never ___.
```

---

When you’re ready, send your submission. I’ll review it the way a senior reviewer would: checking **role clarity**, **risk containment**, and whether your boundaries genuinely prevent over-automation.
