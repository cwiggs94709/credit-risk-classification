# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.

The goal of this analysis was to develop and assess a model focused on predicting loan risk. Using a dataset derived from past lending transactions of a peer-to-peer lending platform, the objective is to construct a robust model capable of discerning the creditworthiness of potential borrowers.


* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
Given the dataset the model leverages the value of loan status to train and predict future outcomes. The values of loan size, borrower income, debt to income ratio, payment history and total debt was used as source data.

* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

To create a Logistic Regression Model with the lending data, I took the following steps: First, train the model by fitting it with the training data (X_train and y_train). Next, utilize the trained model to make predictions on the testing feature data (X_test) and store these predictions for further analysis. Finally, I was able to evaluate the model's performance by generating a confusion matrix to assess the accuracy of predictions and by printing a classification report, I was able to delve deeper into precision, recall, and F1-score metrics.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

Classification Report:
              precision    recall  f1-score   support

           0       1.00      1.00      1.00     15001
           1       0.86      0.91      0.88       507

    accuracy                           0.99     15508
   macro avg       0.93      0.95      0.94     15508
weighted avg       0.99      0.99      0.99     15508

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

Based on the classification report, the machine learning model demonstrates strong performance in classifying loan risk, with an overall accuracy of 99%. For the positive class (representing higher-risk loans), the model achieves a precision of 0.86 and recall of 0.91, indicating that it accurately identifies a substantial portion of high-risk loans while maintaining a relatively low false positive rate. However, for a comprehensive evaluation, it's essential to consider the specific objectives and trade-offs associated with the model's performance metrics. Given its high accuracy and balanced precision-recall trade-off, I would recommend deploying this model for identifying creditworthiness in loan applications.
If you do not recommend any of the models, please justify your reasoning.
