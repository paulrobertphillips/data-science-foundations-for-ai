**Step 1 - Pipeline context**
- **Context:** We are deciding which customer cohorts should receive intervention as means of mitigating churn risk under budget and operational constraints, with uncertainty about whether recent behavioral changes reflect true churn risk or temporary noise.
- **Strategy:** focus on early warning signals of customer churn.
- **High-level pipeline:** decision framing -> data trust boundaries -> cleaning strategy choice -> feature inclusion -> model class selection -> metric & threshold definition.
- **Risk:** risk associated with decision outcome is overintervention of customer outreach.

**Step 2 - AI design review prompt**
```
Act as a critical reviewer of decision framing for an early-warning churn system.

Assume this decision system fails six months after deployment. 

Please describe:
1. The most likely way this decision framing failed
2. Which assumption was probably wrong
3. What warning signs were likely ignored

Do NOT:
- propose fixes
- suggest models
```

**Step 3 - Human review checkpoints**
 1. **decision framing**

AI is allowed to generate decision options, identify the benefit/risk tradeoffs of each option, and generate draft artifacts. Humans retain final authority of what decision option to pursue in solution. Human judgement is required to ensure decision aligns with business needs (e.g., decision is appropriate for real world context).

 2. **data trust & sourcing**

Human judgement is required for this pipeline stage as it's more of a learning stage for AI than it is an action-taking stage. Humans provide AI context about each data source, help AI understand which are considered authoritative, proxy, or heuristic. AI cannot automate this stage as it does not have the appropriate real world context required to do so.

 3. **feature inclusion**
AI is allowed to recommend what relationships a model should see out of the data that has been selected & cleaned for use in the decision system. Human judgement is mandatory to: 1) ensure the correct worldview is being encoded with respect to the goal of the decision system, 2) the strategy is able to support the correct intervention policy, & 3) associated failure modes are explainable.

**Step 4 - Delegation boundary**
AI is allowed to propose multiple threshold strategies, but must never choose thresholds autonomously.