**Chosen strategy**
```
I choose to implement Strategy B, early warning, recall-first.
```

**Recall**
```
- Rewards / punishes:
This metric discourages false negative error, which is the type of error that would result in missed intervention opportunities. Since Strategy B prioritizes identifying early warning signals, the decision process's model needs to be optimized for handling false negative error.

- Hidden failure:
This choice will result in some customers being flagged as potential churn when in fact that may not be the case. That is, by focusing on recall (signal sensitivity) we're accepting losses in precision (signal stability).
```

**Coverage**
```
- Rewards / punishes:
This metric discourages narrow reach of what customers actually get flagged before churning. That is, coverage ensures that the model is being optimized to consider all existing cohorts, not just the ones it performs best for (e.g., the model won't sacrifice coverage for smaller, lower impact cohorts to maximize recall for larger, more impacful cohorts). Since Strategy B prioritizes identifying early warning signals, the decision process's model needs to be optimized to pick up signals for all cohorts, not just the most problematic ones.

- Hidden failure:
This choice will result in loss in recall optimization (e.g., loss in model sensitivity to false negative error). 
```

**Chosen threshold strategy**
```
- Constraint enforced:
Capacity-constrained thresholding.

- Risk accepted:
By choosing this threshold strategy, accepted risk is that the decision-process will take action on customers flagged as "potential churn" when in fact they are not. That is, the threshold strategy will lean into overintervening with customers.
```

**Explicitly rejected option**
```
- Reason for rejection:
We explicitly reject tiered thresholding because Strategy B's decision process seeks to increase sensitivity to early warning customer churn signals. Due to this, the model should be expected to take action at lower confidence scores. Furthermore, the concern with implementing tiered thresholding would be: 1) creating unnecessary cost by adding a human intervention layer to handle medium confidence cases (something that could occur frequently in the system being defined), & 2) taking no action on low confidence cases (something that contradicts what has been defined for Strategy B).
```