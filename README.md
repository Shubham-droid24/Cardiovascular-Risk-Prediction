# Capstone-Project-3-Classification
Cardiovascular Risk Prediction



![image](https://github.com/Shubham-droid24/Cardiovascular-Risk-Prediction/assets/72461022/c4e60fa9-353c-455f-9ed4-6ec2f5070ed6)


I have built machine learning models solving a classification problem to identify whether a patient has a 10-year risk of future coronary heart disease. I have used K-Nearest Neighbours, Support Vector Classifier and Random Forest Classifier to solve the problem and got the best results with the K-Nearest Neighbours.

## Problem Statement

The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts.
The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD).
The dataset provides the patients’ information. It includes over 4,000 records and 15 attributes. Variables Each attribute is a potential risk factor. There are both demographic, behavioral, and medical risk factors.

## Why do we need to do this project?

Cardiovascular disease is the leading cause of death worldwide and a major public health concern. Therefore, its risk assessment is crucial to many existing treatment guidelines. Risk estimates are also being used to predict the magnitude of future cardiovascular disease mortality and morbidity at the population level and in specific subgroups to inform policymakers and health authorities about these risks. Additionally, risk prediction inspires individuals to change their lifestyle and behaviour and to adhere to medications.

This project involves solving a real-world medical problem of predicting coronary heart disease for a patient in future and building up machine learning models for the same.

## Summary

I have summarized the project in 4 steps that how the flow of the project goes:-

First, I understood the Cardiovascular risk dataset in which we are provided with patients information from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. I understood all the variables and how they can be important to the target variable i.e Ten Year CHD.

Second, From Heart Rate column and BMI column(numerical), created new columns named Heart Rate Label and BMI Label which classify the Heart Rate as Low, Normal or High and the BMI as Underweight, Healthyweight, Overweight or Obese respectively in order to use them for visualization purpose.

In visualization, I started from univariate analysis to bivariate and multivariate analysis and in every visualization comparing TenYearCHD with other variables in order to understand the relation and impact or importance of them. From the visualization, I defined and tested three hypothesis and rejected all of them as p-value was less than significance level.

Third, I have done preprocessing which is important before model implementation. In this, I handled missing values and treated outliers , encoding the categorical variables, some feature engineering selection done on the basis of correlation to create new features and remove old ones.

After having selection of important features I transformed some of them, done data splitting and feature scaling. All these were important to be done as they create a great impact on the model performance.

Last, I build different models and predicted whether patient is at risk of Ten Year CHD or not and compared the results of different models developed. Also, I found the most important features required to predict patient is at risk of Ten Year CHD.

## Conclusions

Some important conclusions drawn from the project are as follows:

### From Visualization:

1) Patients after the age of 50 are more prone to Coronary Heart Disease(CHD).

2) Cholestrol level is not the sole deciding factor for predicting whether the person gets coronary heart disease or not. People with similar levels of cholestrol have got coronary heart disease as well as are free from coronary heart disease.

3) SysBP and DiaBP have an effect on the risk of CHD but there is not a significant effect.

4) BMI and Heart Rate have an effect on the risk of CHD

5) Diabetes and Glucose level have an effect on the risk of CHD.

### From Hypothesis Testing :

1) The mean BMI of people with heart disease is not less than or equal to the mean BMI of people without heart disease.

2) The mean Heart Rate of people with heart disease is not less than or equal to the mean Heart Rate of people without heart disease.

3) The mean Cholestrol of people with heart disease is not less than or equal to the mean cholestrol of people without heart disease.

### From Model Implementation :

K-Nearest Neighbours(K-NN) Classifier Model using hyperparameter optimization technique(GridSearchCV) gave the best result of F1-score value on actual test data i.e which indicates that most of the trends and patterns that could be captured by this model without overfitting was done and certainly, a good level of performance was achieved by the model.

### From Model Explainability(using LIME) :

The 5 most important features in predicting the risk of Coronary Heart Disease (CHD) are :

Diabetes_grade, Age, TotChol, Hypertension and Smoking Factor
