# supervised learning project
## Introduction
I have been hired by Beta Bank to predict whether a customer will leave the bank soon. They have been dealing with customers leaving the bank and have determined that it is cheaper to save existing customers rather than attract new ones. 

Goals:
- Build a model with the maximum possible F1 score (higher than 0.59).
- Calculate the AUC-ROC score and compare it with the F1 score.

Data description:
- Features
    - `RowNumber` — data string index
    - `CustomerId` — unique customer identifier
    - `Surname` — surname
    - `CreditScore` — credit score
    - `Geography` — country of residence
    - `Gender` — gender
    - `Age` — age
    - `Tenure` — period of maturation for a customer’s fixed deposit (years)
    - `Balance` — account balance
    - `NumOfProducts` — number of banking products used by the customer
    - `HasCrCard` — customer has a credit card
    - `IsActiveMember` — customer’s activeness
    - `EstimatedSalary` — estimated salary
- Target
    - `Exited` — сustomer has left

Plan:
- Pre-process the data (feature preparation, training/validation/test splitting, feature scaling, investigate class balance).
- Train decision tree, random forest and logistic regression models without taking into account class imbalance.
- Account for class imbalance.
- Compare decision tree, random forest and logistic regression models with different hyperparameters, optimizing using the F1 score.
- Train the best model and calculate performance metrics.
