# Machine_Learning_LendingClub

This analysis focuses on building and evaluating several machine-learning models to predict credit risk using LendingClub data. Since credit risk is inherently imbalanced as there are many more good loans than bad loan, the analysis will need to also evaluate models with imbalanced classes. 

In the credit_risk_resampling file I utilize the imbalanced learn library to resample the LendingClub data and build and evaluate logistic regression classifiers using the resampled data.

In the credit_risk_ensemble file I compare two different ensemble classifiers to predict loan risk and evaluate each model.
- oversample the data using Naive Random Oversampler and SMOTE algorithms.

## Key Questions and Conclusions in Resampling Analysis:
1. Which model had the best balanced accuracy score?
- The combination sample has the highest balanced accuracy score at 0.64

2. Which model had the best recall score?
- The SMOTE oversampling model had the highest recall score at 0.65

3. Which model had the best geometric mean score?
- The combination sample has the highest geometric mean score at 0.64

## Key Questions and Conclusions in Ensemble Analysis:
1. Which model had the best balanced accuracy score?
- Easy ensemble had the highest balanced accuracy score at 0.93

2. Which model had the best recall score?
- The Balanced Random Forest and the Easy Ensemble both have the recall score at 0.92.

3. Which model had the best geometric mean score?
- Easy Ensenmble had the highest geometric mean score at 0.93

4. What are the top three features?
- 'total_rec_prncp'
- 'total_pymnt_inv'
- 'last_pymnt_amnt'
