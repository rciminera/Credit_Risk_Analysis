# Credit_Risk_Analysis

## Overview

The purpose of this analysis is to create supervised machine learning models to predict credit risk and to recommend which model is most effective. A

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Different techniques were employed to train and evaluate models with unbalanced classes.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, three categories of machine learning models were created to predict credit risk:
- Resampling Models which use oversampling and undersampling techniques
- SMOTEEN Combinatorial Model of Over and Undersampling techniques
- Ensemble Classifier Models

JupyterNotebook was used for this analysis along with Imbalanced-learn and scikit-learn machine learning libraries. 

The link to the resampling notebook can be found here: [credit_risk_resampling.ipynb](https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Notebook/credit_risk_resampling.ipynb)

The link to the Ensemble Classifier notebook can be found here: [credit_risk_resampling.ipynb](https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Notebook/credit_risk_resampling.ipynb)




## Results:

There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models 

### I. Resampling Models

Three resampling models were each used to create a predicted outcome and an accuracy score, confusion, matrix, and classification report were created for each, with varying results.

RandomOverSampler Results: 

<img src="https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Screenshots/random_oversampling.png" width = "800" >


<img src="https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Screenshots/smote_oversampling.png" width = "800" >


<img src="https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Screenshots/undersampling.png" width = "800" >



### II. SMOTEENN Combinatorial Model

The SMOTTEEN Combinatorial model of over and undersampling was then used to create a predicted outcome and an accuracy score, confusion, matrix, and classification report.  Of all the sampling models, this delivered the best accuracy result.

<img src="https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Screenshots/combination.png" width = "800" >


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