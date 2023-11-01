# Task
Development of a machine learning model to predict taxi orders for the next hour.

# Project description
In order to attract more drivers during **peak hours*, it is necessary to develop a machine learning model (**regression task**, supervised learning) to predict the number of orders in the next hour.

To train the model, historical data on the number of taxi orders is available.

Model quality requirements:
- assessment based on the **RMSE** metric;
- the metric value should not be more than **48** on the test sample.

The project was completed in 4 steps:
- loading, reviewing and resampling data in one hour;
- data analysis, preprocessing;
- training several different models, selecting the best hyperparameters on the training set. (test sample - 10% of the original data);
- checking the best model on a test sample.

# Tools
- Python
- Pandas
- Scikit-learn
- Statsmodels

# Сonclusions
Historical data contained information on the number of orders in the period from March 1 to August 31, 2018.
The total data volume was 26,496 rows.

As a result of work on the project, it was determined that the data does not require additional preprocessing.

The data was **resampled at 1 hour**, because the customer needs a forecast of the number of orders for the next hour.

Additional features and samples were generated for training machine learning models.

4 models were trained:
- Linear Regression,
- Random Forest,
- CatBoost
- LightGBM.

The best value of the **RMSE metric** on the training set was shown by the **Random Forest** model. RMSE = **8.269**.
The Random Forest model, with the best hyperparameters (number of trees 500, maximum tree depth 20) was tested on a test sample.
The **RMSE** metric value was **47.71**, which meets the customer’s requirement - no more than 48.

The task was completed completely.
