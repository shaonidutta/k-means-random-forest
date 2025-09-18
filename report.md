# Heart Disease Prediction and Clustering Analysis Report

1. Key features affecting heart disease -
    - cp - chest pain type
    - thalach - maximum heart rate achieved
    - oldpeak - ST depression induced by exercise relative to rest
    - slope - the slope of the peak exercise ST segment

2. Best-performing classification results- KNN
    - Accuracy: 0.85
    - Precision: 0.86
    - Recall: 0.84
    - F1-score: 0.85
    - ROC-AUC: 0.85

3. Meaningful clusters & their healthcare implications
    - Cluster 1: High risk of heart disease
    - Cluster 2: Medium risk of heart disease
    - Cluster 3: Low risk of heart disease

# Introduction

Heart disease is one of the leading causes of death globally. Early detection and accurate prediction of heart disease can significantly improve patient outcomes. In this project, we aim to develop a machine learning model to predict the presence of heart disease based on various patient attributes. Additionally, we will explore unsupervised clustering techniques to identify hidden patient groups that may have different risk profiles.

# Data Preprocessing and EDA

We started by loading the dataset and performing exploratory data analysis (EDA) to understand the distribution of the features and the target variable. We also checked for missing values and outliers. The dataset did not contain any missing values, but we found some outliers in the 'age' and 'chol' columns. We decided to keep the outliers as they are valid data points.

# Model Training and Evaluation

We trained several classification models on the dataset and evaluated their performance using various metrics. The best-performing model was the K-Nearest Neighbors (KNN) classifier with an accuracy of 85%. We also performed hyperparameter tuning to optimize the model's performance.

# Clustering Analysis

There were 3 meaningful clusters found using K-Means clustering. Cluster 1 had a high risk of heart disease, Cluster 2 had a medium risk, and Cluster 3 had a low risk. The clusters can be used to identify high-risk patients who may benefit from early intervention and monitoring.

# Business/Application Insights

1. Supervised prediction can help in early diagnosis of heart disease.
2. Unsupervised clustering can help in identifying patient sub-groups for better treatment.

# Supervised Prediction

The best-performing model was the K-Nearest Neighbors (KNN) classifier with an accuracy of 85%. The confusion matrix and classification report are shown in the notebook. The model can be used to predict the presence of heart disease in new patients.
The most important features for predicting heart disease are:
    - cp - chest pain type: Patients with typical angina (value 1) have a higher chance of having heart disease.
    - thalach - maximum heart rate achieved: Patients with a higher maximum heart rate have a higher chance of having heart disease.
    - oldpeak - ST depression induced by exercise relative to rest: Patients with a higher ST depression have a higher chance of having heart disease.
    - slope - the slope of the peak exercise ST segment: Patients with a flat slope (value 1) have a higher chance of having heart disease.


# Unsupervised Clustering

There were 3 meaningful clusters found using K-Means clustering. The clusters can be used to identify high-risk patients who may benefit from early intervention and monitoring. As shown in the notebook, the clusters are well-separated and have distinct characteristics. The clusters can be used to identify high-risk patients who may benefit from early intervention and monitoring.
Also, the silhouette score of 0.5 indicates that the clusters are moderately well-separated.
