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

However, since there is a class imbalance, as the ratio of value counts for high-risk loan is only 3% of total dataset, hence it is important to observe both precison and recall scores. Considering both recall and precision scores for high-risk loan is reasonably good, especially recall scores is at 91%, it can be concluded that simple linear regession model can be used for predicting potential loan borrowers.



