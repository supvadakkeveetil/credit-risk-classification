# credit-risk-classification

## Overview of the Analysis

* Explain the purpose of the analysis.
  The purpose of the analysis is
  - To build a model that can identify the credit worthiness of borrowers
* Explain what financial information the data was on, and what you needed to predict.
  - Historical lending activity dataset froma peer to peer lending services company
  - Structure of the DataFrame
![DF_structure](https://github.com/supvadakkeveetil/credit-risk-classification/assets/144635564/3d70d451-107d-4a59-b4c4-5c3d76f27fa9)

Based on the data we need to predict the Accuracy Score and the Classification Report

* Describe the stages of the machine learning process you went through as part of this analysis.
  - Read data from the CSV file into a Pandas Data Frame
  - Separate the data into labels and features. Create the label set y from the loan_status column and the features dataframe X from the other columns 
  - Split the data into training and testing datasets using the train_test_split
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
  - Create a LogisticRegression Model with the data
  - Make predictions using the testing data
  - Evaluate model's performance using the Confusion Matrix and the Classification Report

## Results

* Machine Learning Model:
  * Description of Models Accuracy, Precision, and Recall scores.
![ML_Accuracy_score](https://github.com/supvadakkeveetil/credit-risk-classification/assets/144635564/175e2ce4-0ab0-4353-94fa-0be13185b075)


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
The accuracy score for the test dataset is about 99%. So it predicts 99.24% loans correctly.
Based on the Classification report, The model can predict the Healthy loans(0) with 100% accuracy, and the High-risk loans(1's) with about 87% (however, based on the recall it missed 11% of them).
The model identifies the healthy and high risk loans effectively, which is very good as misclassification could lead to financial burden for the borrower but there is a need to consider the potential consequences of false negatives of high risk loans (1's) as it could mean financial loss for the lender if these loans default.
