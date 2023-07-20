# Credit-Risk-Classification

## Overview of the analysis

This challenge module uses supervised machine learning technique to build model based on lending dataset provided in "lending_data.csv" to identify the credit worthiness of borrowers. 

The lending dataset provided has various financial debt information of each borrowers and need to utilise the loan status to predict new data set and check the accuracy of the model in the predictions.

Linear regression model is mainly used to predict this dataset on how accurate is the model to predict loan status for healthy loan (as 0) and bad loan (as 1).

On top of this, random forests model is also used to carry out the model accuracy and points out the most important features for this model predictions. 

## Results 
* Machine Learning Model 1: Linear Regression Model
  * Accuracy: 0.99
  * Precision: 1 (for healthy loan), and 0.89 (for high risk loan)
  * Recall: 0.99 (for healthy loan), and 0.92 (for high risk loan)
  * f1-score: 1 (for healthy loan), and 0.91 (for high risk loan)
 
* Machine Learning Model 2: Random Forest Model
  * Accuracy: 0.99
  * Precision: 1 (for healthy loan), and 0.90 (for high risk loan)
  * Recall: 1 (for healthy loan), and 0.92 (for high risk loan)
  * f1-score: 1 (for healthy loan), and 0.90 (for high risk loan)

## Summary
Overall, both models result in similar results, high accuracy and f1 score for predicting loan status.

However, since there is a class imbalance, as the ratio of value counts for high-risk loan is only 3% of total dataset, hence it is important to observe both precison and recall scores. 

Recall scores are more highly considered as company do not want to make false predictions for false negative borrowers whom in real life already has huge debt. Thus, with recall scores being at 92%, it is considered a good model. 

The model for high risk loan has initially has f1-score below 90%, but the model was improved by using following 3 methods: 
 - Stratified sampling: using same ratio as label data
 - Set optimum test data: 20% of data for test, 80% of data for training
 - Set random state: 42 is the optimum random state to increase the scores

In conclusion, simple linear regession model can be used for predicting potential loan borrowers.
