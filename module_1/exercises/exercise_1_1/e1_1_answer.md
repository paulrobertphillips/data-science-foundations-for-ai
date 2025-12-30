**Chosen Input**
Historical churn labels.


**Classification Answers**
1. This source is heuristic because event labels would an inferred signal.
2. Team controls this data because human intervention is required to define context behind assigned labels.
3. Confidence in downstream decisions should be low, because AI is at risk of:
    - Inferring label delay or noise.
    - Assuming historical churn labels are correct.
    - Missing changes in upstream collection logic (e.g., label updates for records previously trained on).

**Failure Sentence**
If this data is wrong or misleading, the most dangerous downstream decision failure would be action taken resulting in one of the previously identified, irreversible outcomes.