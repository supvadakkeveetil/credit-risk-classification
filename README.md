# credit-risk-classification

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
  - Read data from the CSV file into a Pandas Data Frame
  - Separate the data into labels and features. Create the label set y from the loan_status column and the features dataframe X from the other columns 
  - Split the data into training and testing datasets using the train_test_split
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
 - Create a LogisticRegressin Model with the data
 - Make predictions using the testing data
 - Evaluate model's performance using the Confusion Matrix and the Classification Report

## Results

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
![ML_Accuracy_score](https://github.com/supvadakkeveetil/credit-risk-classification/assets/144635564/175e2ce4-0ab0-4353-94fa-0be13185b075)


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
