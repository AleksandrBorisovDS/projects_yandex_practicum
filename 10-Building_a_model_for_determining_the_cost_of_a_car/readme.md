# Task
Based on historical data (technical characteristics, configurations and prices of cars), to build a machine learning model (solve a **regression problem**, supervised learning) to predict the market value of cars.

# Project description
The customer, a service for selling used cars "Not a Bit, Not a Paint", is developing an application that provides the ability **to quickly** determine the cost of a car based on its technical parameters, and is interested in developing a machine learning model that would predict this price.

Model characteristics required by the customer: 
- high speed of operation,
- quality metric **RMSE** no more than **2,500**.

To develop the project, a dataset was provided with historical data on sales prices of used cars, including the technical characteristics of these cars.

# Tools
- Python
- Pandas
- LightGBM

# Сonclusions
To develop the project, a dataset with historical data was provided, which contained 354,369 rows and 16 columns. The data contained gaps.
As a result of the data preprocessing, a dataset of 277,080 rows and 10 columns was prepared, containing no gaps, full of explicit and implicit duplicate rows, which was used for training and testing machine learning models.

3 machine learning models were studied:
- LightBRM,
- CatBoost
- Linear regression.

Linear regression showed the best results in terms of training and prediction time, but did not provide the required quality.

The LightBRM and CatBoost models have been extensively analyzed and both training and prediction times have been significantly reduced.

The **CatBoost** model was chosen as the best model, showing the following results:
- the training time was: 12.9 s.
- the prediction time on the test sample was: 0.049 s.
- **RMSE: 1,626**.

The resulting RMSE value is significantly lower than the threshold specified by the customer (2,500).
Thus, the task was completely completed.
