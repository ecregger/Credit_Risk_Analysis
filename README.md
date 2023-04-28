# Credit_Risk_Analysis
The basis of this analysis is to create several different machine-learning models in order to determine whether they will be useful to predict someone's loan risk upon application. 

## Resampling Models
- <h2>Naive Random Oversampling: </h2> This method is not ideal due to the nearly non-existent precision score in predicting high risk alongside the low f1 scores and and unimpressive accuracy score. </p> <b>Results: </b> 
- <h2>SMOTE Oversampling: </h2> This method suffers from the same issues as the naive method. With a low accuracy of just below 0.65 and a nearly non-existent precision for predicting high risk. </p>
<b>Results:</b> 
- <h2>Cluster Centroids: </h2> With an under 0.55 accuracy score and a 0.01 for precision and f1 for high risk prediction, this will not be a good option either. </p>
<b>Results:</b> 
- <h2>SMOTEEN Combination: </h2> This method is also produced unsatisfactory results with an accuracy score just under 0.65 and very low precision and f1 scores for high risk loans. </p>
<b>Results: </b>

## Ensemble Models
- <h2>Balanced Random Forest: </h2> The precision results for this one are low for determining high-risk loans but the low-risk results remain at 1 (as all others have) and an accuracy score of .78 which is approaching acceptable. Still not ideal for high risk predictions. </p>
<b>Results: </b>
- <h2>Easy Ensemble AdaBoost: </h2> This model looks to be performing well with a 0.93 accuracy score but is not performing well with predicting high-risk loans as opposed to it's exact precision rating with low-risk. 

# Results and Reccomendation
The reullts of this initial analysis is a bit dissapointing, all models did not predict high-risk loans well at all. The only model to truly consider out of this set is the last one, the "Easy Ensemble AdaBoost Classifer". However, I wouldn't reccomend proceeding with "production" work using this model. Due to the low precision score for predicting high-risk loans, this model fails more than succeeds in it's true purpose. More training and more data needs to be considered or potentially even dropped from the model in order to nail-down the root cause of the innaccuracies in predicting high-risk loans. 
