# Task
Using data from the Yandex.Realty service, determine the market value of real estate and typical parameters of apartments.

# Project description
Based on the Yandex.Realty service data, the market value of various types of real estate objects, typical parameters of apartments, depending on the distance from the center, were determined. 

- Data preprocessing has been carried out. 

- Added new data. 

- Histograms, boxplots, scatterplots are constructed.

# Tools
- Python
- Pandas
- Matplotlib

# Сonclusions
In the study, a dataframe was analyzed with information on sales of apartments in St. Petersburg and the Leningrad Region for the period 2014 - 2019. 

The sample size is 23,699 lines. During the study, data preprocessing was carried out: the formats of individual columns were changed, implicit duplicates were eliminated, gaps were filled in, where this did not affect the quality of data statistics, anomalous values ​​were examined for individual columns, and dataframe filtering was carried out to exclude rows with anomalous values.

**As a result of the analysis**:
- defined "normal" ad placement period = 102 days;
- a direct relationship has been established between the cost of the object and its area and the number of rooms;
- it was revealed that the most expensive objects are placed at the beginning of the week (Tuesday), and the cheapest - on the weekend;
- the presence of seasonality in the market has been established, in which the most expensive objects are placed in April, and the cheapest in June;
- found that since 2017, the market has moved to growth, after a three-year period of decline;
- a factor analysis of the market was carried out for the entire period, it was found that in 2014-2015 the market decline was associated both with a decrease in the total area of ​​apartments for sale and with a decrease in the average cost per square meter, then, from 2016, the cost per square meter begins to grow, and after it since 2018, the area of ​​objects for sale also begins to grow.
