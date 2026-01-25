# ✅ Data Science Readiness for Production

## Decision-First Checklist Template

> **Purpose:**
> Determine whether a data science system is *ready to influence real decisions* — not whether it “works.”

---

## 1️⃣ Decision Readiness

[] The decision being supported is clearly stated in plain language
[] The decision owner (human) is explicitly named
[] The cost of being wrong is understood and documented
[] Decision reversibility (or irreversibility) is clear
[] This system is solving a *decision*, not “doing modeling for insight”

**Red flags**

* “We’ll figure out how to use it later”
* Multiple stakeholders assume different decisions

---

## 2️⃣ Data & Assumption Readiness

[] All major data sources are documented and defensible
[] Known data limitations (delay, noise, bias) are acknowledged
[] Label construction and trustworthiness are explicitly discussed
[] Key assumptions are written down (not implied)
[] There is agreement on what the data *does not* represent

**Red flags**

* “This is the best data we have”
* Labels treated as objective truth without context

---

## 3️⃣ Pipeline Coherence

[] Cleaning strategy aligns with the decision’s risk profile
[] Feature representations reflect intended behavior signals
[] Modeling approach (if used) satisfies decision constraints
[] Evaluation metrics reflect real-world consequences
[] Threshold strategies encode explicit policy choices
[] No pipeline step contradicts earlier assumptions

**Red flags**

* Each stage optimized independently
* Metrics look good but outcomes feel wrong

---

## 4️⃣ Human Oversight & Delegation Boundaries

[] Human review checkpoints are clearly defined
[] AI roles (analyst, reviewer, implementer) are explicitly constrained
[] AI is not allowed to make irreversible or policy decisions
[] Humans know when *not* to trust the system
[] Accountability for decisions is clearly human-owned

**Red flags**

* “The model decided”
* No clear intervention or override responsibility

---

## 5️⃣ Failure Awareness & Risk Acceptance

[] Plausible failure scenarios are documented
[] Silent failure modes are explicitly discussed
[] The team knows how failure would *first* appear
[] There is clarity on who absorbs cost when things go wrong
[] Risks are consciously accepted, not ignored

**Red flags**

* “We’ll catch it in monitoring”
* Surprise is treated as unavoidable

---

## 6️⃣ Organizational & Ethical Fit (Optional but Recommended)

[] System behavior aligns with organizational values
[] Uneven impact across groups has been considered
[] The system can be explained retrospectively
[] Deployment does not exceed the organization’s maturity level
[] There is confidence in defending this system externally if needed

**Red flags**

* “This is just an internal tool”
* “No one will notice if it’s wrong”

---

## 🧭 Final Readiness Call

**Overall assessment (choose one):**

* [] ✅ Go
* [] ⚠️ Conditional Go
* [] ❌ No-Go

**Justification (1–2 sentences):**

> *Why is this decision system ready — or not ready — to ship?*

---

## 🔑 Guiding Principle (Worth Remembering)

> **Production readiness is not about confidence.
> It’s about clarity on what you are committing to.**

---

## How to Use This Template Effectively

* Run it **before** deployment discussions
* Use it to slow down “metrics-driven optimism”
* Treat a **No-Go** as a success outcome
* Revisit it when assumptions change

This checklist is designed to travel with you across roles, teams, and companies — it reflects **judgment**, not tooling.

---

If you’d like next, I can:

* compress this into a **one-page executive version**
* adapt it into a **Jira / Confluence checklist**
* or map it directly to **Production Foundations** material

Just tell me how you’d like to use it.
