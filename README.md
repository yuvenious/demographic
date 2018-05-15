### Summary
This analysis started from the hypothesis that the demographic information may give a valuable
source to predict citizens’ voting behavior. This predictive model was made by the demographic
information of 388 municipalities and corresponding election result of ****. The model can be used to
**classify 388 municipalities into one of 6 political groups** by its demographic data . For
example, given two municipalities’ demographic data, the model can estimate how their voting
patterns will be and whether they share a similar voting pattern.

### Method
In short, it is a classification (y = cluster of political preference, 0 ~ 5) learning with multiple
numeric predictors (x = demographic data, 63). Since the original data contains 63 independent
(predictors: demographic) and 28 dependent variables (target: parties), such high dimensions of
variables needs to be reduced. Non-negative matrix factorization is mainly applied to investigate
the most probable number of clusters.

1. Given the election result of 388 municipalities, all municipalities are labeled (as a target
variable) from cluster 0 to 5 by their political preferences.
2. 63 Demographic data are used as predictors.

### Result
The model shows 75~80% of accuracy predicting the political clusters. If the subset of
predictors are finely chosen, there is a chance to improve even more.
