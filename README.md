# Credit_Risk_Analysis

## Overview
Credit risk is inherently an unbalanced classification problem, and good credit easily trumps risky credit. Therefore, we need to apply different techniques to train and evaluate models with imbalanced classes.

Using the credit card loan dataset from LendingClub, a P2P lending service, we will oversample the data using the RandomOverSampler and SMOTE algorithms and undersample the data using the ClusterCentroids algorithm. Then we use the combined oversampling and undersampling method of the SMOTEENN algorithm. Next, we compared two new machine learning models with reduced bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once completed, we will evaluate the performance of these models and provide written recommendations on whether they should be used to predict credit risk.


## Results

### Oversampling

#### Naive Random Oversampling

![Naive Random Oversampling](https://github.com/Simro25011/Credit_Risk_Analysis/blob/main/Resources/oversampling.png)

- Balanced Accuracy: 0.6366972052004142
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall: High/Low risk = .62/.65

#### SMOTE Oversampling

![SMOTE Oversampling](https://github.com/Simro25011/Credit_Risk_Analysis/blob/main/Resources/Smote.png)

- Balanced Accuracy: 0.6302712208564487.
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall: High/Low risk = .62/.64

### Undersampling

![Undersampling](https://github.com/Simro25011/Credit_Risk_Analysis/blob/main/Resources/undersampling.png)

- Balanced Accuracy: 0.590320332297924
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall: High/Low risk = .61/.57

### Combination (Over and Under) Sampling

![Combination (Over and Under) Sampling](https://github.com/Simro25011/Credit_Risk_Analysis/blob/main/Resources/Combination.png)

- Balanced Accuracy: 0.6375533316412246
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall: High/Low risk = .70/.57

### Ensemble Learners

#### Balanced Random Forest Classifier

![Balanced Random Forest Classifier](https://github.com/Simro25011/Credit_Risk_Analysis/blob/main/Resources/Balanced%20random.png)

- Balanced Accuracy: 0.7877672625306695
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall: High/Low risk = .67/.91

#### Easy Ensemble AdaBoost Class

![Easy Ensemble AdaBoost Classifier](https://github.com/Simro25011/Credit_Risk_Analysis/blob/main/Resources/easy%20ensemble.png)

- Balanced Accuracy: 0.925427358175101
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall: High/Low risk = .91/.94

## Summary
When working with balanced accuracyy score, the range is between 0 and 1, with the closest to 1 being the best machine learning model. For credit card records, the Easy Ensemble AdaBoost Classifier has a balanced accuracy of 0.93 and is the best choice model. The balance accuracy of the other models is below 0.9. The accuracy of all models is similar and within a reasonable range. The recall value must also be between 0 and 1, numbers closer to 1 are better models. The Easy Ensemble AdaBoost classifier had the highest recall score, making it the final choice for the best machine learning model for further credit card analysis.
