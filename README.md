# Credit Card Fraud Detection

## Problem Statement:
- It has been estimated by Nilson Report that by 2020, banking frauds would account for **$30 billion** worldwide. With the rise in digital payment channels, the number of fraudulent transactions is also increasing in new and different ways. 
- Fraudulent activities in India have increased severalfold, with approximately **52,304** cases of credit/debit card fraud reported in FY 2019 alone.
- Owing to this steep increase in banking frauds, it is the need of the hour to detect these fraudulent transactions in time to help consumers and banks that are losing their credit worth each day.
- Banks need to be cautious about their customers’ transactions, as they cannot afford to lose their customers’ money to fraudsters.
- Every fraud is a loss to the bank, as the bank is responsible for the fraudulent transactions if they are reported within a certain time frame by the customer.

## Objective:
- The aim of this project is to **predict fraudulent credit card transactions using machine learning models.**

## Dataset
- Out of a total of **2,84,807** transactions, **492** were fraudulent. 
- This data set is **highly unbalanced**, with the positive class (frauds) accounting for **0.172%** of the total transactions.   

## Project Pipeline:
1. **Importing Libraries**
2. **Data Understanding:**
    - Load
    - Describe
    - Distribution
    - Info
3. **Exploratory data analytics (EDA)**
    - Missing Values
    - Outliers
    - Skewness
4. **Train/Test split**
5. **Model building**
    - Logistic Regression
    - Decision Tree
    - Random Forest
6. **Model building with balancing Classes**
    - Logistic Regrassion with Random Oversampling
	- Decision Tree with Random Oversampling
	- Decision Tree with optimal hyperparameters
	- XGBoost with Random Oversampling
    - Logistic Regression on balanced data + SMOTE
	- Logistic Regression with optimal C
	- Decision Tree on balanced data + SMOTE
	- XGBoost on balanced data + SMOTE
    - Logistic Regression on balanced data with ADASYN
	- Decision Tree on balanced data with ADASYN
	- XGBoost on balanced data + ADASYN
6. **Hyperparameter Tuning**
7. **Model Evaluation**
8. **Conclusion**

# Conclusion:
- We have to foucs more on the **RECALL** for the farudlant instances
- We get **100%** ROC score on the train data.
- TPR is the highest and FPR is the lowest as **90%** is the threshold
- We concluded that in the **BALANCED DATASET** with **ADASYN** technique the **XGBoost** model has good ROC score(**99%**) and also high Recall(**86%**).Hence, we can go with the **XGBoost** model here.
