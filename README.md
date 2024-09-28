# Term Deposit Subscription Prediction: Logistic vs. Ensemble Models

## Project Overview
This project is focused on solving a classification problem using machine learning techniques. The main objective is to predict whether a client will subscribe to a term deposit based on various features related to direct marketing campaigns of a Portuguese bank.

## Dataset
The dataset used in this project is related to direct marketing campaigns (phone calls) of a Portuguese banking institution. The classification goal is to predict if the client will subscribe to a term deposit (variable **y**). 

- **Source**: [Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)
- **File**: `bank-full.csv`

## Features:
The dataset contains the following features:
- **age**: Age of the client
- **job**: Job of the client
- **marital**: Marital status of the client
- **education**: Education level
- **default**: Whether the client has credit in default
- **balance**: Bank balance
- **housing**: Housing loan status
- **loan**: Personal loan status
- **contact**: Type of communication contact
- **day**: Last contact day of the month
- **month**: Last contact month of the year
- **duration**: Duration of the last contact
- **campaign**: Number of contacts performed during this campaign
- **pdays**: Number of days since the client was last contacted
- **previous**: Number of contacts before this campaign
- **poutcome**: Outcome of the previous marketing campaign
- **y**: The target variable (1 = client subscribed, 0 = client did not subscribe)


## Libraries Used
To run the code in this notebook, you will need the following Python libraries:
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`


## Model Overview
The notebook includes the following steps:

- Data loading and preprocessing.
- Feature encoding for categorical variables.
- Splitting the data into training and testing sets.
- Training a Logistic Regression model.
- Hyperparameter tuning using GridSearchCV.
- Building ensemble models using Random Forest and Gradient Boosting.
- Evaluating model performance using metrics such as accuracy, confusion matrix, and AUC.

## Results
-----------------------------------------------------
          Models         |   Accuracy    |    AUC   |
-----------------------------------------------------       
Logistic Regression      |    90.06%     |  0.6485  |      
Random Forest            |    90.22%     |  0.6663  |
Gradient Boosting        |    90.11%     |  0.6788  |
-----------------------------------------------------      

## Conclusion
This project demonstrates how to apply different machine learning models to a real-world classification problem. The performance of the models was compared using accuracy and AUC, and the most suitable model was identified.