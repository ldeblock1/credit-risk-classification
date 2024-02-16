# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of the analysis was to develop machine learning models to predict credit-risk of loan applicants based on various financial features.

* Explain what financial information the data was on, and what you needed to predict.
The data included information on loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt, among other variables. The target variable for prediction was the loan status, which indicated whether a loan was classified as high-risk (1) or healthy (0).

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

Loan Status (y): The target variable representing loan status, with two categories: 0 for healthy loans and 1 for high-risk loans. The value_counts showed imbalanced classes, with a larger number of healthy loans compared to high-risk loans.
Features (X): Various financial features used as predictors, including loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.

* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

1. Split the dataset into training and testing sets using train_test_split.
2. Train the machine learning models, including Logistic Regression, on the training data.
3. Evaluate theb model's performance using metrics such as balanced accuracy score, precision, recall, confusion matrix, and classification report.
4. Address the class imbalance using resampling techniques such as RandomOverSampler to improve model performance on minority class prediction.




## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

Balanced Accuracy Score: 0.952
Precision (Class 0): 1.00
Precision (Class 1): 0.85
Recall (Class 0): 0.99
Recall (Class 1): 0.91


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

Balanced Accuracy Score: 0.994
Precision (Class 0): 1.00
Precision (Class 1): 0.84
Recall (Class 0): 0.99
Recall (Class 1): 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?

Model 2, with logistic regression and resampling, performs better based on its higher balanced accuracy score and improved recall for both classes.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

Yes, performance depends on the problem being solved. In this case, correctly predicting high-risk loans (1) is crucial to avoid potential financial losses. Model 2's higher recall for (1) makes it more suitable for this problem, as it reduces the chances of missing high-risk loans.

If you do not recommend any of the models, please justify your reasoning.

Based on the results, Model 2 (Logistic Regression with Resampling) is recommended for predicting loan status. It demonstrates superior performance in terms of balanced accuracy and recall for both healthy and high-risk loans, making it more reliable for assessing creditworthiness.