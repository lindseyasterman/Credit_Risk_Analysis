# Credit_Risk_Analysis

### Overview:
We will be analyzing a credit card dataset to determine risk in lending. This type of data is challenging because outcomes (whether the debt will be repaid or not) are heavily skewed.  
We will use the imbalanced-learn and scikit-learn libraries to build and evaluate model using resampling.  We will test both oversampling, undersampling and a combination of the two looking 
to reduce bias and provide accurate predictions.  

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



3.
4.
5.
6.

### Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)