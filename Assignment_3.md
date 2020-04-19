#### Assignment 3 - Methodological Review
#### Logistic Regression vs. BFAST


#### Introduction:
One of the important elements to effective development is understanding the environmental factors that are most directly correlated with the quality of life for citizens. Urbanization and progressive growth is an inherently complex process which if it is to be modeled and predicted, requires the quantitative analysis of a variety of perspectives. One of the ways that shows great promise and efficacy is the use of geospatial data to illustrate physical expansion and growth of urban areas. Models that use Logistic Regression as well as Breaks For Additive Seasonal and Trends (BFAST) models have shown promise in regard to this pursuit. 

#### Inquiry Type:
This research question is equal part explanatory, and equally exploratory. My research question revolves around understanding the variables that correlate with urban expansion and development and how much of a causal factor they are. Similar to Geoff West’s book on Scale, there is a certain amount of urban growth that is a product of our structure of the human mind. We live in a time with an unprecedented amount of geospatial data, and being able to utilize this data will allow us to not only understand the practical implications of development, but the existential complexities and limitations of the human condition. To model and predict these geographical behaviors and changes is to ascertain a perspective on humanity that has never been witnessed before. 
The main questions that this research seeks to address are:
- How can geospatial data be effectively used to project and estimate the future urban growth. 
  - What factors and covariates are most correlated with this growth?
  - What steps can be taken to ensure the most efficient amount of development?
- What methods of geospatial analysis are most effective at predicting change?
  - How can this data be harnessed to improve life for residents?
  - What patterns can be extrapolated and applied to all developing areas? How does this compare to the patterns that are only locally significant?

### Method 1: Logistic Regression Model [1]
As a brief introduction, logistic regression functions look like an ‘S’ shaped logistic function. The curve goes from 0 to 1 and the number signifies probability. In logistic regression, predictions can be made using discrete or continuous data, and each variable can be tested to see if it is helpful in the prediction by testing to see if the effect on the prediction is significantly different from zero, this can be done using Wald’s test (chi-squared test) to see if data is relevant to the prediction. Logistic regression is a popular machine learning method because of its classification uses. In our specific case, this is the formula:
<img src="https://github.com/RonanChance/Evolving-Solutions/blob/master/Images/LogReg.png">

In this formula, 
- P(z) is the probability of the dependent variable.
- Z; x1, x2, ⋯ xm are the independent variables.
- A is the interception. 
- B1, b2, … , bm are the regression coefficients. 
- Epsilon is the binomially distributed error.  
- Z is the probability of occurrence of privatized land (value between 1 and 0).

Regression coefficients represent the contribution of each independent variable on P(z). 
If the regression coefficient is positive, this is an increased probability of growth. Conversely, a negative coefficient means no growth. 

The way this study was conducted, they rasterized (which means to take a photo and break it down into its binary data) the geospatially collected photographs. With this, the distance to roads and water kiosks can be calculated, as well as classifying areas into their respective subcategories. 

<img src="https://github.com/RonanChance/Evolving-Solutions/blob/master/Images/TimeChange.png" width="175" height="350">

Using a logistic regression model, this specific study found that such expansion is related to social infrastructure rather than to natural landforms. The most significant increase over the years was in private land ownership in Ulaanbaatar (as seen in the illustrations above). The study also found that they could determine potential ‘hot spots’ by estimating spatially and comparing the regression coefficients. The places near water kiosks and near roads showed a much greater likelihood of being developed. Surprisingly, natural environmental factors were much less important compared to the social infrastructure influences. 

Unfortunately, the expansion that was seen in the years depicted resulted in a deterioration of living standards and actually caused an increasingly disordered pattern amongst the fringes of the city. I feel as though this finding has serious merit in further studies regarding prediction, and wonder if these ‘disordered’ patterns resemble anything like that of a fractal. 

#### Method 2: Breaks for Additive Seasonal and Trend Model [2]
The BFAST model is used for change detection of land cover, and it estimates the both the time and number of changes which are characterized by their magnitudes and directions. 

<img src="https://github.com/RonanChance/Evolving-Solutions/blob/master/Images/BFAST1.png" width="375" height="70">
<img src="https://github.com/RonanChance/Evolving-Solutions/blob/master/Images/BFAST2.png" width="375" height="70">
<img src="https://github.com/RonanChance/Evolving-Solutions/blob/master/Images/BFAST3.png" width="500" height="70">

As can be seen, this modeling process does require a significant amount of math and is relatively complex. The model combines an iterative decomposition of seasonal, trend, remainder components to detect change. Then, a piecewise linear trend and seasonal model can be created with the above equations.

<img src="https://github.com/RonanChance/Evolving-Solutions/blob/master/Images/BFAST4.png" width="400" height="400">

The above equations are incorporated into this diagram which show Yt (the observed data at the current time), Tt (the trend component), St (the seasonal component), and et (the remainder component). Essentially, this shows us when ‘breaks’ occur, which is when structural changes happen. 

In past use cases, the BFAST methodology has only been used to monitor vegetation to distinguish grassland and detect forest fires. This study realizes the potential for BFAST to monitor the land changes that result from urban growth. There have been a multitude of negative results because of the unplanned growth of the privately held ger-areas. It has caused pollution, traffic congestion and even unemployment. The BFAST method has potential to greatly benefit policymakers and governments in furthering and shaping the best possible outcomes of development.

#### Further Study & Conclusion

The Linear Regression and Breaks For Additive Seasonal and Trends models have both yielded useful data, and for this reason, both warrant continued usage and application in continuing studies regarding urban development. In fact, these methods are not mutually exclusive, and finding ways to use them in unison could be a continued line of research. I would also like to see a connection to Geoff West’s scaling laws and fractal-like nature of growth. 

#### Sources

[1] Tsutsumida, N., Saizen, I., Matsuoka, M., & Ishii, R. (2015). Addressing urban expansion using feature-oriented spatial data in a peripheral area of Ulaanbaatar, Mongolia. 
doi: https://doi.org/10.1016/j.habitatint.2015.01.024

[2] Tsutsumida, N., Saizen, I., Matsuoka, M., & Ishii, R. (2013). Land Cover Change Detection in Ulaanbaatar Using the Breaks for Additive Seasonal and Trend Method. Land, 2(4), 534–549. doi: https://doi.org/10.3390/land2040534
