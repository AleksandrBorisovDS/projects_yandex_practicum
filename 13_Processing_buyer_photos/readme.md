# Task
Development of a machine learning model to determine the age of buyers from photographs.

# Project description
In connection with the introduction of a **computer vision system** for processing photographs of customers, it is necessary to develop a model that would determine the **approximate age** of the buyer from a photograph taken in the checkout area at the time of purchase.

Necessary develop a machine learning model (**regression problem**, supervised learning) based on an existing dataset with photographs of people and an indication of age.

Model requirements:
- quality assessment metric - **MAE**
- quality metric value is **less than 8**.

The project was completed in 2 stages:
- exploratory analysis of data from the existing dataset;
- formation and training of a machine learning model on a GPU simulator.

# Tools
- Python
- Keras

# Сonclusions
To train the model, a labeled dataset of **7,591 photographs** of people with the specified age was used.

As a result of the project, a model was developed based on a **convolutional neural network on the ResNet50** architecture with the **Adam** optimizer.

To reduce the model training time, the following was used:
- use of the reduced ResNet50 architecture (parameter include_top=False);
- using weights calculated on a pre-trained **imagenet** neural network;
- application of the **loss function mean squared error**.

As a result, model showed a **MAE** metric value on the test sample = **6.47**, which is significantly lower than the minimum required threshold for model quality.
