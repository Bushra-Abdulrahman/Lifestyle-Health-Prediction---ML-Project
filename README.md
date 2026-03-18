# Lifestyle & Health Prediction - ML Project

A machine learning project built on the BRFSS 2013 dataset to analyze and predict lifestyle-related health patterns using supervised and unsupervised learning.

# Project Overview
This project applies a full ML pipeline to the Behavioral Risk Factor Surveillance System (BRFSS) dataset (~500K records, ~300 features) to classify individuals into healthy/unhealthy lifestyle groups and predict key behavioral health outcomes.

# Objectives
 ∙ Predict behavioral health targets: weight, sleep time, and vegetable consumption
 ∙ Classify individuals by diabetes risk: Non-Diabetic, At-Risk, Diabetic
 ∙ Cluster individuals based on lifestyle patterns

🗂️ Report Contents

|Section|Topic                                                                              |
|-------|-----------------------------------------------------------------------------------|
|1      |Abstract & Introduction                                                            |
|2      |Dataset & Domain Description                                                       |
|3      |Theoretical Background — Linear Regression, Decision Tree, K-Means                 |
|4      |Methodology — Preprocessing Pipeline, Supervised & Unsupervised Models             |
|5      |Results & Evaluation                                                               |
|6      |Extra Models — KNN, Gradient Boosting, Random Forest, XGBoost, Hierarchical, DBSCAN|
|7      |Discussion & Conclusion                                                            |


# Dataset
BRFSS 2013 — Available on Kaggle 
* ~500,000 records
* ~300 features
* Domain: Behavioral health surveillance (US adults)
* Link: https://www.kaggle.com/datasets/nguyenngocphung/behavioral-risk-factor-surveillance-system2013?select=brfss2013.csv

# Preprocessing Pipeline
* Drop irrelevant columns
* Handle missing values
* Handle outliers & scaling
* Encoding
* Feature Selection / Extraction

# Models Used
Supervised:
* Linear Regression
* Decision Tree Classifier
* KNN
* Random Forest
* XGBoost
* Gradient Boosting Regressor


Unsupervised:
* K-Means Clustering
* Hierarchical Clustering
* DBSCAN



# Key Results

* Regression:  Weight prediction gave the best result (R² = 0.71), vegetables were moderate (R² = 0.63), and sleep time was unpredictable across all models (R² ≈ 0.00).
* Classification: XGBoost was the best classifier at 99.4%, followed by Decision Tree at 98.13%. All models struggled with the At-Risk class due to data imbalance.
* Clustering: Hierarchical clustering was the most useful, revealing 3 groups — Healthy, Unhealthy, and Stressed. DBSCAN only detected outliers without meaningful separation.|

