# Credit_Risk_Analysis

## Overview
Th purpose of this project was to analyise credit risk from a datadet by LendingCLub using `imbalanced-learn`and `scikit-learn` libraries to build and evaluate models using resampling. Oversampling the data was done using `RandomOverSampler` and `SMOTE` algorithms, while undersampling ther data using `ClusterCentroids` algorithm. Combining over and under sampleing, `SMOTEEN` algorithm. To reduce bias, two machine learning models were used `BalancedRandomForestClassifer` and `EasyEnsembleClassifer`, to predict credit risk.

## Results

## Dev 1: Resampling Models to Predict Credit Risk

### Naive Random OverSampling

![Oversampling_report](https://user-images.githubusercontent.com/115188500/223168099-0b14ea82-d9ef-4da6-8b1c-57ade8d2a373.png)

* Balanced Accuracy: 0.6547385707934685
* Precision: Precision is low for High-risk loans and high for Low-risk loans
* Recall: High Risk: 0.72  | Low Risk: 0.59

### SMOTE Oversampling

<img width="687" alt="SMOTE_report" src="https://user-images.githubusercontent.com/115188500/223169638-4550bf37-b288-4078-b582-4ec8d4d33818.png">

* Balanced Accuracy: 0.6547385707934685
* Precision: Precision is low for High-risk loans and high for Low-risk loans
* Recall: High Risk: 0.72 | Low Risk: 0.59

### Undersampling

<img width="687" alt="undersampling_report" src="https://user-images.githubusercontent.com/115188500/223170421-b761f8bf-fdd2-4b5c-84c3-6b24999e304a.png">

* Balanced Accuracy: 0.5442369453268994
* Precision: Precision is low for High-risk loans and high for Low-risk loans
* Recall: High Risk: 0.69 | Low Risk: 0.40

## Dev 2: Combination SMOTEEN Sampling

### Combination Sampling

<img width="713" alt="Combination_report" src="https://user-images.githubusercontent.com/115188500/223173133-6f739e29-b3f9-4926-aaf4-e7350a36f513.png">

* Balanced Accuracy: 0.6472841741611017
* Precision: Precision is low for High-risk loans and high for Low-risk loans
* Recall: High Risk: 0.72 | Low Risk: 0.57

## Dev 3: Ensemble Classifiers

### Balanced Random Forest Classifer

<img width="698" alt="BalancedRandom_report" src="https://user-images.githubusercontent.com/115188500/223171645-32d8e3af-549c-44a8-b6e6-13cb92e1ed44.png">

* Balanced Accuracy: 0.7885466545953005
* Precision: Precision is low for High-risk loans and high for Low-risk loans
* Recall: High Risk: 0.70 | Low Risk: 0.87


### Easy Ensemble AdaBoost Classifer

<img width="673" alt="Easyensemble_report" src="https://user-images.githubusercontent.com/115188500/223172334-63990f4a-7ab1-4994-be6b-d1963d866fcd.png">

* Balanced Accuracy: 0.9316600714093861
* Precision: Precision is low for High-risk loans and high for Low-risk loans
* Recall: High Risk: 0.92 | Low Risk: 0.94


## Summary:
The highest balanced accuracy score closest to 1 is the best Machine Learning model to use. For this project, the `EasyEnsembleClassifer` was the closest score at 0.93 balanced accuracy. The other models were quite low, between .40 - and .87. The precision remained consistant for the High Risk and Low Risk loans. The `EasyEnsembleClassifer` had the highest recall score closest to 1 (0.92/0.94), making it the best machine learning model to use for future credit risk analysis.
