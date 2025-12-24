# 🧪 Module 1 Mini-Exercise — Ingestion as Trust Calibration

We will stay **strictly at the ingestion boundary**.
No cleaning, no modeling, no fixes.

---

## Step 1 — Choose ONE input source

From the churn-intervention scenario, pick **one** of the following (just one):

* **Customer usage logs**
* **Support ticket volume**
* **Billing / tenure data**
* **Historical churn labels**

👉 Tell me **which one you chose**.

---

## Step 2 — Classify the source (AI-style)

Answer briefly:

1. Is this source **authoritative**, **proxy**, or **heuristic**?
2. Who *controls* this data (system, team, vendor)?
3. How confident should downstream decisions be in this data
   *(high / medium / low — and why)*?

---

## Step 3 — Boundary failure thought experiment

Complete this sentence:

> **“If this data is wrong or misleading, the most dangerous downstream decision failure would be ______.”**

Be concrete. Think in **decision impact**, not technical error.

---

## Rules (Important)

❌ Do **not** propose validation, cleaning, or fixes
❌ Do **not** talk about models or features
✅ Only reason about **trust, assumptions, and breakage**

---

## What I’ll Do After You Reply

I’ll review your answers as a **senior AI-native ingestion reviewer** and show you:

* what trust assumptions you made (explicit or implicit)
* where AI would over- or under-weight this input
* how this shapes *everything* in Module 2 (cleaning)

When you’re ready, reply with:

* your chosen input
* your classification answers
* your failure sentence

Take your time — this is where systems quietly succeed or fail.
