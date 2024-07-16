Monash Boot Camp Week 20 Challenge Report

Overview of Analysis
The purpose of this project is to use machine learning to evaluate the eligibility of borrowers.
The dataset contains lending activity from a peer-to-peer lending services company,
and we aim to predict whether a future loan will be healthy (0) or at high risk of defaulting (1).

The main steps are as follows:
Data Preparation: Reading the CSV file into a Pandas DataFrame, and splitting the data into features (X) and labels (y).
Data Splitting: Dividing the dataset into training and testing sets using `train_test_split`.
Model Training: Training a logistic regression model using the training data.
Model Evaluation: Evaluating the model's performance using a confusion matrix and a classification report.

Results
Classification Report:
           precision    recall  f1-score   support

       0       1.00      0.99      1.00     18765
       1       0.84      0.94      0.89       619

accuracy                           0.99     19384

Summary
-Accuracy: The model achieved an accuracy of 0.99, indicating that 99% of the predictions were correct.
-Precision: The precision for high-risk loans was 0.84, suggesting that 84% of the predicted high-risk loans were actually high risk.
-Recall: The recall for high-risk loans was 0.94, indicating that the model correctly identified 94% of all actual high-risk loans.

The logistic regression does a very good job at predicting the eventual results. The accuracy of 99% means that all but 1% of cases were correctly identified.
A precision of 84% for the high risk loans, and a recall of 94%, means that it's very good at identifying those loans.

As the loans which are at risk of defaulting are the most important to identify, and as this model does a good job of identifying those loans,
it would be recommended to implement this model in the decision making process for a company.
