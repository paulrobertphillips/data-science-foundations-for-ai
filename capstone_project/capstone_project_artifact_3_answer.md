# Capstone — Artifact 3

**1. Chosen evaluation metrics**
- Metric 1: Recall
  - Rewards: Overproactive inspection & maintenance servicing.
  - Punishes: Missed inspection & servicing opportunities.
  - Why appropriate: Since the decision system is being designed to prioritize early warning signals, the system's decision mechanism needs to be calibrated for handling false negative error.
- Metric 2: Coverage
  - Rewards: Lower accuracy of actions.
  - Punishes: Sacrificing reach across identified asset types for increased overall decision mechanism performance.
  - Why appropriate: Since key signal characteristics vary by asset type and environment which assets reside in, the system's decision mechanism needs to be calibrated for subtle, contextual differences observed across assets to avoid favoring one type over another.
- Metric 3: Time-to-Detection
  - Rewards: Increased frequency of inspection & maintenance servicing events.
  - Punishes: Increased lags between inspection & maintenance servicing events.
  - Why appropriate: Since actions made on assets are extremely costly monetarily speaking, the system's decision mechanism must be calibrated to prioritize timing of decision outcomes to avoid causing the organization to also incur irreversible costs in time. 

**2. Hidden failure modes**
- Metric 1: Recall
  - Hidden failure: Increased misprioritized for inspections or maintenance when in fact they may need require such.
- Metric 2: Coverage
  - Hidden failure: Decreased sensitivity in decision mechanism's ability to detect early warning signals.
- Metric 3: Time-to-detection
  - Hidden failure: Increased misprioritized for inspections or maintenance when in fact they may need require such.

**3. Threshold strategy**
- Strategy:
- Constraint enforced:
- Risk accepted:

**4. Explicitly rejected options**
- Rejected metric: Precision
  - Reason: We explicitly reject precision because the decision system's strategy seeks to increase sensitivity to early warning asset inspection & maintenance signals. Due to this, the model accepts increased error in misprioritizing asset inspection and maintenance servicing over missing asset inspection and maintenance servicing opportunities.
- Rejected threshold strategy:
  - Reason:
