# Credit_Risk_Analysis

## Overview

The purpose of this analysis is to create machine learning models to predict credit risk.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Different techniques were employed to train and evaluate models with unbalanced classes. Imbalanced-learn and scikit-learn libraries were used to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, six machine learning models were created to predict credit risk:

1.  Oversampling using the RandomOverSampler and SMOTE algorithms
2.  Oversampling using the SMOTE algorithms
3.  Undersampling using the ClusterCentroids algorithm
4.  Combinatorial approach of over- and undersampling using the SMOTEENN algorithm
5.  Bias reduction usinng BalancedRandomForestClassifier
6.  Bias reduction using EasyEnsembleClassifier

The performance of these models was then evaluated and a recommendation was made on whether they should be used to predict credit risk.

## Results:

There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models 

### I. Resampling Models to Predict Credit Risk

For all three algorithms, the following have been completed:
- An accuracy score for the model is calculated 
- A confusion matrix has been generated
- An imbalanced classification report has been generated

### II. SMOTEENN algorithm  to Predict Credit Risk

The combinatorial SMOTEENN algorithm does the following:
- An accuracy score for the model is calculated 
- A confusion matrix has been generated
- An imbalanced classification report has been generated 

### III. Use Ensemble Classifiers to Predict Credit Risk

The BalancedRandomForestClassifier algorithm does the following:
- An accuracy score for the model is calculated 
- A confusion matrix has been generated
- An imbalanced classification report has been generated
- The features are sorted in descending order by feature importance

The EasyEnsembleClassifier algorithm does the following:
- An accuracy score of the model is calculated
- A confusion matrix has been generated
- An imbalanced classification report has been generated


## Summary:

There is a summary of the results

There is a recommendation on which model to use, or there is no recommendation with a justification