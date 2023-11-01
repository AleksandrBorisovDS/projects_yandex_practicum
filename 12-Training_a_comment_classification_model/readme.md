# Task
Development of a machine learning model to determine the toxicity of comments for online store.

# Project description
Develop a tool - a machine learning model (**binary classification** task, supervised learning) that will identify toxic comments and send them for moderation.

The customer provided a set of data with markings about the toxicity of edits (the text column is the text of the comment, and toxic is the target attribute).

The customer's requirement for the quality of the model is that the value of the quality **metric F1** is not less than **0.75**.

The project was completed in 3 steps:
- loading, review and preprocessing of data;
- generating features for machine learning models;
- training various models and selecting the best hyperparameters.
  
# Tools
- Python
- Pandas
- nltk
- tf-idf

# Сonclusions
The customer provided initial data with comments marked on toxicity, data volume: 159,292 rows and 2 columns (comment text and toxicity markup).

As a result of the project:
- the data was preprocessed:
     -  comments were reduced to the original form of words,
     -  stop words were removed;
- an analysis of class balance was carried out, the results of which were taken into account in the parameters of the models;
- three machine learning models were trained:
     -  logistic regression,
     -  decision tree 
     -  random forest.
- the best hyperparameters were selected for each model.
- 
As a result, the best value of the **F1** metric was shown by the **Logistic Regression** model, for which on the test sample (with parameter C=16) the value of the F1 metric = **0.7888**.
The task was successfully completed.
