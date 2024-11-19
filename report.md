# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

In this analysis, I attempted to use historical financial data from our users to try and create a model that could determine if users would be eligible for a loan. The historical data contained past loan sizes, interest rates, the borrower's income, the debt-to-income rate, the number of accounts, the derogatory marks, total debt, and whether or not the loan was healthy or high-risk. As previously stated, the goal of the model would be to predict whether or not the loan was healthy or high-risk so we could avoid high-risk loans in the future based on relationships that might not be obvious to the human eye. A Logistic Regression model was used in this case. The data was split into testing and training, the model was fit to the training data, then the model was used to make predictions on the test data, and the effectiveness of the model wasanalyzed using a confusion matrix and a classification report.

## Results

* Logistic Regression:
    * Accuracy: 0.99
    * Average precision: 0.94
    * Average Recall: 0.97

## Summary

I would not recommend this model for application in your company. It boasts a 99% accuracy, performing extremely well. However, it biases False Negatives over False Positives. We would rather have that be the other way around to err on the side of safety to guarantee that we lose as little money as possible on bad investments. Trying other models will be necessary.