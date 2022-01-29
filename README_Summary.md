# Unit 11 - Risky Business

## Summary of Models and Findings
 
![Credit Risk](Images/credit-risk.jpg)

## Background

Mortgages, student and auto loans, and debt consolidation are just a few examples of credit and loans that people seek online. Peer-to-peer lending services such as Loans Canada and Mogo let investors loan people money without using a bank. However, because investors always want to mitigate risk, a client has asked that you help them predict credit risk with machine learning techniques.

In this assignment I will build and evaluate several machine learning models to predict credit risk using data you'd typically see from peer-to-peer lending services. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans). I have employed different techniques for training and evaluating models with imbalanced classes. I have used the imbalanced-learn and Scikit-learn libraries to build and evaluate models using the two following techniques:

1. [Resampling](#Resampling)
2. [Ensemble Learning](#Ensemble-Learning)

# Summary 

## Credit Risk Resampling Techniques - Final Questions

1. Which model had the best balanced accuracy score?

    - 0.9892813049736127 - Simple Logistic Regression
    - 0.9946414201183431 - Naive Random Oversampling
    - **0.9946680739911509 - SMOTE Oversampling**
    - 0.9932813049736127 - Undersampling
    - **0.9946680739911509 - Combination (Over and Under) Sampling**
    
    **ANSWER:** Examining the figures above it can bee seen that the **SMOTE Oversampling** and the **Combination (Over and Under) Sampling** models had the equal best balanced accuracy scores.

2. Which model had the best recall score?

    - 0.9942220387948824  - Simple Logistic Regression
    - 0.9941188609162196 - Naive Random Oversampling
    - 0.9941704498555509 - SMOTE Oversampling
    - **0.9944799834915394  - Undersampling**
    - 0.9941704498555509  - Combination (Over and Under) Sampling
    
    **ANSWER:** Examining the figures above it can bee seen that the **Undersampling** model had the best recall score.

3. Which model had the best geometric mean score?

    - 0.9892672076785270 - Simple Logistic Regression
    - 0.9946412632721158 - Naive Random Oversampling
    - **0.9946679317601361 - SMOTE Oversampling**
    - 0.9932804785495624 - Undersampling
    - **0.9946679317601361 - Combination (Over and Under) Sampling**
    
    **ANSWER:** Examining the figures above it can bee seen that the **SMOTE Oversampling** and the **Combination (Over and Under) Sampling** had the equal best geometric scores.

## Ensemble Learning - Final Questions

1. Which model had the best balanced accuracy score?

    - 0.67209249388625 - Balanced Random Forest Classifier
    - **0.9254565671948463 - Easy Ensemble Classifier**
    
    **ANSWER:** Examining the figures above it can bee seen that the **Easy Ensemble Classifier** model had the best balanced accuracy score.

2. Which model had the best recall score?

    - **0.9960476605637896 - Balanced Random Forest Classifier**
    - 0.9426910781749491 - Easy Ensemble Classifier
    
    **ANSWER:** Examining the figures above it can bee seen that the **Balanced Random Forest Classifier** model had the best recall score.

3. Which model had the best geometric mean score?

    - 0.5870315157978003 - Balanced Random Forest Classifier
    - **0.9252927802125857 - Easy Ensemble Classifier**
    
    **ANSWER:** Examining the figures above it can bee seen that the **Easy Ensemble Classifier** model had the best geometric mean score. had the equal best geometric scores.

4. What are the top three features?

     **ANSWER:** The following lists the top three features
         - total_rec_prncp 
         - total_pymnt
         - total_pymnt_inv