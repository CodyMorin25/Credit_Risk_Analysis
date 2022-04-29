# Credit_Risk_Analysis

## Overview of the Analysis

### Purpose

Using a credit card credit dataset from LendingClub(hypothetical), a peer-to-peer lending services company. We oversample the data using RandomOverSampler and SMOTE algorithims. Then undersample the data using the ClusterCentroids algorithim. Next use a combination of over- and undersampling using the SMOTEENN algorithm. Lastly compare two maching learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, in order to predict credit risk.

## Results

#### Naive Random Oversampling
  - Balanced Accuracy = 0.6477019551913493
  - Precision
    - High Risk = Precision is very low for High Risk loans at 0.01
    - Low Risk = Precision is very high for Low Risk loans at 1.00
  - Recall
    - High Risk = 0.63
    - Low Risk = 0.66
![NRO](https://github.com/CodyMorin25/Credit_Risk_Analysis/blob/main/Images/Naive_Random_Oversampling.png)

#### SMOTE Oversampling
  - Balanced Accuracy = 0.635499635390857
   - Precision
    - High Risk = Precision is very low for High Risk loans at 0.01
    - Low Risk = Precision is very high for Low Risk loans at 1.00
  - Recall
    - High Risk = 0.62
    - Low Risk = 0.65
![SMOTE](https://github.com/CodyMorin25/Credit_Risk_Analysis/blob/main/Images/SMOTE_Oversampling.png)

#### Undersampling
  - Balanced Accuracy = 0.5212843105261249
   - Precision
    - High Risk = Precision is very low for High Risk loans at 0.01
    - Low Risk = Precision is very high for Low Risk loans at 1.00
  - Recall
    - High Risk = 0.59
    - Low Risk = 0.46
![UnderSampling](https://github.com/CodyMorin25/Credit_Risk_Analysis/blob/main/Images/Undersampling.png)

#### Combination Over/Under Sampling
  - Balanced Accuracy = 0.6081902091365814
   - Precision
    - High Risk = Precision is very low for High Risk loans at 0.01
    - Low Risk = Precision is very high for Low Risk loans at 1.00
  - Recall
    - High Risk = 0.67
    - Low Risk = 0.55
![Over/Under](https://github.com/CodyMorin25/Credit_Risk_Analysis/blob/main/Images/Over_Under_Sampling.png)

#### Balanced Random Forest Classifier
  - Balanced Accuracy = 0.795829959187949
   - Precision
    - High Risk = Precision changes slightly but is still very low for High Risk loans at 0.03
    - Low Risk = Precision is very high for Low Risk loans at 1.00
  - Recall
    - High Risk = 0.71
    - Low Risk = 0.88
![BRLC](https://github.com/CodyMorin25/Credit_Risk_Analysis/blob/main/Images/Balanced_Random_Forest_Classifier.png)

#### Easy Ensemble AdaBoost Classifier
  - Balanced Accuracy = 0.9263912558266958
   - Precision
    - High Risk = Precision changes slightly also but is still very low for High Risk loans at 0.08
    - Low Risk = Precision is very high for Low Risk loans at 1.00
  - Recall
    - High Risk = 0.91
    - Low Risk = 0.94
![Ensemble](https://github.com/CodyMorin25/Credit_Risk_Analysis/blob/main/Images/Easy_Ensemble_AdaBoost_Classifier.png)

# Summary

When Undersampling the data using the Cluster Centroids algorithm it yielded the lowest balanced accuracy score of 0.5212843105261249. The precision scores for predicting high risk was low and scores for predicting low risk was high for all six models. The Easy Ensemble Classifier gave the highest balanced accuracy score of 0.9263912558266958 and gave the highest recall scores of 0.91 and 0.94 for high and low risk. I would recommend using the Easy Ensemble Classifier because of the six models it yielded the better results. However the company should take into account the high risk precision score. With a score of 0.09 means it is not all that reliable.
