# credit-risk-classification

## Overview of Analysis
The purpose of this analysis was to determine whether a borrower (someone looking for a loan) would be a low-risk or high-risk borrower. Low-risk borrowers are expected to pay back loans on time while high-risk borrowers are less likely to make timely payments, stay current on payment plans, etc. This was done using a logistic regression model (scikit-learn) and determines whether borrowers were low-risk (0) or high-risk (1). The dataset provided 77,536 examples of low-risk and high-risk data points to work with and create our models with.

## The Results
The results of the model were very interesting. The precision and recall scores were as follows:
  0 Class (low-risk) precision 1.00 (100%), recall 0.99 (99%)
  1 Class (high-risk) precision 0.85 (85%), recall 0.91 (91%)
These results reflect a very high accuracy for the low-risk borrowers and a lower accuracy for the high-risk borrowers. This means we can almost perfectly predict those who will be a low-risk borrower, but our current model is not nearly as accurate with predicting borrowers who are considered to be high-risk.

We can also observe all of the true negatives (18,663), false positives (102), false negatives (56) and true positives (563).

## Summary
Our model is pretty effective, especially in identifying true negatives (loan rejections). There is room for improvement in minimizing false positives (approving high-risk borrowers who should have been denied, or at least, re-classified). Overall, I think this model would be effective but would need slight adjustments to improve the false positives.
