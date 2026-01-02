**Capstone — Artifact 2**

**1. Data trust boundaries**
- **Asset Telemetry & Condition Signals**
  - These sources are heuristic because they're buffered and aggregated downstream.
  - Representation of a given asset's current state could break if signal is wrong.
  - Failure modes:
    - Calibration drift, which will impact decision outcome over time. 
    - Not all assets have identical signal coverage, which could cause decision mechanism to misinterpret certain assets.
  - Ingestion is streaming or near-real-time, because of how embedded data collection systems have been configured.
  - Confidence in downstream decisions should be medium.
- **Maintenance & Inspection History**
  - These sources are heuristic because event data would be inferred signal.
  - Decision of when a given asset is due for proactive inspection or maintenance could break if signal is wrong.
  - Failure modes:
    - Label delay, since data is recorded after the event has already occurred.
    - Label noise, since label creation is influenced by inspection practices and incentives present over time. Labels are also human entered and reflect what was observed, not necessarily true asset state.
    - Label leakage, could invoke short-cut learning in decision mechanism.
    - Missing changes in upstream collection logic.
  - Ingestion is episodic, because data is only generated when a maintenance or inspection event occurs.
  - Confidence in downstream decisions should be low.
- **Operational Context & Usage**
  - These sources are heuristic because they are often derived from upstream systems, and may be inferred rather than directly measured.
  - Representation of a given asset's current state could break if signal is wrong.
  - Failure modes:
    - Label delay, since collection system is known to experience lag.
  - Ingestion is batch, data is collected in daily or weekly aggregates.
  - Confidence in downstream decisions should be medium.
- **Failure & Incident Report**
  - These sources are heuristic because event labels would be an inferred signal.
  - Decision of when a given asset is due for proactive inspection or maintenance could break if signal is wrong.
  - Failure modes:
    - Label delay, since data is recorded after the event has already occurred.
    - Missing changes in upstream collection logic.
    - Label leakage, could invoke short-cut learning in decision mechanism.
  - Ingestion is episodic, because data is only generated when a failure or incident event occurs.
  - Confidence in downstream decisions should be low.

**2. Uncertainty shaping strategy**
- Strategy:
  - Abiguity is intentionally preserved.
  - Short-term volatility is retained.
  - No aggressive label stabilization is applied.
  - Edge cases are not collapsed.
- Risk: Accepting messiness to avoid false certainty.
- Assumptions: Observed anomalies are occurring systematically.
- Dangerous If: Observed anomalies being treated as systematic error are in fact occurring randomly.


**3. Representation & feature concepts**
- **Feature concept 1:** Weekly fluctation in asset telemetry & condition signals.
  - Makes visible: Drastic changes in signal could offer an early warning signal for inspection or maintenance requirements.
  - Assumption: Reason for signal changes are mechanically driven, not environmentally driven.
- **Feature concept 2:** Total time since last maintenance & inspection event.
  - Makes visible: How long it's been since assets have last received a maintenance or inspection event.
  - Assumption: Reason for changes in length of time are driven by current state of asset, not environmentally driven.
- **Feature concept 3:** Weekly fluctuation in operational context & usage signals.
 - Makes visible: Drastic changes in asset usage and performance could offer an early warning signal for inspection or maintenance requirements.
 - Assumption: Reason for changes in usage patterns directly correlates with changes in maintenance and inspection requirements for a given asset.
- **Feature concept 4:** Number of failure & incident reports.
 - Makes visible: Frequency of issues that have occurred with each asset.
 - Assumption: The more issues that have occurred, the more inspection or maintenance attention the asset should be receiving.

**4. Modeling stance**
- Position: a Rule-based system that outputs risk scores, not decisions.
- Rationale: Actions taken by decision system are viewed as irreversible due to all outcomes being considered costly to the organization. Even if this rationale were overriden, labels are also not considered meaningful and timely. They are at risk of label delay, contextual drift, and leakage.
- Explicit constraints / rejections: We explicitly reject use of probabilistic reasoning in this decision system because actions taken from such are considered costly (e.g., irreversible). The combined risk of weak signals and trust erosion being present also the system should rely on a decision mechanism that can fail predictably.
