Create README.md on 14 April 2024

# Challenge 20 - Credit Risk Classification

Introduction

The purpose of this Challenge is to build a model from historical lending activity that can identify the creditworthiness of borrowers. 

The historical data of lending activity included loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt, and loan_status. The loan status was recorded as 0 for a healthy loan and 1 for an unhealthy load. The object is to process the other features to predict whether a loan will be healthy or a problem.

LogisticRegression Model.

The method used in this Challenge was the LogisticRegression model. This choice was made due to its simplicity, efficiency, and interpretability, making it an excellent starting point for any binary classification problem. It provides a solid baseline, and from its performance, you can determine whether more complex models are necessary or if its results are sufficient for your needs. 

LogisticRegression predicts a binary outcome and provides probability scores.  It performs well when the decision boundary between the classes is linearly separable (i.e., it can be separated by a straight line). It's a strong linear classifier when relationships between features are roughly linear.

Results

Classification Report

              precision    recall  f1-score   support

           0       1.00      1.00      1.00     15001
           1       0.86      0.91      0.88       507

    accuracy                           0.99     15508
   macro avg       0.93      0.95      0.94     15508
weighted avg       0.99      0.99      0.99     15508


Precision: Indicates the accuracy of positive predictions.

For class 0 (healthy loans), the precision is 1.00, meaning that when the model predicts a loan is healthy, it is correct 100% of the time.

For class 1 (problem loans), the precision is 0.86, which means that when the model predicts a loan is a problem, it is correct 86% of the time.

For class 0, the recall is 1.00, implying that the model identified all healthy loans correctly.

For class 1, the recall is 0.91, indicating that the model correctly identified 91% of all actual problem loans.

F1-Score: The weighted average of Precision and Recall. This score takes both false positives and false negatives into account. 

For class 0, the F1-score is 1.00, showing excellent model performance for healthy loans.

The F1-score for class 1 is 0.88, indicating good performance, but there is room for improvement compared to healthy loan performance.

Class 0 has 15001 instances, making it the majority class.
Class 1 has 507 cases, indicating it is much rarer in comparison.

References

Scikit-learn Documentation: - scikit-learn.org/.021/documentation.html
Scikit-learn: -devdocs.io/scikit_learn/
Scikit-learn - What is scikit learn tutorial - Youtube - Inttelipast
Scikit-learn tutorial - Youtube - Simplilearn
Logistic Regression in Python from Scratch [ Youtube - Coding Lane
ChatGPT



