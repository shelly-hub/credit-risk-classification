# Credit-Risk-Classification

## Overview of the analysis

This challenge module uses supervised machine learning technique to build model based on lending dataset provided in "lending_data.csv" to identify the credit worthiness of borrowers. 

The lending dataset provided has various financial debt information of each borrowers and need to utilise the loan status to predict new data set and check the accuracy of the model in the predictions.

Linear regression model is mainly used to predict this dataset on how accurate is the model to predict loan status for healthy loan (as 0) and bad loan (as 1).

On top of this, random forests model is also used to carry out the model accuracy and points out the most important features for this model predictions. 

## Results 
* Machine Learning Model 1: Linear Regression Model and Random Forest Model 
  * Accuracy: 0.99
  * Precision: 1 (for healthy loan), and 0.85 (for high risk loan)
  * Recall: 0.99 (for healthy loan), and 0.91 (for high risk loan)
  * f1-score: 1 (for healthy loan), and 0.87 (for high risk loan)

## Summary
Overall, both models result in similar results, high accuracy for predicting loan status.

However, there is slight shortfall for predicting high risk loan as f1-score falls below 90%.
Even though the ratio of value counts for high-risk loan is minimal only takes up 3% of total data, but it is the most important output which determines if loan should be given. 

