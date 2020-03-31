### Nieves et a. use the random forest machine learning method to predict what value globally? Describe in detail how the random forest works. What is a dasymmetric population allocation? Which geospatial covariates proved to be the most important when predicting global values of where humans reside?

The goal is to find the best predictive correlates for population and population density. They looked at:
- Nighttime lights
- Energy productivity of plants
- Topographic elevation
- Climatic factors
- Type of land cover
- Roads
- Water features
- Human settlements and urban areas

Then they came up with a WIR for each category (Weighted Importance Rank). This is calculated by taking the within-country ranked importance and dividing it by the total number of covariates in the model. Ultimately topographical features were very important predictors. Also "urban/suburban extents, built environment and urban/suburban proxies, climatic/environmental variables, populated place covariates, and transportation networks. The article also says that the importance of climatic factors was unexpected. One of the challenges that was experienced was the recency and date of data. Often the census data did not align perfectly with the geospatial data, which is problematic for finding correlations. 

The Random Forest algorithm is a non-linear statistical method that includes machine-learning. It's an ensemble method because it combines individually weak predictive trees into one that is more predictive than the others alone. The Dasmetric population allocation is a process where (in this case) where we draw more accurate data by creating new boundaries by distributing the data. In this case, census data was used to understand how population was distributed and then using this comparitively to the other varibles to find relationships in the data.
