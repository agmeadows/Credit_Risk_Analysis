# Credit_Risk_Analysis
 
## Overview

The purpose of this analysis is to assess the credit risk of individuals based on a number of features. Three machine learning models were used to assess risk. Each model is evaluated for performance.

## Results

### Resampling Models

#### RandomOversampler

    - Accuracy: 0.74
    - Precision:
        - low_risk: 1.00
        - high_risk: 0.01
    - Recall: 
        - low_risk: 0.74
        - high_risk: 0.53

##### Classification Report:
![RandomForest](Resources/Randover_report.PNG)

#### SMOTE Oversampling

    - Accuracy: 0.64
    - Precision:
        - low_risk: 1.00
        - high_risk: 0.01
    - Recall: 
        - low_risk: 0.66
        - high_risk: 0.63

##### Classification Report:
![RandomForest](Resources/SMOTE_report.PNG)

#### ClusterCentroid Undersampling

    - Accuracy: 0.64
    - Precision:
        - low_risk: 1.00
        - high_risk: 0.01
    - Recall: 
        - low_risk: 0.66
        - high_risk: 0.63

##### Classification Report:
![RandomForest](Resources/Cluster_report.PNG)

#### SMOTEENN Combination

    - Accuracy: 0.64
    - Precision:
        - low_risk: 1.00
        - high_risk: 0.01
    - Recall: 
        - low_risk: 0.66
        - high_risk: 0.63

##### Classification Report:
![RandomForest](Resources/SMOTEEN_report.PNG)

#### RandomForest Classifier

    - Accuracy: 0.86
    - Precision:
        - low_risk: 1.00
        - high_risk: 0.02
    - Recall: 
        - low_risk: 0.86
        - high_risk: 0.64

##### Classification Report:
![RandomForest](Resources/Randomforest_report.PNG)

#### AdaBoost Classifier

    - Accuracy: 0.86
    - Precision:
        - low_risk: 1.00
        - high_risk: 0.03
    - Recall: 
        - low_risk: 0.86
        - high_risk: 0.82

##### Classification Report:
![RandomForest](Resources/Randomforest_report.PNG)

## Summary

After evaluating each of the machine learning methods, it has been determined that AdaBoost Boostrapping provides the best results. The undersampling and oversampling methods have an accuracy far below either of the Ensemble strategies. It for this reason I would recommend using the AdaBoost method for determining credit risk.

