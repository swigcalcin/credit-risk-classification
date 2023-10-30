# credit-risk-classification(Put my Analysis on the README)

Overview of the Analysis
In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

-Explain the purpose of the analysis.
The purpose is to use various techniques to test the effectiveness and predict the loan risk. To build a model that can spot the worthinesss of credit borrowers. 

-Explain what financial information the data was on, and what you needed to predict.
We created a file path of the lending dataframe. We needed to predict how risky the loans are with the information given to us. The information given to us in the lending dataframe can be characterized as loan_size, interest_rate, borrower_income, debt_to_income, number of accounts, marks, and total debt. We use this information to weigh on high risk or healthy a loan is. 

-Provide basic information about the variables you were trying to predict (e.g., value_counts).
After creating a file path of the lending dataframe, we received two types of loans. The healthy loans (0) and the high risk loans (1). The health loans had a count of 75036 while the high risk loans had 2500. 


-Describe the stages of the machine learning process you went through as part of this analysis.
We first created labels setting y from loan status and creating features with X from the other columns. We check the balances of the labels using value_count and then split the data by using train_test_split.  We then created a logistic regression with the training data which in trun helped us save the predictions on the data labels by using the testing feature data and fitted the model. Lastly, we review the predictions and the modles through balance accuracy, confusion matrix, and classification_report. We then repeated the same process withe the resampled training by using RandomOverSampler. 

-Briefly touch on any methods you used (e.g., LogisticRegression, or any resampling method).
The methods we used were LogisticRegression Model and the RandomOVerSampler(resampling method to determine our probabilities 


Results
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

-Machine Learning Model 1:

Description of Model 1 Accuracy, Precision, and Recall scores.
Accuracy score: 95.21%

Healthy Loans: 
Precision: 100% (1.00)
recall: 99% 

High-risk loan:
Precision: 85%
recall: 91%


-Machine Learning Model 2:

Description of Model 2 Accuracy, Precision, and Recall scores.
Accuracy score: 99.47%

Healthy loans:
Precision: 99%
recall:99%

High-risk loan: 
Precision: 99%
recall:99%


Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

-Which one seems to perform best? How do you know it performs best?
The method that should be preferred and performed better would be method 2 the resampling method. 

-Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the 1's, or predict the 0's? )
I believe its a bit more important to predict more of the 0's due to the high risk loans being slightly more unpredictable when using model 1. Therefore, multiple methods are esstenial. 

-If you do not recommend any of the models, please justify your reasoning.
Both methods seem to be extremely accurate with their predictions nearing 90-100 percentile. However, the slight edge for the resampling method may be method that is more favorable compared to the 1st one. 
