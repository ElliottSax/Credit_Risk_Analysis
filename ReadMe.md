# Credit Risk Analysis

# Overview of the analysis
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. 
Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. 
Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample
the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. 
Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 
Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier
to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on
whether they should be used to predict credit risk.

# Results:

# -Naive Random Oversampling
Accuracy score: 66%
Predicted High Risk Applicants 1% precision, 69% recall
Predicted Low Risk Applicants 100% precision, 61% recall

# -SMOTE oversampling model
Accuracy score: 66%
Predicted High Risk Applicants 1% precision, 63% recall
Predicted Low Risk Applicants 100% precision, 69% recall

# -Undersampling
Accuracy score: 66%
Predicted High Risk Applicants 1% precision, 69% recall
Predicted Low Risk Applicants 100% precision, 40% recall

# -Combination
Accuracy score: 54%
Predicted High Risk Applicants 1% precision, 72% recall
Predicted Low Risk Applicants 100% precision, 57% recall

# -Balanced Random Forest Classifier
Accuracy score: 77%
Predicted High Risk Applicants 3% precision,  66% recall
Predicted Low Risk Applicants 100% precision, 88% recall

# -Easy Ensemble Classifier
Accuracy score: 91%
Predicted High Risk Applicants 9% precision, 89% recall
Predicted Low Risk Applicants 100% precision, 94% recall


# Summary
The results vary considerably between the models. The accuracy varies from 54 percent to 91 percent. 
Far and away the best model is Easy Ensemble Classifier with an accuracy score of 91 percent and by far the best all around.