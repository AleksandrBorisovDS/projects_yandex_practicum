# Task
Based on historical data on customer behavior and termination of contracts with Beta-Bank, it is necessary to predict whether the client will leave the bank in the near future or not.

# Project description
It is necessary to solve the **classification task** and build a supervised learning model.
The criterion for the success of the model, defined by the customer, is the high value of the **F1-measure** on the test sample, no less than **0.59**.

The project was completed in 4 steps:
- preparing data from an existing dataset;
- research of model options;
- eliminating class imbalance;
- testing the best model.

# Tools
- Python
- Pandas
- Matplotlib
- Scikit-learn

# Сonclusions
As a result of the project, a dataset with historical data on the behavior of Beta-Bank clients and the termination of contracts with them was studied.
The dataset size is 10,000 rows and 13 columns.

Three models were analyzed:
- Decision tree
- Random forest
- Logical regression.

The best model turned out to be **Random Forest**, which showed an **F1-measure** value of **0.613** on the test sample. 
This indicator is higher than the minimum value required by the customer of 0.59, which means that the selected model is successful and can be used by the customer to predict the possible termination of the contract by existing customers.

Additionally, the **AUC-ROC** indicator was calculated for all models, which was equal to **0.85** on the test sample.
