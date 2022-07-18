# Credit_Risk_Analysis

### Overview:
We will be analyzing a credit card dataset to determine risk in lending. This type of data is challenging because outcomes (whether the debt will be repaid or not) are heavily skewed. We will use the imbalanced-learn and scikit-learn libraries to build and evaluate model using resampling.  We will test both oversampling, undersampling and a combination of the two in effort to reduce bias and provide accurate predictions.  

### Results: 
1. Naive Random Oversampling 
- balanced accuracy score = 0.625
- precision = 1 for low risk / 0.01 for high risk
- recall = 0.60 for low risk / 0.65 for high risk
- confusion matrix 

![1](https://github.com/lindseyasterman/Credit_Risk_Analysis/blob/main/images/1-randomoversample.png)


2. SMOTE Oversampling
- balanced accuracy score = 0.651
- precision = 1 for low risk / 0.01 for high risk
- recall = 0.66 for low risk / 0.64 for high risk
- confusion matrix 

![2](https://github.com/lindseyasterman/Credit_Risk_Analysis/blob/main/images/2-smoteoversample.png)


3. Cluster Centroids (undersampling)
- balanced accuracy score = 0.529
- precision = 1 for low risk / 0.01 for high risk
- recall = 0.45 for low risk / 0.61 for high risk
- confusion matrix 

![3](https://github.com/lindseyasterman/Credit_Risk_Analysis/blob/main/images/3-undersample.png)

4. SMOTEENN (combonation oversampling and undersampling)
- balanced accuracy score = 0.650
- precision = 1 for low risk / 0.01 for high risk
- recall = 0.58 for low risk / 0.72 for high risk
- confusion matrix 

![4](https://github.com/lindseyasterman/Credit_Risk_Analysis/blob/main/images/4-smoteencombo.png)

5. Balanced Random Forest Classifier
- balanced accuracy score = 0.788
- precision = 1 for low risk / 0.04 for high risk
- recall = 0.91 for low risk / 0.67 for high risk
- confusion matrix 

![5](https://github.com/lindseyasterman/Credit_Risk_Analysis/blob/main/images/5-balancedrandomforest.png)

6. Easy Ensemble AdaBoost Classifier
- balanced accuracy score = 0.925
- precision = 1 for low risk / 0.07 for high risk
- recall = 0.94 for low risk / 0.91 for high risk
- confusion matrix 

![6](https://github.com/lindseyasterman/Credit_Risk_Analysis/blob/main/images/6-easyensembleadaboost.png)


### Summary: 
Each of our machine learning models struggled to overcome the large size dicrepancy in the samples of data.
All models showcased precision in identifying low risk candidates.  Where the models failed was correctly identifying high risk.
The low sensitivity scores demostrate that all models predicted large numbers of false positives.  The Easy Ensemble AdaBoost Classifier
acheived the highest accuracy score of 93% and yet it too contained almost 1,000 false positives.  This bias in creating false positives could lead to discrimination in lending.
I would not reccomend any of these models without further refinement.