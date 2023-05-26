# credit-risk-classification

## Overview of the Analysis

The purpose of this analysis was to develop machine learning models that predict whether a loan from LendingClub will be high risk or not. To achieve this goal, I used various machine learning models, including Random Forest Classifier, Logistic Regression, and AdaBoost Classifier. The data set provided contained information on various financial attributes of each loan, such as loan amount, interest rate, term, and borrower's income, among others.

Since the data set was imbalanced with more healthy loans (0) than high-risk loans (1), I used a combination of oversampling and undersampling methods to train and test my machine learning models. Specifically, I used the RandomOverSampler module from the imbalanced-learn library to oversample the minority class and the ClusterCentroids module from the same library to undersample the majority class.

## Results

The balanced accuracy scores and the precision and recall scores for each machine learning model are as follows:

Random Forest Classifier:

Balanced accuracy score: 0.678
Precision score:
High-risk loans (1): 0.98
Healthy loans (0): 0.75
Recall score:
High-risk loans (1): 0.05
Healthy loans (0): 1.00
Logistic Regression:

Balanced accuracy score: 0.671
Precision score:
High-risk loans (1): 0.08
Healthy loans (0): 1.00
Recall score:
High-risk loans (1): 0.72
Healthy loans (0): 0.62
AdaBoost Classifier:

Balanced accuracy score: 0.643
Precision score:
High-risk loans (1): 0.06
Healthy loans (0): 1.00
Recall score:
High-risk loans (1): 0.60
Healthy loans (0): 0.69

## Summary

Among the three models, the Random Forest Classifier had the highest balanced accuracy score of 0.678. This model also had the highest precision score for high-risk loans (1) at 0.98. However, the recall score for high-risk loans (1) was the lowest of the three models, at 0.05, indicating that the model is not very good at identifying high-risk loans.

The Logistic Regression model had the second-highest balanced accuracy score of 0.671, but the lowest precision score for high-risk loans (1) at 0.08. The recall score for high-risk loans (1) was the highest of the three models, at 0.72, indicating that this model is better at identifying high-risk loans than the other two models.

Finally, the AdaBoost Classifier had the lowest balanced accuracy score of 0.643 and the lowest precision score for high-risk loans (1) at 0.06. The recall score for high-risk loans (1) was in the middle of the three models, at 0.60.

Overall, I recommend using the Logistic Regression model due to its higher recall score for high-risk loans (1) and overall balanced accuracy score. However, it is important to note that the low precision score for high-risk loans (1) means that some healthy loans may be classified as high-risk loans, so additional evaluation and refinement of the model is necessary.
