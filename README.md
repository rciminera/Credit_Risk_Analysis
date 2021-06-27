# Credit_Risk_Analysis

## Overview

The purpose of this analysis is to create supervised machine learning models to predict credit risk and to recommend which model is most effective. 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Different techniques were employed to train and evaluate models with unbalanced classes.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, three categories of machine learning models were created to predict credit risk:
- Resampling Models which use oversampling and undersampling techniques
- SMOTEEN Combinatorial Model of Over and Undersampling techniques
- Ensemble Classifier Models

JupyterNotebook was used for this analysis along with Imbalanced-learn and scikit-learn machine learning libraries. 

The link to the resampling notebook can be found here: [credit_risk_resampling.ipynb](https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Notebook/credit_risk_resampling.ipynb)

The link to the Ensemble Classifier notebook can be found here: [credit_risk_resampling.ipynb](https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Notebook/credit_risk_resampling.ipynb)




## Results:

Following are the results of the six supervised machine learning models.

### I. Resampling Models

Three resampling models were each used to create a predicted outcome.  These models were: Random Oversampling, SMOTE Oversampling, and Undersampling.  A balanced accuracy score, confusion, matrix, and balanced classification report were created for each, with varying results. 


<img src="https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Screenshots/random.png" width = "800" >




<img src="https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Screenshots/smote.png" width = "800" >



<img src="https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Screenshots/undersampling.png" width = "800" >



### II. SMOTEENN Combinatorial Model

The SMOTTEEN Combinatorial model of over and undersampling was then used to create a predicted outcome and an accuracy score, confusion, matrix, and classification report.  Of all the sampling models, this delivered the best accuracy result.

<img src="https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Screenshots/smoteenn.png" width = "800" >


### III. Use Ensemble Classifiers to Predict Credit Risk


<img src="https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Screenshots/bal_rfc.png" width = "800" >



<img src="https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Screenshots/easy_ensemble.png" width = "800" >


## Summary:

Based on the results of the six different supervised machine learning models, the recommended model to use for the determination of credit risk is the EasyEnsemble Classifier.  With an accuracy score of 93.17%, the EasyEnsmble Classifier outperformed the other five models in the analysis by a significant margin.

<img src="https://github.com/rciminera/Credit_Risk_Analysis/blob/main/Screenshots/bac_comparsion.png" width = "400">


#
#

### Appendix

Glossary of Definitions:

Precision or "pre": Precision is the ratio of correctly predicted positive classes to the total number of positively predicted classes. The formula for precision is
Precision = TP/(TP+FP) where TP is the number of true positives and FN is the number of false negatives.

Recall of "rec":  Also know as sensitivity is the ratio TP / (TP + FN).   The sensitivity quantifies the ability to avoid false negatives

Specificity or "spe":  The specificity is the ratio TN / (TN + FP). The specificity quantifies the ability to avoid false positives.

F1: F1-score is the harmonic mean of precision and recall. The formula for F1-score is F1-score = 2*Precision*Recall/(Precision+Recall)

Geometric Mean or "geo:  Geometric mean is the square root of the product of Recall and Specificity. The formula for Geometric Mean is
Geometric Mean = √(Recall*Specificity) or Geometric Mean = √(True Positive Rate * True Negative Rate)


Index of Balanced Accuracy or "iba": t is a new metric for measuring performance. First of all Dominance is calculated which is the difference of True Positive Rate and True Negative Rate. The formula is Dominance = Recall-Specificity. The value of dominance is assigned a weight α. The formula of Index Balanced Accuracy (IBA) is IBA = (1 + α*Dominance)(GMean²). In simplified terms it is
IBA = (1 + α*(Recall-Specificity))*(Recall*Specificity)
Note: default value for α is .1

Support or "sup": The support is the number of occurrences of each class in y_true