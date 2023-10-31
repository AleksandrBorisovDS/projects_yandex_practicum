# Task
Build a machine learning model - a regression task, supervised learning - that will help determine the region where mining will bring the greatest profit.

# Project description
The customer, the oil producing company GlavRosGosNeft, due to the need to expand oil production in one of the three existing fields, is interested in an objective justification for the choice of the region in which new wells will be installed.

Data on the characteristics of existing fields is available - oil samples in three regions: in each 10,000 fields, where the quality of oil and the volume of its reserves were measured.

The project was completed in 4 steps:
- loading, review and preparation of source data;
- preparation of samples for the model, formation of the model and evaluation of modeling results;
- assessment of the minimum effective production value at which production makes a profit;
- calculation of profits and risks, conclusion for a promising region.

# Tools
- Python
- Pandas
- Matplotlib
- Scikit-learn

# Сonclusions
As a result of the development of the project, data for 3 oil production regions was analyzed; for each region, data in the amount of 100,000 rows and 5 columns were analyzed.

Based on these data, **linear regression** models (supervised learning) were generated, according to which, using the **bootstrap** procedure, the values ​​of possible profit from mining in each region were predicted.

According to the calculation results, **Region 2** was recognized as the best region.

However, despite the good indicators of Region 2, it is necessary to further check the source data for this region, since the indicators of the source data of Region 2 differ significantly from the source data of Regions 1 and 3.
