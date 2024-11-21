# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis. The primary goal of this analysis was to evaluate machine learning models to predict loan risk, identifying loans as either 0 (healthy loan) or 1 (high-risk loan). This prediction can help financial institutions assess and manage loan portfolios effectively.

  
* Explain what financial information the data was on, and what you needed to predict.

  The dataset included financial information related to loan applications, such as applicant credit scores, income, debt-to-income ratios, loan amounts, and other key variables.
The target variable was a binary classification: 0 (healthy loan) and 1 (high-risk loan). The task involved predicting this binary label.


* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The dataset was imbalanced, with far more instances of 0 (healthy loans) compared to 1 (high-risk loans). The value_counts showed:
0: 18,765
1: 619
  
* Describe the stages of the machine learning process you went through as part of this analysis.
Data Preprocessing:
Handled imbalanced data by considering performance metrics like precision, recall, and F1-score, which are better suited for imbalanced datasets.
Split data into training and testing sets to evaluate model performance effectively.
Feature Selection and Scaling:
Identified important features influencing loan risk and scaled numerical data using standardization.
Model Training:
Trained machine learning models such as LogisticRegression on the data to classify loans.
Model Evaluation:
Evaluated models using metrics like accuracy, precision, recall, and F1-score, especially focusing on 1 (high-risk loans) to ensure the model captures critical cases.


* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
 Logistic Regression was implemented as the primary algorithm due to its simplicity and effectiveness in binary classification tasks.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
 
  Accuracy: 99%
Precision:
0 (healthy loans): 1.00
1 (high-risk loans): 0.85
Recall:
0 (healthy loans): 0.99
1 (high-risk loans): 0.95
F1-Score:
0 (healthy loans): 1.00
1 (high-risk loans): 0.89

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
  
Which Model Performs Best?

Logistic Regression performed exceptionally well, achieving an overall accuracy of 99%. It demonstrated high recall for high-risk loans (1), which is critical for minimizing financial risks.
Performance Dependency on the Problem:

For this problem, recall for high-risk loans (1) is more critical than precision. Financial institutions must minimize the risk of incorrectly classifying a high-risk loan as healthy (0), even if it means occasionally misclassifying healthy loans as high-risk (1).
  

If you do not recommend any of the models, please justify your reasoning.

Based on the high accuracy, precision, recall, and F1-score, Logistic Regression is recommended. Its ability to correctly identify 95% of high-risk loans makes it a reliable choice for predicting loan risk.
