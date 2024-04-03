# Credit-risk-classification

Overview
The purpose of this analysis is to evaluate the performance of a machine learning model in predicting credit risk. The logistic regression model has been developed to differentiate between healthy loans (0) and high-risk loans (1).

Results
Accuracy Score: The model exhibits a high overall accuracy of 99.18%.
Balanced Accuracy Score: A balanced accuracy of 95.20% indicates good performance on both classes despite class imbalance.
Precision Score:
For healthy loans (0): Precision is 100%, meaning no false positives were identified.
For high-risk loans (1): Precision is 85%, indicating some false positives.
Recall Score:
For healthy loans (0): Recall is 99%, suggesting almost all healthy loans are correctly identified.
For high-risk loans (1): Recall is 91%, showing that most high-risk loans are correctly identified but some are missed.
Summary
The logistic regression model used in this analysis shows excellent performance metrics; however, it is crucial to consider the context of these results:

The high performance is partly due to the data imbalance, with 96.77% of the loans being healthy. Therefore, while the model is adept at identifying healthy loans, its ability to detect high-risk loans—although still good—may not be as robust as the numbers suggest.
The performance of a credit risk model depends on the cost of misclassification. If predicting high-risk loans (1's) is critical to avoid financial loss, the recall score for high-risk loans is particularly important.
Given that the recall for high-risk loans is 91%, this suggests that 9% of high-risk loans might go undetected, potentially leading to unaccounted financial risk for the company.
Machine Learning Model 1: Logistic Regression
Accuracy: 99.18%
Balanced Accuracy: 95.20%
Precision: 100% for healthy loans, 85% for high-risk loans.
Recall: 99% for healthy loans, 91% for high-risk loans.
Recommendation
Considering the results:

The model demonstrates strong performance for an imbalanced dataset, particularly in precision and recall for healthy loans.
The recall for high-risk loans is good but could be improved; this is critical for credit risk models where failing to detect high risk can be costly.
Based on the current performance, I recommend using the model with the following considerations:

Further investigate the 9% of high-risk loans that might be missed to understand the financial implications.
Consider applying techniques to handle the data imbalance, such as oversampling the minority class or using anomaly detection methods specifically for high-risk loan detection.
If the cost of missing high-risk loans is high, continue to refine the model to improve recall for high-risk loans before deployment.
