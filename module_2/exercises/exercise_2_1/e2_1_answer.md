**Strategy A**
```
Description:
Goal of approach is to focus on reducing noise in the data. This means cleansing outcome will ensure data is reshaped to have clear boundaries between what is considered to be a "churned customer" and what is not. In other words this approach will effectively stabilize current understanding of what a "churned customer" is. This involves data improvements such as removing ambiguous labels, collapsing edge cases, and enforcing stricter definitions of churn.

Questions:
1. What assumption does this strategy make about churn?
This strategy assumes that risk to mitigate for are false positives if the decision being made is to determine who should receive costly retention incentives. In this decision case it's more important to mitigate risk of a customer being flagged as a "churned customer" when the customer in fact is not.


2. What bias does this strategy introduce?
Cleaning approach focuses on smoothing short-term volatility and being conservative about retaining observed anomalies. Observed error is treated as occurring randomly.

3. When would this strategy be dangerous?
This approach assumes observed anomalies are occurring at random. Danger of approach would be if this assumption is violated. That is, if observed anomalies are either systematic or structural error as opposed to being random.
```

**Strategy B**
```
Description:
Goal of approach is to focus on preserving ambiguity in the data. That means cleansing outcome will ensure data is reshaped to capture all known (& undiscovered) subgroups present. In other words this approach will exhaustively explore what a "churned customer" can be. This involves keeping uncertain labels, encoding uncertainty explicitly, and accepting messiness to avoid false certainty.

Questions:
1. What assumption does this strategy make about churn?
This strategy assumes that risk to mitigate for are false negatives if the decision being made is to determine who needs immediate human outreach. In this decision case it's more important to mitigate risk of a customer not being flagged as a "churned customer" when the customer in fact is.

2. What bias does this strategy introduce?
Cleaning approach focuses on preserving anomalies and treating missing data as warning signals. Observed error is treated as not occurring at random.

3. When would this strategy be dangerous?
This approach assumes observed anomalies are occurring systematically. Danger of approach would be if this assumption is violated. That is, if observed anomalies are treated as systematic error but are in fact random.
```