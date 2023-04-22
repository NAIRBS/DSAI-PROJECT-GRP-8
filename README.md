# Welcome to Stroke Prediction Repository
## About
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on patient data from [kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset), for stroke prediction.

Please view the source code [here](https://google.com)

## Contributors
* @NAIRBS (Brian Soh) - Data Extraction, Data Visualization, Random Forests, GridSearch
* Yee Shem - Data Visualization, Data oversampling (SMOTE)
* Angelo - Categorical Encoding, Decision Trees

## Problem Definition
### Can we use one’s lifestyle to predict if they have a stroke?

## Models Used
1. Decision Tree
2. Random Forest
3. GridSearch

## Conclusion
* We can tell that there is probably a positive correlation for BMI and avg_glucose level to stroke likelihood.
* It is difficult to tell what categorical variables are correlated with stroke likelihood as the dataset is unbalanced.
* It is difficult to accurately predict True Positives (stroke patients) based on the data as there simply isn't enough data about stroke patients compared to non-stroke patients even after oversampling with SMOTE.
* Applying hyperparameter tuning did not help much in terms of raising accuracy rate or True Positive rates, this could show that the data we are using are heavily unbalanced and biased in terms of non-stroke patients.
* In short, due to unbalanced and insufficient data on stroke patients, we are unable to achieve an accuracy higher than 92.5% (Decision Tree), which, despite sounding good, fails to predict those with strokes as True Positive rates were at best 17% (Decision Tree).
* Therefore, we conclude that we were not able to use one's lifestyle to predict with certainty if they would have a stroke.

## What we have learnt from this project
* How to handle inbalanced datasets using SMOTE oversampling techniques
* How to avoid overfitting by using Random Forest Model
* GridSearch Parameter Hypertuning

## References
### **Dataset Used:**
https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

### **EDA:**
#### **Diabetic Blood Sugar Levels:** 
**https://www.cdc.gov/diabetes/basics/getting-tested.html#:~:text=A%20fasting%20blood%20sugar%20level,higher%20indicates%20you%20have%20diabetes.**

#### **How to handle unknown categorical data:**
**https://medium.com/analytics-vidhya/ways-to-handle-categorical-column-missing-data-its-implementations-15dc4a56893**

#### **Hold out cross validation:**
**https://www.mygreatlearning.com/blog/cross-validation/**

#### **How we identify outliers:**
**https://www.pluralsight.com/guides/cleaning-up-data-from-outliers**

#### **SMOTE:**
#### **https://www.analyticsvidhya.com/blog/2020/10/overcoming-class-imbalance-using-smote-techniques/**
---

### **Decision Tree:**
### **https://scikit-learn.org/stable/modules/tree.html**
---

### **Random Forests:**
### **https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html**
---
### **Tuning Hyperparameters with RandomSearchCV:**
### **https://www.geeksforgeeks.org/random-forest-hyperparameter-tuning-in-python/**

