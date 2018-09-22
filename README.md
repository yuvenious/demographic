Demographic and Voting behavior
======================
This analysis started from the hypothesis that the demographic information may give a valuable source to predict citizens’ voting behavior. This predictive model was made by the demographic information of 388 municipalities and corresponding election result of ****. The model can be used to **classify 388 municipalities into one of 6 political groups** by its demographic data . For example, given two municipalities’ demographic data, the model can estimate how their voting patterns will be and whether they share a similar voting pattern.
![scheme](https://user-images.githubusercontent.com/37578231/45921790-d9159700-bebc-11e8-9ce2-7574074d5947.png)

![choropleth](https://user-images.githubusercontent.com/37578231/45921789-d9159700-bebc-11e8-99ef-095ded541dcc.png)

Method
----------------------
It is a classification (y = cluster of political preference, 0 ~ 5) learning case with multiple numeric predictors (x = demographic data, 63). Since the original data contains 63 independent (predictors: demographic) and 28 dependent variables (target: parties), such high dimensions of variables needs to be reduced. Non-negative matrix factorization is mainly applied to investigate the most probable number of clusters.

- Given the election result of 388 municipalities, all municipalities are labeled (as a target variable) from cluster 0 to 5 by their political preferences.
- 63 Demographic data are used as predictors.

![similar](https://user-images.githubusercontent.com/37578231/45921791-d9159700-bebc-11e8-9b31-1e34c7cfbe0c.png)

Result
-----------------------
The model shows 75~80% of accuracy predicting the political clusters. If the subset of predictors are finely chosen, there is a chance to improve even more.
![accuracy](https://user-images.githubusercontent.com/37578231/45921788-d87d0080-bebc-11e8-8d73-7b5179f8181a.png)
