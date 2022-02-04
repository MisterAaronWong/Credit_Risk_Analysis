# Credit_Risk_Analysis

## Overview
The purpose of this analysis was to employ different techniques to train and evaluate models with unbalanced classes for credit risk analysis. This is because credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. First, the data was oversampled using the RandomOverSampler and SMOTE algorithms, and then undersampled using the ClusterCentroids algorithm. Afterwards, a combinatorial approach of over- and undersampling using the SMOTEENN algorithm was implemented. Next, the usuge of the BalancedRandomForestClassifier and EasyEnsembleClassifier machine learning models that reduce bias are compared to predict credit risk. Finally, the performance of these models were evaluated and a recommendation was made on whether they should be used to predict credit risk.

## Results
### Naive Random Oversampling
![82](Resources/82.png)

### Naive Random Oversampling
![nonvine5percent](Resources/nonvine5percent.png)

## Summary
In regards to balanced accuracy, this metric is measured between 0 and 1. The model with the an accuracy score closest to 1 would be considered the best machine learning model for this metric. In this case, the Easy Ensemble AdaBoost Classifier held the highest balanced accuracy score at nearly 0.93. No other models came close to this accuracy score.

The precision values for all models were similar. The precision scores for all models showed low scores for high-risk loans and high scores for low-risk loans. 

The recall score ranges between 0 and 1, with numbers closer to 1 indicating the better model. Under this metric, the Easy Ensemble AdaBoost Classifier had the highest recall scores (.91 for high-risk and .94 for low-risk), proving this to be the best machine learning model to choose for further credit card analysis.
