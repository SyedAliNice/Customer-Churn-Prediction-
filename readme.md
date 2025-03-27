# Customer Churn Prediction

## Introduction

This project leverages Logistic Regression, Decision Tree, Random Forest, and Naive Bayes algorithms to predict customer churn, helping businesses proactively retain their customers.


## Dataset

The dataset consists of bank customer data with 14 features, such as age, bank balance, tenure, geography, and credit score. These features are used to predict whether a customer will exit the bank (churn). The target column indicates if the customer exited or not.
### Dataset Statistics:

Here is sample statistics of the data.

- **Name:** Churn_Modelling
- **Mode:** Tabular Data
- **Number of Samples:** 
  - Train: 12,723 
  - Test: 3,181
- **Type:** Binary Classification
- **Number of Classes:** 2
- **Classes Name:** 
  - Not Exited: 0
  - Exited: 1

## Pre-processing

The preprocessing steps of the proposed project are the following:
<list of preprocessing steps>

1. Removed unnecessary columns: Row Number, Customer ID, and Surname
2. Detected and removed outliers
3. Applied label encoding on the Age column
4. Used one-hot encoding for the Geography column
5. Balanced the target class using SMOTE to address class imbalance
6. Scaled the data using StandardScaler

## Models

For the Customer Churn Prediction following models are trained with the tuned hyperparameters:


- **Logistic Regression**
  - The Logistic Regression model was trained using default hyperparameters, with no additional tuning.

- **Decision Tree**
  - The Decision Tree model was trained using default hyperparameters, with no additional tuning.

  **Random Forest**
  - The Random Forest model was trained using default hyperparameters, with no additional tuning.

- **Naive Bayes**
  - The Naive Bayes model was trained using default hyperparameters, with no additional tuning.

## Results


| Metrics    | Logistic Regression | Decision Tree | Random Forest | Naive Bayes |
|------------|---------------------|---------------|---------------|-------------|
| Accuracy   |        0.8233       |     0.8240    |    0.8862     |   0.8004    | 
| Precision  |        0.825        |     0.820     |    0.885      |   0.803     |
| Recall     |        0.825        |     0.825     |    0.890      |   0.800     |
| F1-Score   |        0.825        |     0.825     |    0.885      |   0.800     |


## Dependencies

- **NumPy version: 1.26.4**: For numerical operations.
- **Pandas version: 2.2.2**: For data manipulation and analysis.
- **Scikit-learn version: 1.4.2**: For machine learning tools.
- **Matplotlib version: 3.8.4**: For data visualization.
- **Seaborn version: 0.13.2**: For data visualization.
- **ImbLearn version: 0.12.3**: For SMOTE method for class imbalancing.



