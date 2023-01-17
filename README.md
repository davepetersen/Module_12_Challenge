# Module_12_Challenge

12th Challenge for the Columbia FinTech Boot Camp

## Technologies

* numpy
* pandas
* pathlib
* sklearn
* imblearn
* warnings

## Data

The data came from a database of peer to peer loans from a lending services company. Each loan contained the following information:

* Loan size
* Interest rate
* Borrower's income
* Debt-to-income ratio
* Number of accounts
* Number of marks against the borrower
* Total debt
* Marked if loan is healthy or high-risk

## Results/Summary

I split the original data into training and test sets. Then, I ran a logistic regression on the training data and found more healthy loans than high-risk loans (75,036 vs. 2,500). The logistic regression gave 56 false negatives and 102 false positives for a precision/recall of 85%/91% for high-risk loans. To improve recall, I oversampled the high-risk loans. As a result, we were able to produce a precision recall of 84%/99% and catch more high-risk loans, but at the cost of mislabeling some healthy loans as high-risk.