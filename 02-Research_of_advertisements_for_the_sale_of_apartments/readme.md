# Task
Using data from the Yandex.Realty service, determine the market value of real estate and typical parameters of apartments.

# Project description
Based on the Yandex.Realty service data, the market value of various types of real estate objects, typical parameters of apartments, depending on the distance from the center, were determined. 

- Data preprocessing has been carried out. 

- Added new data. 

- Histograms, boxplots, scatterplots are constructed.

# Tools
- Pyton
- Pandas
- Matplotlib

# Сonclusions
In the study, a dataframe was analyzed with information on sales of apartments in St. Petersburg and the Leningrad Region for the period 2014 - 2019. 

The sample size is 23,699 lines. During the study, data preprocessing was carried out: the formats of individual columns were changed, implicit duplicates were eliminated, gaps were filled in, where this did not affect the quality of data statistics, anomalous values ​​were examined for individual columns, and dataframe filtering was carried out to exclude rows with anomalous values.

**As a result of the analysis**:
- defined "normal" ad placement period = 102 days;
- a direct relationship has been established between the cost of the object and its area and the number of rooms;
- 
