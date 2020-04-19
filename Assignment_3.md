### Assignment 3 - Methodological Review
#### Logistic Regression vs. BFAST


### Introduction:
One of the important elements to effective development is understanding the environmental factors that are most directly correlated with the quality of life for citizens. Urbanization and progressive growth is an inherently complex process which if it is to be modeled and predicted, requires the quantitative analysis of a variety of perspectives. One of the ways that shows great promise and efficacy is the use of geospatial data to illustrate physical expansion and growth of urban areas. Models that use Logistic Regression as well as Breaks For Additive Seasonal and Trends (BFAST) models have shown promise in regard to this pursuit. 

### Inquiry Type:
This research question is equal part explanatory, and equally exploratory. My research question revolves around understanding the variables that correlate with urban expansion and development and how much of a causal factor they are. Similar to Geoff West’s book on Scale, there is a certain amount of urban growth that is a product of our structure of the human mind. We live in a time with an unprecedented amount of geospatial data, and being able to utilize this data will allow us to not only understand the practical implications of development, but the existential complexities and limitations of the human condition. To model and predict these geographical behaviors and changes is to ascertain a perspective on humanity that has never been witnessed before. 
The main questions that this research seeks to address are:
- How can geospatial data be effectively used to project and estimate the future urban growth. 
  - What factors and covariates are most correlated with this growth?
  - What steps can be taken to ensure the most efficient amount of development?
- What methods of geospatial analysis are most effective at predicting change?
  - How can this data be harnessed to improve life for residents?
  - What patterns can be extrapolated and applied to all developing areas? How does this compare to the patterns that are only locally significant?

### Method 1: Logistic Regression Model [1]

### Model: Logistic Regression Model
As a brief introduction, logistic regression functions look like an ‘S’ shaped logistic function. The curve goes from 0 to 1 and the number signifies probability. In logistic regression, predictions can be made using discrete or continuous data, and each variable can be tested to see if it is helpful in the prediction by testing to see if the effect on the prediction is significantly different from zero, this can be done using Wald’s test (chi-squared test) to see if data is relevant to the prediction. Logistic regression is a popular machine learning method because of its classification uses. In our specific case, this is the formula:
<image>
![Example Image](/Images/LogReg.png){
  width: 70%;
  border: none;
  background: none;
}
</image>
