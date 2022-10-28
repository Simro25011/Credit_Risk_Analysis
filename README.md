# Credit_Risk_Analysis

## Overview
Credit risk is inherently an unbalanced classification problem, and good credit easily trumps risky credit. Therefore, we need to apply different techniques to train and evaluate models with imbalanced classes.

Using the credit card loan dataset from LendingClub, a P2P lending service, we will oversample the data using the RandomOverSampler and SMOTE algorithms and undersample the data using the ClusterCentroids algorithm. Then we use the combined oversampling and undersampling method of the SMOTEENN algorithm. Next, we compared two new machine learning models with reduced bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once completed, we will evaluate the performance of these models and provide written recommendations on whether they should be used to predict credit risk.


## Results
### Oversampling

- Naive Random Oversampling

![Naive Random Oversampling](https://github.com/Simro25011/Credit_Risk_Analysis/blob/main/Resources/oversampling.png)

- SMOTE Oversampling
- 
![SMOTE Oversampling](https://github.com/Simro25011/Credit_Risk_Analysis/blob/main/Resources/Smote.png)

### Undersampling

![Undersampling](https://github.com/Simro25011/Credit_Risk_Analysis/blob/main/Resources/undersampling.png)

### Combination (Over and Under) Sampling

![Combination (Over and Under) Sampling](https://github.com/Simro25011/Credit_Risk_Analysis/blob/main/Resources/Combination.png)

### Ensemble Learners

- Balanced Random Forest Classifier

![Balanced Random Forest Classifier](https://github.com/Simro25011/Credit_Risk_Analysis/blob/main/Resources/Balanced%20random.png)

- Easy Ensemble AdaBoost Classifier

![Easy Ensemble AdaBoost Classifier](https://github.com/Simro25011/Credit_Risk_Analysis/blob/main/Resources/easy%20ensemble.png)


