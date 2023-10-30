# Task
Based on the data, offer the client a tariff.

# Project description
Based on data on the behavior of customers of the mobile operator "Megaline", build a model to recommend a suitable current tariff plan ("Smart" or "Ultra").
The model will be formed based on data on the behavior of users who have already switched to these tariffs.

# Tools
- Pyton
- Pandas
- Matplotlib
- Scikit-learn

# Сonclusions
Using a data set of behavior of users who selected current tariffs of the Megaline company in the amount of **3,214 rows**, a tariff recommendation model was created, which is based on the **Random Forest model**. 
This model showed high **accuracy** on both the validation (80.9%) and test (**78.4%**) samples, and also passed the adequacy test. 
Due to the fact that the minimum accuracy of the model was determined by the customer to be 75%, this model can be used by Megaline to recommend current tariffs for users.
