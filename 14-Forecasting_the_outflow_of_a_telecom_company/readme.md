# Task
Develop a machine learning model to predict customer churn for a telecommunications company.

# Project description
Based on historical data, create a machine learning model that would predict whether a customer plans to leave or not. 
Solve the **classification** problem, supervised learning. 
Train a model, that determines the client’s desire to refuse the company’s services in order not to lose him and promptly offer promotional codes and special conditions.

Quality metric of the resulting model: **AUC-ROC**
Required metric value: more than **0.85**.

# Tools
- Python
- Pandas
- Matplotlib
- Scikit-learn

# Сonclusions
**Description of the main steps performed when working on the project:**
- Loading data from 4 different files into 4 variables. The load process attempted to load date data into datetime format.
- The data was merged into 1 file (merge(left, right, on=['customerID'], how='outer')).
- Obvious complete duplicate lines were removed, gaps were filled (with the value "No").
- Based on data about the beginning (BeginDate) and end (EndDate) of the contractual relationship with the client, two additional characteristics were created:
    - the period ("client_period") during which the client is (was) a client 
    - the target characteristic ("target") whether he is a client (1) or no longer (0).
- The data is reduced to the required formats:
    - numeric attributes to the float and int formats
    - categorical attributes to the object format;
- The correlation between signs has been studied. It was found that the characteristics InternetService and MonthlyCharges have the highest correlation, the correlation coefficient between them is 0.92;
- Column names are set to "snake_style".

To train the models, a sample size of 7,039 rows by 18 columns was generated, of which 1 - int, 2 - float and 15 - object.

To solve the problem, 3 machine learning models were generated and trained:
- LogisticRegression;
- RandomForestClassifier;
- CatBoostClassifier.

The selection of the best hyperparameters of the models was carried out using GridSearchCV.

The results of training models with the best hyperparameters according to the **roc-auc** quality metric are as follows:
- LogisticRegression - 76.9%;
- RandomForestClassifier - 80.8%;
- CatBoostClassifier - 92.5%.

Thus, the best indicator in terms of quality metrics was the **CatBoostClassifier** model with the following hyperparameters:
- 'classifier__depth': 4,
- 'classifier__iterations': 1000,
- 'classifier__l2_leaf_reg': 1,
- 'classifier__learning_rate': 0.1

The best model was tested on a **test sample**, where it showed a **quality metric value of 91.7%**,
the project objectives have been fully completed.
