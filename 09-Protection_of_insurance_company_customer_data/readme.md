# Task
Develop a method for converting personal data of clients of the insurance company "Though the Flood" in such a way that:
- on the one hand, the data was difficult to recover;
- on the other hand, data transformation did not degrade the quality of the machine learning model (linear regression).

# Project execution order.

The project was completed in 4 steps:
- loading, viewing and preprocessing of data;
- matrix multiplication method processing;
- selection and justification of the data conversion algorithm;
- testing the algorithm using performance metrics of machine model learning.

# Tools
- Python
- NumPy
- Scikit-learn

# Сonclusions
During the work on the project, a dataset of 5,000 rows and 5 columns was examined.

Based on the results of preprocessing, 153 lines of complete duplicates were found and excluded; otherwise, the data was ready for processing.

The method of **multiplying the feature matrix by an invertible matrix** was chosen as a method that meets the requirements of the problem. The possibility of using this method was confirmed both 
- theoretically - through formulas for calculating weights and prediction vectors.
- practically - through calculating the quality metric of a **linear regression model** based on the initial characteristics and on the characteristics after appropriate multiplication by an invertible matrix.

**CONCLUSION**: the method of multiplying a feature matrix by an invertible matrix can be used to protect personal data, without affecting the quality of the linear regression model.
