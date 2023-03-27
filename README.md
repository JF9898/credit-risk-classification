# credit-risk-classification
ML model to analyze credit risk
# Module 12 Report Template

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
 - the purpose of this analysis is to create a model that can accurately predict levels of credit risk between healthy (0) and high-risk (1)
* Explain what financial information the data was on, and what you needed to predict.
 - The data used had multiple columns that took into account, the loan size, interest rate, borrower income, debt to income, number of accounts derogatory marks as well as total debt. The prediction that needed to be made was whether the account in question falls under the healthy loan category or the high risk loan category.
 
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
 - The two models created both performed very well and it depends on the specific metric the user would like to know better in order to determine which of the two models would work best in their scenario. The original model I made appears to be slightly better at predicting the High risk category which may be of more importance in comparison to healthy loans. With that being said, the oversampled data had a higher overall accuracy between the both of them.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  Overall the Model 1 accuracy was 0.9520479254722232, 
  the precision between category 0 and 1 were 1.00 and 0.85 respectively. 
  
  the final classification report looks like this...
                precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  Model 2 accuracy was 0.9936781215845847, which is highly accurate however the precison between the 2 categories was 1.00 for category 0 and 0.84 for category 1 
  the final classification report looks like this...
                precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.99      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
 - in summary, both models performed extremely well if I do say so myself, either of them will produce accurate responses however the first model will likely predict the high risk category better than the overall more accurate second model. This leads into the next bullet point. 
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
The two models are both highly accurate and can likely be interchangeable, however I would be using the first model if trying to predict the high credit risk individual accounts as it is slightly more precise, if just looking for overall accuracy I would use the second model.
If you do not recommend any of the models, please justify your reasoning.
Thankfully that is not the case here today.
