# Credit_Risk_Analysis
Imbalanced-learn library, supervised learning, Scikit-learn machine learning library for Python (sklearn), supervised learning in linear models (linear regression; logistic regression), Accuracy/Precision/sensitivity(recall)/F1 score, confusion matrix, SVM(Support Vector Machine – support vector, hyperplane), data preprocessing: - labelling (encoding),  - Data Scale: Normalization (Standard scaler – mean = 0, variance = 1), Decision Trees, Ensemble Learning – Random Forest (weak/moderate/strong learner), Bootstrap Aggregation, Boosting: Adaptive boosting (AdaBoost), Gradient Boosting, for Class imbalance (solution 1: Oversampling (Random oversampling, synthetic minority oversampling technique (SMOTE)), solution 2: Undersampling (Random undersampling, Cluster Centroid undersampling, solution 3: SMOTEENN)

## Overview of the Project
Credit risk is an inherently unbalanced classificaiton problem. The project uses multiple supervised learning techniques (imbalanced-learn, scikit-learn library) to train and evaluate models with unbalanced classes. Due to the imbalanced amount of data, oversampling/undersampling/SMOTEENN (combination) will be applid to address the imbalance issue. Then data gets splitted into training and testing data for model performance assessment. The analysis applies Naive Random Oversampling, SMOTE Oversampling, Cluster Centroid undersampling, SMOTEENN resampling, Random Forest Classifier and Adapt Boost Classifier to predict the credit risk. In the end the analysis evaluate the performance of each model and provide recommendation for credit risk assessment.

## Result
- Naive Random Oversampling
Accuracy Score:  
![naive_random_oversampling_acc.PNG](image/naive_random_oversampling_acc.PNG)  
Confusion Matrix:  
![naive_random_oversampling_cm.PNG](image/naive_random_oversampling_cm.PNG)  
Classification Report:
![naive_random_oversampling_classification_report.PNG](image/naive_random_oversampling_classification_report.PNG)  
- SMOTE
Accuracy Score:  
![smote_acc.PNG](image/smote_acc.PNG)  
Confusion Matrix:  
![smote_cm.PNG](image/smote_cm.PNG)  
Classification Report:  
![smote_classification_report.PNG](image/smote_classification_report.PNG)  
- Cluster Centroids Undersampling  
Accuracy Score:  
![ccr_acc.PNG](image/ccr_acc.PNG)  
Confusion Matrix:  
![ccr_cm.PNG](image/ccr_cm.PNG)  
Classification Report:  
![ccr_classification_report.PNG](image/ccr_classification_report.PNG)  
- SMOTEENN Resampling:
Accuracy Score:  
![smoteenn_acc.PNG](image/smoteenn_acc.PNG)  
Confusion Matrix:  
![smote_cm.PNG](image/smote_cm.PNG)  
Classification Report:  
![smoteenn_classification_report.PNG](image/smoteenn_classification_report.PNG)  
- Balanced Random Forest Classifier  
Accuracy Score:  
![brf_acc.PNG](image/brf_acc.PNG)  
Confusion Matrix:  
![brf_cm.PNG](image/brf_cm.PNG)  
Classification Report:  
![brf_classification_report.PNG](image/brf_classification_report.PNG)  
- Adaptive Boost Classifer:  
Accuracy Score:  
![adaboost_acc.PNG](image/adaboost_acc.PNG)  
Confusion Matrix:  
![adaboost_cm.PNG](image/adaboost_cm.PNG)  
Classification Report:  
![adaboost_classification_report.PNG](image/adaboost_classification_report.PNG)  

## Summary
Through the analysis above, Adaptive Boosting (Adaboost) classifier should be recommended to use to assess credit risk as the precision to assess "high risk" category is relatively better compared to the rest of the models. Besides, the sensitivity for Adaboost also has the highest score for both "low risk" and "high risk". It is not recommended to use "Cluster Centroids Undersampling" as both the precision and sensitivity behave the worst compared to the rest of the models.
