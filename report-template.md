# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

-- We are evaluating a model based on loan risk. The analysis uses a dataset of lending activity to build a model that can identify the creditworthiness of borrowers. The financial data of loan sizes, interest rates, borrower income, debt-to-income value, number of accounts, derogatory marks and total debt were used in this analysis to overall predict the loan status. 

Steps
1. Read in the CSV file
2. Seperate the data into labels and features
3. Check balance of labels variable using 'value_counts'
4. Split data into training and testing
5. Fit a logistic regression model using the training data and then save predictions
6. Evaluate the models performace, using accuracy score and confusion matrix
7. Predict a Logistic Regression Model with Resampled Training Data
8. Use LogisticRegression Classifier to fit the model and make predicitons
9. Evaluate model performance


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
                 precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
                precision    recall  f1-score   support

           0       0.99      0.99      0.99     56271
           1       0.99      0.99      0.99     56271

    accuracy                           0.99    112542
   macro avg       0.99      0.99      0.99    112542
weighted avg       0.99      0.99      0.99    112542

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
-- Model 2 performs the best due to it having a quantity of 0.99 across all its sections.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
-- Yes performace depends on the problem itself. In this case, it should be more important being able to predict the 0s in order to know what to look out for in terms of risk.
