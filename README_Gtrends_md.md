# Gtrends_Oil

## Introduction
This project follows on from the Oil_Environment project and investigates some features of the Google Trends data further.

I will consider:
1. Is there a seasonal cycle in the Google Trends data?
2. Does combining the 'global warming' and 'climate change' values provide a more useful measure of environmental concern?
3. Is there evidence of a non-linear relationship between the Google Trends data and the oil company price data?

For this project I will concentrate on the 'global warming' and 'climate change' variables. We saw that the number of searches for 'oil spill' was generally very low so separating any trend from the noise would be difficult. 

 
## Conclusions
After applying decomposition models to the 'global warming' and 'climate change' search data it was apparent that they shared a similar seasonal pattern. With the aim of extracting a stronger signal from the data I chose to create a new variable defined as the sum of the trend components of the two search values.
I investigated a variety of polynomial regression models and determined that the best performing model was a linear model including orthogonal polynomials of the combined environmental trend data up to degree 5.
Comparing the preferred model to the simple model without any environmental search predictor I conclude that there is an association between RDSA share value and Google environmental searches. This project confirms that the Google environmental search data does partly 'explain' the RDSA data although greater contributions to the models performance come from the fuel price and FTSE index data.