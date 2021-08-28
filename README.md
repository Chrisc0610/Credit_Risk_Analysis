# Credit_Risk_Analysis

## Overview of the analysis: 

The purpose of this analysis was to apply machine learning to solve a real-world challenge: credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore,we will need to employ different techniques to train and evaluate models with unbalanced classes. Using imbalance-learn, scikit-learn, we will evaluate the models using resampling.

Then we will oversample the data using the RandomOversampler and Smote Algorithms. Then undersample the data using the ClusterCentroids algorithm. After, we'll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Finally, we’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results: 

- Naive Random Oversampling results:
    * The balanced accuracy score is 65%
    * The percision for high risk is low at  1%
    * with a recall of 69%
    *

- Smote Oversampling results:
    * The accuracy score is 66%
    * The percision for high risk is low at  1%
    * with a recall of 69%


- Undersampling results:
    * The balanced accuracy score is 54%
    * The percision total is at 99%
    * with a recall of 40%


- Combined over and under sampling results:
    * The balanced accuracy score is 54%
    * The percision total is at  99%
    * with a recall of 40% over


- Balanced Random Forest Classifier results:
    * The accuracy score is 78%
    * The percision total is at 99%
    * with a recall of 88%

- Naive Random Oversampling results:
    * The balanced accuracy score is 92%
    * The percision total is at 99%
    * with a recall of 94%

## Summary: 

In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. Typically in your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.

