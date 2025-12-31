# Capstone Context — Data Assumptions for Artifact 2

**Infrastructure Maintenance Prioritization System**

Use the following as **ground truth assumptions** when completing Artifact 2.

---

## 1️⃣ What Data Is Available (Conceptual Categories)

You may assume the organization has **four broad classes of data** available.

### A. Asset Telemetry & Condition Signals

Examples (conceptual, not exhaustive):

* sensor readings (temperature, vibration, load, pressure)
* error or warning codes
* automated health indicators

**Key characteristics:**

* collected automatically by embedded systems
* noisy and environment-sensitive
* varies significantly by asset type
* not all assets have identical sensor coverage

---

### B. Maintenance & Inspection History

Examples:

* dates of past inspections
* maintenance actions taken
* findings or notes from inspections
* severity classifications (if any)

**Key characteristics:**

* partially structured
* human-entered
* reflects **what was observed**, not necessarily true asset state
* influenced by inspection practices and incentives

---

### C. Operational Context & Usage

Examples:

* utilization rates
* duty cycles
* load profiles
* environmental exposure (weather, geography, seasonality)

**Key characteristics:**

* often aggregated
* may be inferred rather than directly measured
* critical for contextualizing telemetry

---

### D. Failure & Incident Records

Examples:

* asset failures
* near-miss incidents
* emergency repairs
* downtime events

**Key characteristics:**

* rare
* high impact
* often recorded *after the fact*
* definitions may change over time

---

## 2️⃣ What the Organization Understands About the Data

You can assume the organization has **partial but imperfect understanding** of its data.

### Well Understood

* where data comes from (systems of record)
* which teams own which sources
* basic collection mechanisms
* rough latency (minutes vs days)

### Poorly Understood / Risky

* sensor calibration drift
* historical changes in logging behavior
* consistency of inspection notes across teams
* whether failures represent true “ground truth” or reporting artifacts

Importantly:

> **No data source is treated as objective truth.**

This is a core assumption you should lean on.

---

## 3️⃣ How Data Is Collected (Ingestion Mode)

You can assume a **mixed ingestion landscape**, which is very realistic.

### Telemetry Data

* **Streaming or near-real-time**
* buffered and aggregated downstream
* raw streams usually not consumed directly by DS

**Implication:**
High volume, high noise, temporal sensitivity.

---

### Maintenance & Inspection Records

* **Episodic**
* generated when inspections occur
* backfilled after field work is completed

**Implication:**
Event-driven, irregular cadence, human bias.

---

### Operational Context Data

* **Batch**
* daily or weekly aggregates
* often derived from upstream systems

**Implication:**
Lagged but stabilizing context.

---

### Failure & Incident Records

* **Episodic**
* often delayed
* sometimes revised post-incident

**Implication:**
Label delay and definition drift are expected.

---

## 4️⃣ Storage & Accessibility Assumptions

You may assume:

* data is centrally accessible (e.g., data lake / warehouse)
* schemas exist but are not perfectly enforced
* historical backfills occur
* lineage is partially documented

You should **not** assume:

* perfect versioning
* clean, consistent schemas over time
* uniform data quality across asset classes

---

## 5️⃣ What This Means for Artifact 2 (How to Use This)

When writing **Artifact 2**, you should:

### In **Data Trust Boundaries**

* treat all data as **directional evidence**
* explicitly reject any source as ground truth
* require human context for high-stakes interpretation

---

### In **Uncertainty Shaping**

* acknowledge sensor noise and label delay
* decide whether to preserve or suppress short-term volatility
* explicitly justify ambiguity preservation or smoothing

---

### In **Representation**

* favor **relative changes**, trends, and deviations
* avoid absolute thresholds as “truth”
* encode context-aware signals

---

### In **Modeling Stance**

* explicitly constrain what models are allowed to infer
* ensure humans remain responsible for action
* reject approaches that imply false certainty

---

## 6️⃣ One-Line Mental Model (Very Important)

> **This system reasons over imperfect evidence to support prioritization —
> it does not diagnose failure.**

If you keep that sentence in mind, your Artifact 2 will stay aligned.

---