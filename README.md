# Credit_Risk_Analysis

## Project Overview
Using the different techniques I've learned, such as imbalanced-learn and scikit-learn libraries, I'll apply them to train and evaluate models with unbalanced classes. Using the credit card credit dataset from LendingClub, I will:
  1. Oversamplethe data using the RandomOverSampler and SMOTE algorithms
  2. Undersample the data using the ClusterCentroids algorithm
  3. Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm
  4. Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier to predict credit risk

## Results
  - Naive Random Oversampling

![Naive Random Oversampling](https://user-images.githubusercontent.com/110737061/206319418-fa34806d-3cc7-4db0-9391-07cba009e950.png)

    - Balance Accuracy Score (BAS): 64.7%
    - Precision: 99% / Recall: 67%
    - High Risk: 1% / Recall: 62%
    
  - SMOTE Oversampling

![SMOTE Oversampling](https://user-images.githubusercontent.com/110737061/206319454-0238cf70-1964-4ec6-84ca-99719a318c6b.png)

    - Balance Accuracy Score (BAS): 62.5%
    - Precision: 99% / Recall: 63%
    - High Risk: 1% / Recall: 62%

  - Undersampling

![Undersampling](https://user-images.githubusercontent.com/110737061/206319502-12813140-ec05-4d4d-ad22-ef7590422587.png)

    - Balance Accuracy Score (BAS): 51.3%
    - Precision: 99% / Recall: 43%
    - High Risk: 1% / Recall: 60%

  - Combination Sampling

![Combination](https://user-images.githubusercontent.com/110737061/206319555-d883713c-54b8-42f9-820f-5777d4256308.png)

    - Balance Accuracy Score (BAS): 51.3%
    - Precision: 99% / Recall: 58%
    - High Risk: 1% / Recall: 70%

  - Balanced Random Forest Classifier

![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/110737061/206319606-8c261c0d-1ab9-450d-934c-d5e2047776cc.png)

    - Balance Accuracy Score (BAS): 78.9%
    - Precision: 99% / Recall: 87%
    - High Risk: 3% / Recall: 70%

  - Easy Ensemble AdaBoost Classifier

![Easy Ensemble AdaBoost Classifier](https://user-images.githubusercontent.com/110737061/206319805-489a90a9-ce88-49e7-8e8f-af3c70d3e398.png)

    - Balance Accuracy Score (BAS): 93.2%
    - Precision: 99% / Recall: 94%
    - High Risk: 9% / Recall: 92%

## Summary
Looking at the data we've gathered, we notice that there is low precision based off the amount of high risk. This could indicate a number of false positives. Based off the data, Easy Ensemble AdaBoost Classifier is probably the most reliable and effective of all the models.
