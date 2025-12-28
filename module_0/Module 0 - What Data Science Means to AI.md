# MODULE 0 — What “Data Science” Means to AI

---

### The Core Mental Model (This Is the Unifying Idea)

> **A data science pipeline is a sequence of irreversible decisions that progressively collapse uncertainty into structure.**

Each step:
- answers some questions
- locks in some assumptions
- eliminates entire classes of future options
This is why early steps feel abstract and later steps feel constrained.
---
### Terminology
- **SAP BW tools** - refers to SAP Business Warehouse, an enterprise data warehousing platform used by large organizations to collect, transform, & report on data from SAP & non-SAP systems.
	- In practice usually means the ETL, data modeling, & reporting components inside SAP BW that support enterprise analytics & decision-making rather than ad hoc data science work.
- **Label delay** - means the outcome you care about (example: true customer churn) is only observed after a significant time lag, so recent data may be mislabeled as "not churned" simply because the event hasn't happened yet
- **f** - means some recorded outcomes are wrong or ambiguous (e.g., customers marked as churned for administrative reasons), causing the system to learn patterns that reflect logging artifacts rather than real behavior.
---


https://www.analyticsvidhya.com/blog/2022/08/basic-introduction-to-data-science-pipeline/?utm_source=chatgpt.com
https://www.sapbwconsulting.com/blog/decision-making-and-uncertainty?utm_source=chatgpt.com

Notes:
- Notice the message isn't data scientists are expected to know everything there is about information technology. There is a clear slot in which data science fits in the grand scheme of information technology.

https://codiant.com/blog/role-of-data-science-in-informed-business-decision-making/?utm_source=chatgpt.com

https://www.geeksforgeeks.org/machine-learning/decision-tree-introduction-example/?utm_source=chatgpt.com
https://kanerika.com/blogs/data-analytics-pipeline/?utm_source=chatgpt.com

https://www.timeplus.com/post/data-pipeline-architecture?utm_source=chatgpt.com

Why This Module Exists

Humans often define data science by tools. AI defines data science by decision structure.
If you don’t align on this early, everything downstream breaks:
- models optimize the wrong thing
- metrics don’t map to decisions
- production teams inherit undefendable systems
This module reprograms your mental model before you touch ingestion, cleaning, or modeling.
---

Core Mental Model (Anchor This)

To AI, data science is the practice of transforming uncertainty into constrained, defensible decisions using data.Pipelines are not scripts.They are decision graphs.

Takeaways
- Historically data science has been taught as "something you do" before delivering analysis (e.g., loading, cleaning, merging, etc.) -> 80% of DS work is data preparation, 20% is modeling (as the saying goes).
	- Issue: this mental model naturally narrows practitioners point of view from what matters to an organization -> it's why conversations tend to become technical very quickly, everything spoken about is tool & technique driven, how the work ties back to the organization is usually thought through at the very end.
	- Issue: this causes discipline to become blurry, practitioners find themselves involved in unnecessary technical deep dives that span across other disciplines (data engineering, database administration, IT, etc).
- DS's role is to transform uncertainty into something structured & explainable -> DS is not simply being a technician with a toolbelt.
	- It's not the stakeholder's responsibility to turn business needs into formulated projects
	- Moving away from "using this tool" to "do this thing" -> moving to "what are we trying to do?", "what does that need to look like?", "what would having this help us achieve?", "what would failure mean to us out of this?" -> which then drives what actions need to occur & those actions drive what tools & techniques will be required
---

How AI Sees the Data Science Lifecycle

AI implicitly reasons backwards:
1. What decision is being made?
2. What uncertainty affects that decision?
3. What evidence reduces that uncertainty?
4. What representation (features, summaries) makes that evidence usable?
5. Is a model even necessary?
Most human workflows start at step 4 or 5. AI starts at step 1 — and everything else must justify itself.
---

Key Reframes (Very Important)


❌ Old framing

- “I’m building a model to predict X”
- “This notebook does EDA and modeling”
- “We need better features”

✅ AI-native framing

- “We are deciding X under Y constraints with Z uncertainty”
- “This step reduces uncertainty about [specific risk]”
- “This representation changes what the model can see”
This language shift is subtle — but it’s the difference between analysis and decision support.
---

AI Decision Questions (You’ll Reuse These Constantly)

At every pipeline stage, AI implicitly asks:
1. What decision is downstream of this?
2. What uncertainty am I reducing?
3. What constraints matter most here?
If you cannot answer all three, the step is likely misaligned or unnecessary.
---

📊 Example Project Scenario (Shared Baseline)


Project Idea: Customer Retention Intervention System

A subscription-based company has noticed that customer churn has increased over the last two quarters. Leadership wants to reduce churn, but interventions (discounts, outreach, service upgrades) are costly and limited, so they cannot be applied to everyone.
A data science team is asked to “analyze the data and build a model” to help address the issue.
Available data includes:
- customer usage history
- billing and tenure information
- support ticket volume
- past churn outcomes (with noise and delays)
There is uncertainty about:
- which signals actually precede churn
- whether churn is behavior-driven or price-driven
- how reliable historical labels are
---

🧪 Revised Module 0 Mini-Exercise (Decision-First)


Step 1 — Rewrite the project goal as a decision statement

Use this template:
“We are deciding [action] under [constraints] with uncertainty about [unknowns].”Example solution (one of many valid answers):
“We are deciding which customers should receive retention interventions under budget and operational constraints, with uncertainty about whether observed behavior indicates true churn risk or temporary noise.”
Step 2 — Sanity-check alignment

Ask:
- Who takes this action?
- What happens if the decision is wrong?
- Is this decision reversible?
If those answers are fuzzy, the problem definition — not the model — is the issue.
---
This scenario is intentionally generic, realistic, and reusable.We’ll continue to reuse it lightly across ingestion, cleaning, features, modeling, and evaluation so you can see how the same decision propagates through the pipeline.
When you’re ready, we’ll move on to Module 1 — Data Ingestion: How AI Thinks About Inputs.
---

How AI Should Be Used Here (Discipline Check)

At this stage, AI’s role is:
- translator (turning tasks into decisions)
- challenger (questioning assumptions)
- enumerator (listing uncertainties)
AI should not:
- design full pipelines yet
- suggest models
- optimize metrics
We’ll earn that later.
---

What You’ve Gained After Module 0

By the end of this module, you can:
- explain data science without naming tools
- frame work in AI-native decision language
- catch misaligned pipelines before they harden
- sound production-aware without touching production
This is the lowest-risk, highest-signal shift you can make at work.

Takeaways
- AI-native nuance when it comes to stating whether a decision is reversible or not
	- 💸 Cost is irreversible
	- 📉 Customer churn outcomes may be irreversible (partial)
	- 🔁 Policy decisions can be revised in future cycles
---
