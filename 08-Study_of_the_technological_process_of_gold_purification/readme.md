# Task
Development of a prototype machine learning model by predicting the recovery rate of gold from gold ore.

# Project description
The model must use **both data** with parameters for 
- the extraction and
- purification of raw materials.
The result of the model will be used to optimize production, making it possible not to launch an enterprise with unprofitable characteristics.

The model solves the **regression** problem, supervised learning.
Model predictions must be based independently on feedstock parameters and processing parameters.

The quality of the models will be compared using the **sMAPE metric**. 
The final model will be the one that shows the best metric value in comparison with others.

The project was completed in 3 steps:
- review and preprocessing of data;
- exploratory data analysis;
- building, training and testing the best model on a test set.

# Tools
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

# Сonclusions
To develop the model, 3 datasets with dimensions of 14,579 by 87, 4,860 by 53, and 19,439 rows by 87 columns were considered.

During preprocessing, it was determined that there were some rows containing gaps in the data, these rows were removed, which led to a reduction in data volumes from 7 to 16%, the data volume remained more than 10,000 rows.

**Research analysis** showed a close to normal distribution of gold (and other metals) concentrations at different stages of processing.

Two models were considered: **Decision Tree** and **Random Forest**.

According to the calculation results a prototype machine learning model (**Random Forest**) has been developed to predict the recovery rate of gold from gold ore, with a quality indicator on the test sample according to the metric **sMAPE = 7.1%**
