# Credit_Risk_Analysis

## Analysis Overview
In this project, Python was used to build and evaluate several machine learning models to predict credit risk.  
WThe following procedures were used: 
- Oversampling the data using the **RandomOverSampler** and **SMOTE** algorithms.
- Undersampling the data using the **ClusterCentroids** algorithm.
- Using a combined approach of over- and undersampling using the **SMOTEENN** algorithm.
- Comparing two machine learning models that reduce bias, **BalancedRandomForestClassifier** and **EasyEnsembleClassifier**.  

The goal is to evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.

## Results 

### RandomOverSampler model  





### SMOTE model





### ClusterCentroids model




### SMOTEENN model





### BalancedRandomForestClassifier model





### EasyEnsembleClassifier model





## Summary
All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high. The Ensemble models brought a lot more improvment, especially on the sensitivity of the high risk credits. The EasyEnsembleClassifier model shows a recall of 92% so it detects almost all high risk credit.
