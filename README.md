# credit-risk-classification

### *There was an inconsistency in the beginning of this challenge. The instructions on the Bootcamp Module say to:
1.  Create a new repository for this project called credit-risk-classification. Do not add this homework to an existing repository.
2.  Clone the new repository to your computer.
3.  Inside your credit-risk-classification repository, create a folder titled "Credit_Risk."
4.  Inside the "Credit_Risk" folder, add the credit_risk_classification.ipynb and lending_data.csv files found in the "Starter_Code.zip" file.
5.  Push your changes to GitHub.
### *As you can see, there was no instruction to create a "Resources" folder to put the csv file in. Therefore, I did not make a Resources folder. The problem comes in the actual Jupyter Notebook, where the instructions say to "Read the lending_data.csv data from the Resources folder into a Pandas DataFrame". This is confusing, as the instructions don't say to make a Resources folder. I went ahead and included a line of code simulating if there were a Resources folder, but my completed code is meant to run with the 2 files in the same location.

## Overview of Analysis
The purpose of this analysis was to determine whether a borrower (someone looking for a loan) would be a low-risk or high-risk borrower. Low-risk borrowers are expected to pay back loans on time while high-risk borrowers are less likely to make timely payments, stay current on payment plans, etc. This was done using scikit-learn to implement a logistic regression model and determine whether borrowers were low-risk (0) or high-risk (1). The dataset provided 77,536 examples of low-risk and high-risk data points to work with and create our models with.

## The Results
The results of the model were very interesting. The precision and recall scores were as follows:
  0 Class (low-risk) precision 1.00 (100%), recall 0.99 (99%)
  1 Class (high-risk) precision 0.85 (85%), recall 0.91 (91%)
These results reflect a very high accuracy for the low-risk borrowers and a lower accuracy for the high-risk borrowers. This means we can almost perfectly predict those who will be a low-risk borrower, but our current model is not nearly as accurate with predicting borrowers who are considered to be high-risk. We can also observe all of the true negatives (18,663), false positives (102), false negatives (56) and true positives (563).

## Summary
Our model is pretty effective, especially in identifying true negatives (loan rejections). There is room for improvement in minimizing false positives (approving high-risk borrowers who should have been denied, or at least, re-classified). In terms of precision and recall with low-risk borrowers, the model is highly accurate. In terms of precision and recall with high-risk borrowers, the model is less accurate but still performs well.  Overall, I think this model would be effective to use, but could be improved.
