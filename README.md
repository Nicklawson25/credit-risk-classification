# credit-risk-classification

## Instructions

1. **Split the Data into Training and Testing Sets:**
   - Load the `lending_data.csv` file into a Pandas DataFrame.
   - Create the labels set (`y`) from the `loan_status` column, where:
     - `0`: Healthy loan.
     - `1`: High-risk loan.
   - Create the features dataset (`X`) by selecting the remaining columns.
   - Use `train_test_split` to divide the data into training and testing datasets.

2. **Create a Logistic Regression Model with the Original Data:**
   - Train a logistic regression model using the training data (`X_train` and `y_train`).
   - Predict the outcomes for the testing dataset (`X_test`) using the trained model.
   - Evaluate the model's performance by:
     - Generating a confusion matrix.
     - Printing a classification report to analyze precision, recall, and F1-score.

3. **Write a Credit Risk Analysis Report:**
   - Summarize the model's performance, including key metrics such as accuracy, precision, and recall.
   - Provide recommendations based on the model's ability to classify both `healthy loans` and `high-risk loans`.

## Results

- **Accuracy Score:** 99%
- **Precision Scores:**
  - `0` (Healthy loan): 1.00
  - `1` (High-risk loan): 0.85
- **Recall Scores:**
  - `0` (Healthy loan): 0.99
  - `1` (High-risk loan): 0.95
- **F1-Scores:**
  - `0` (Healthy loan): 1.00
  - `1` (High-risk loan): 0.89

## Summary and Recommendations

The logistic regression model demonstrated exceptional performance, achieving an accuracy score of 99%. It accurately identified 95% of high-risk loans (`1`) and maintained high precision and recall for healthy loans (`0`). This makes it a reliable choice for predicting loan risk and supporting creditworthiness evaluations.

### Recommendation:

We recommend using the logistic regression model for this task due to its strong performance metrics, especially its ability to correctly classify high-risk loans. This is crucial for minimizing financial losses and ensuring effective risk management. However, further optimization or alternative techniques (e.g., ensemble methods) can be explored if even greater precision for high-risk loans is desired.
