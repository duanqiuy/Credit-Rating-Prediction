# Credit-Rating-Prediction

Something need to be changed: 
The logistic regression model produces probabilities and classify the predictions if the probability is higher than 0.5. For example, it approves a credit application if the probability of default is 45%; that is, the probability of the client repaying fully is 55%. But, banks never approve such applications if the risk is 45%. Ideally, the probability predictions should be obtained by predict_proba() function. If the risk level exceeds a reasonable threshold (e.g., 10%), the predictions should be classified as "negative." This analysis is missing.

The way assigned numbers to categorical data is not correct. 

For example, marital_status takes 0 if not specified, 1 for single, and 2 for married. The categories are not sorted out in sequence. The ideal strategy should be to use get_dummies.
