# Credit Risk Analysis

## Overview of Project

### Purpose

The purpose of this project was to predict credit risk, which is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. To try and solve the unbalance we used several different methods like below:
  
  *	oversampling the data by using RandomOverSampler and SMOTE algorithms
  * undersampling the data using the ClusterCentroids algorithm
  *	over- and undersampling using the SMOTEENN algorithm
  *	Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier

## Results

Here we will look at the balanced accuracy scores, the precision, recall scores, and the F1 scores of all six machine learning models.

### RandomOverSampler model

![naïve_random.png](https://github.com/SZapata4/Credit_Risk_Analysis/blob/main/Images/naive_random.png)

  *	The balanced accuracy score is 65%.
  *	The high_risk precision is about 1% with 62% sensitivity which makes a F1 of 2%.
  *	The low_risk precision is almost 100% with a sensitivity of 68% and a F1 of 81%.

### SMOTE Model

![smote.png](https://github.com/SZapata4/Credit_Risk_Analysis/blob/main/Images/smote.png)

  *	The balanced accuracy score is 64%.
  *	The high_risk precision is about 1% with 63% sensitivity which makes a F1 of 2%.
  *	The low_risk precision is almost 100% with a sensitivity of 66% and a F1 of 79%.

### ClusterCentroids Model

![cluster_centroids.png](https://github.com/SZapata4/Credit_Risk_Analysis/blob/main/Images/cluster_centroids.png)

  *	The balanced accuracy score is 53%.
  *	The high_risk precision is about 1% with 61% sensitivity which makes a F1 of 1%.
  *	The low_risk precision is almost 100% with a sensitivity of 45% and a F1 of 62%.

### SMOTEENN Model

![smoteenn.png](https://github.com/SZapata4/Credit_Risk_Analysis/blob/main/Images/smoteenn.png)

  *	The balanced accuracy score is 62%.
  *	The high_risk precision is about 1% with 68% sensitivity which makes a F1 of 2%.
  *	The low_risk precision is almost 100% with a sensitivity of 57% and a F1 of 73%.

### BalancedRandomForestClassifier Model

![balanced_random_forest.png](https://github.com/SZapata4/Credit_Risk_Analysis/blob/main/Images/balanced_random_forest.png)

  *	The balanced accuracy score is 79%.
  *	The high_risk precision is about 4% with 91% sensitivity which makes a F1 of 7%.
  *	The low_risk precision is almost 100% with a sensitivity of 91% and a F1 of 95%.

### EasyEnsembleClassifier Model

![AdaBoost.png](https://github.com/SZapata4/Credit_Risk_Analysis/blob/main/Images/AdaBoost.png)

  *	The balanced accuracy score is 93%.
  *	The high_risk precision is about 7% with 91% sensitivity which makes a F1 of 14%.
  *	The low_risk precision is almost 100% with a sensitivity of 94% and a F1 of 97%.


## Summary

After evaluating the different models above they all have some sort of short coming in predicting credit risk. Although, the Easy Ensemble Classifier Model does bring back the highest Accuracy Score at 92% and the highest high_risk sensitivity score of 91% of all the models I would still not recommend any of these models to a bank because of the low high_risk precision. The Easy Ensemble Classifier Model again has the highest high_risk precison at 7% but at that number a bank could lose a lot of money by giving out loans that are high_risk without even knowing it.


