**Model 1**
Logistic regression for modeling under Strategy A.
- Satisfies:
This modeling approach would handle both interpretability & stability well, is logistic regression tends to be more rigid with its trend interpretation. Coefficients can also be understood from a contextual perspective in terms of importance.
- Violates:
The tradeoff for being a more simplistic, more rigid modeling approach is that logistic regression would be more sensitive changes in underlying distributions (e.g., distribution shifts). In other words, this approach relies more on distribution-related assumptions than perhaps other modeling techniques may. 
- Hard-to-detect failure:
The hardest-to-detect failure would be gradual drift, as at first modeling accuracy changes may be initially viewed as temporary noise in the data when in fact the inaccuracies could be signaling a need to retrain (or replace) the logistic regression modeling put in place.

**Model 2**
Gradient-boosted tree for modeling under Strategy B.
- Satisfies:
This modeling approach handles noisy features very well due to being a form a tree ensemble approach that seeks to minimize observed prediction error. 
- Violates:
The tradeoff for being a high-performing, highly-flexible modeling technique is having to deal with opacity of the model. Due to the fact this technique is considered a form of tree ensemble, modeling outcomes can be very difficult to interpret, espcially for someone who does not have a technical data science background.
- Hard-to-detect failure:
This model has the potential to fall for shortcut learning, since with each sequential tree added to the ensemble the model would seeking to reduce observed error. If this model is not implemented under the correct context, loss of stakeholder trust is also of high risk as this modeling technique (even if used properly) would be difficult to explain.

**Model 3**
K-nearest neighbors (KNN) for modeling under Strategy B.
- Satisfies:
This modeling approach balances both interpretability while being capable of handling noise features quite well. It is also operationally simple to understand & implement.
- Violates:
The constraint this modeling technique would violate would be latency. Due to the very nature of KNN, the model would essentially have to be retrained with every incoming batch of new data, making it computationally expensive to implment when compared to a modeling technique that would require retraining on a much less frequent basis.
- Hard-to-detect failure:
Because this modeling technique offers both interpretability & flexibility, it's easy to become over-confident in its performance. Gradual drift would also be of concern since the model has to be retrained with every new batch of records. However, gradual drift concern in the context of KNN would be different than that of something like logistic regression because with KNN gradual drift would be more of a "real world representation" concern than a performance once. In other words even as customer behaviors shift, KNN would likely perform well (since the model must be retrained with every new batch of records), but understanding overarching (big picture) changes in consumer behavior could only be caught/understood by cross-comparing properly timestamped modeled outcomes. If modeled outcomes are not managed properly, these changes in consumer behavior would be nearly impossible to detect.

**Explicitly rejected model**
- Reason for rejection:
We explicitly reject Model 1 because actions driven by Strategy A's decision-making process are viewed as being costly (e.g., irreversible). In other words the decision risk is high, therefore decision-making should not be based on probabilistic reasoning.