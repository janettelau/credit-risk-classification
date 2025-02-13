# credit-risk-classification

## Setup and Usage
1. Clone this repository to your local machine using `git clone`.
2. Navigate to the cloned directory in Visual Studio Code.
3. Open the Jupyter Notebook `credit_risk_classification.ipynb`.
4. Run each cell sequentially to load the data, create and train the model, test it, and evaluate its performance.

## Credit Risk Analysis Report

### Overview of the Analysis
The purpose of the analysis is to build a machine learning model using `LogisticRegression` that can identify the creditworthiness of the borrower and predict whether it is a healthy or high-risk loan. The dataset contains historical lending activity from a peer-to-peer lending services company, with data including loan sizes, interest rates, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total amount of debt, and loan status.

The target variable is `loan_status`, which has a value of `0` (healthy loan) or `1` (high-risk loan). 

The machine learning process in this analysis includes three main stages:
1. Splitting the data into training and testing datasets using `train_test_split`.
2. Building the machine learning model using `LogisticRegression`, then training it and testing the fitted model.
3. Evaluating the model’s performance by generating a confusion matrix and a classification report.

### Results
#### Machine Learning – Logistic Regression Model
* Accuracy Score: 0.99
    * The logistic regression model is 99% accurate in predicting whether it is a healthy or high-risk loan correctly.
* Precision Scores:
    * Class `0` (healthy loan): 1.00
       * The model has a precision of 100% in predicting healthy loans, meaning it has extremely high accuracy and makes no false positives or false negatives.
    * Class `1` (high-risk loan): 0.87
       * The model has a precision of 87% in predicting high-risk loans. This means that about 13% of the predicted high-risk loans are in fact healthy loans, so there is some room for improvement.
* Recall Scores:
    * Class `0` (healthy loan): 1.00
       * The model predicts healthy loans with 100% recall.
    * Class `1` (high-risk loan): 0.95
       * The model predicts high-risk loans with 95% recall.

### Summary
Overall, the logistic regression model achieves a very high accuracy of 99%, making it highly effective in predicting the labels. However, the model is more accurate in predicting healthy loans, while its accuracy in predicting high-risk loans could benefit from some improvements.
