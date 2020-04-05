### Dasymetric mapping and Bayesian modeling for improved prediction of effective urbanization throughout Mongolia
#### by Ronan Donovan 
#### March 31, 2020

### Introduction
The purpose of this research is to improve upon the use of high resolution geospatial data to generate a multi-layered dasymetric map of Mongolia by specifying, estimating and validating a bayesian model of sentiment analysis. Achieving this result will require meeting the following objectives:

Collection of geospatial data regarding air pollution, water quality, and topography. 
Using collected data to estimate a bayesian model for predicting hot spots of poor environmental quality across Mongolia. 
Combining data with a dasymetric analysis map of sentiment surveys.
Analysis of correlation between covariates and social well-being.

This work will build on previous research by Byambakhuu Gantumur et. al and Gankhuyag and will incorporate new methods to implement both a dasymetric map and a bayesian model towards inferring the most impactful covariates to social satisfaction. 

### Human Development Topic
Rapid urbanization has profound impacts on both the socio-economics of a country as well as the environment. Both of these areas have been investigated in a number of countries, and in Mongolia. The inherent issue lies in the unsustainable manner in which development often occurs, and Ulaanbaatar is an example of this kind of growth. 

In 2015 the United Nations proposed 17 Sustainable Development Goals (SDG). The issue of sustainable cities and communities (goal 11), good health and well-being (goal 3), and responsible consumption and production (goal 12) are only a few of the problems with which an understanding and utilization of geospatial data and analysis could vastly improve the future. 

### Human Development Process
Mongolia is a landlocked country that lies between Russia and China. Despite the significant land mass of the country, the vast majority of all development is centralized in the capital city, Ulaanbaatar, which is home to ~45% of the country’s population. The cities of Mongolia are mostly populated by ger settlements with little access to proper sanitation, waste disposal, or safe drinking water (Ts. Gantsog). The economy has historically been heavily dependent on the mining sector, with approximately 90% of trade being with the Soviet Union during 1960 to 1990. In 1990, Mongolia had its first parliamentary election and began to build a market economy. Since then, the economy has been heavily dominated by private entities with an emphasis on mining coal (Ts. Gantsog). Despite these economical steps forward and significant urbanization and development, the country faces a number of issues in regard to sustainable development. 


### Geospatial and Data Science methods
The paper by Tsutsumida focused on monitoring urban expansion in Ulaanbaatar by using spatial data to calculate and use a Logistic Regression Model to better understand the factors that contribute to further development. A logistic regression model is based on statistics with a dependent binary result, which in this case, is whether future development is predicted in a location. They study GIS data and ASTER imagery. The resolution of early data was 1-4m2 but improved to 0.6-2.8m2. The research found a very significant increase in urbanization, and the proportion of private land in the study increased by 12.9% in six years. They also found that the increase in private land did correlate with the proximity of water kiosks and roads. Essentially, private land tended to be built by other private land. The researchers did explain that it was difficult to ‘incorporate the effects of disaggregated human behaviors on urban surfaces’ (Tsutsumida). In addition to this, topographical indicators did not have nearly as much of an effect as was expected. 

The assessment written by Kelderman and Batima did an in depth analysis of water pollution in Mongolia. The data examined was quite aged as it was taken between 1949 and 1990. Despite this, the study found some interesting geographical and geological trends. Their data science method included the use of 72 monitoring stations on the 35 rivers of Mongolia. These stations monitored a number of variables including the Total Suspended Solids, along with all the major ions, oxygen, and nutrients. Much of the negative impact on water pollution was a result of Ulaanbaatar's increasing urbanization with increased levels of Ammonia in the Tuul river. 

Gankhuyag’s paper on monitoring the development of informal settlements in Ulaanbaatar takes a different approach than Tutsumida’s paper. This paper is designed to be used to plan future development and infrastructure in Mongolia. Similar to Ttusumida, the study utilized geospatial data (landsat images, aerial photography, ASTER data) and topographical mapping. However, they grouped the data more specifically into classes. Eight different classification types of development gave a much more in depth analysis of the kind of urban growth happening. The study also gained insightful knowledge on the different benefits and drawbacks to Aerial photography vs. SPOT pan vs. ASTER vs. SPOT XS vs. Landsat. 

Jean Caldieron from Florida Atlantic University studied the residential satisfaction of neighborhoods in Ulaanbaatar. This study consisted of a 33 questionnaire survey data, and the data collected was quite fascinating. About half of surveyed individuals were previously nomadic (48%), 57% had been living in their current place for less than 5 years, 79% own the land they are on. The majority (69%) also are happy with the neighborhood they reside. The data collected showed a higher satisfaction than expected. 

The paper by Allen explores how air pollution is correlated to mortality rates in Mongolia. The process relied heavily on Land Use Regression (LUR) modeling and Mobile monitoring to estimate mortality attributable to pollution. The study concluded that “29% of cardiopulmonary deaths and 40% of lung cancer was attributable to outdoor air pollution” (Allen). The LUR modeling was possible through monitoring population density, land use, elevation, and other geographical characteristics. A Digital Elevation Model was produced using GIS to calculate the elevation distribution of the country. The road data was obtained from OpenStreetMap (with some minor changes made using ETM images). Mobile and stationary monitoring sites monitored the concentration of NO2and SO2. The study concluded that there were around 7-8 times the World Health Organization’s air quality guidelines depending on the month (winter months were much worse).

The study by Nyamtseren focused on the precipitation trends in Mongolia. Climatic aridity (droughts) are very significant environmental problems that affect quite a number of people and can be very detrimental to a landlocked country like Mongolia. The data was collected from the National Agency for Meteorology and Environmental Monitoring by 70 weather stations over 40 years. The Mann-Kendall process (statistical test for analysis of climate trends). It is non-parametric (so data does not have to be normally distributed), and was used to detect trends in time series. Future aridity predictions were made with ECHAM5 models with 30km resolution. Due to urbanization, the Mann-Kendall predictions estimates that aridity will likely impact livestock and agriculture, which are very essential to Mongolia. This information could be valuable for planning water distribution and resources to most at-risk areas. 

Net Primary Production (NPP) is the measurement of new carbon stored as biomass in vegetation. To better understand the process of global warming, this can be measured and monitored using multi-spectral satellite sensor data (Xiong Yan). The chosen site that was studied is southwest of Ulaanbaater and is 60km2. The team took measurements over 5 months and developed a new ‘vegetation index’ referred to as VIPD. Using this formula, they continued to input their measurements into it (Generally - when vegetation is doing well, VIPD goes towards 1, when it is dying, it goes towards 0). Using the Landsat ETM+ data, the estimated NPP was ~0.056kgCO2in June of 2001. Geospatial data such as this could be extremely beneficial to understanding the effects of the increased carbon in the environment resulting is coal usage.

The impact of the environment on health in Mongolia is a pressing issue that was explored in depth by Jadambaa et al. in their systematic review using electronic databases and studies. Results showed that the population had significant exposure to “pollution, metals, tobacco, and chemical toxins” (Jadambaa et al.). This kind of data is essential to the understanding of the country because 27.6% of the population was below the age of 15 in 2009, and around 40% of the population under 19 and are at risk of health degradation (as children are particularly vulnerable). Significant issue exists, like 45.4% of all springs in rural areas containing E. Coli in 2008. Rapid industrialization has caused increasing work-related illnesses, and problems with child labor. Blood levels of lead, mercury, arsenic, zinc, etc. in Mongolian children is also significantly higher than children in both Russia and China (Jadambaa et al.). This review did not use geospatial data, however it was an aggregation of other studies that utilized various means of data collection. 
	
The relationship between the rapid urbanization process of Mongolia and the effect it has on the environment was studied closely by Byambakhuu Gantumur et. al. and their method included a number of remote sensing methods to conduct their study. Land Use and Land Cover (LULC) are important in understanding the impact of development. Because urbanization often occurs in an unplanned process, understanding the impacts can help prepare for how to better develop in the future. The study relied on landsat images collected by the USGS EDC between 1990 and 2015. The team used a change detection process to analyze the remotely sensed data. The raster maps were converted to boxplots with R. The graphs are able to show the increase of agricultural fields, water reflux of the Tuul river, and built up areas. 


### Discussion
The aggregation of these articles and datasets gives a much more contextual understanding of the processes that are being used to understand the development of Mongolia and the city of Ulaanbaatar. One of the important elements to effective development is understanding the environmental factors that are most correlated with quality of life. This study seeks to find ways of giving numerical answers to complex practical issues. There has yet to be a consolidation of the geospatially and survey collected data for aggregated mapping applications, and doing so would provide unparalleled understanding for future growth. The connection between health and satisfaction with air pollution, water quality, and urban development, is essential to the future of the country. 

## References

#### New Sources
Byambakhuu Gantumur, Falin Wu, Yan Zhao, Battsengel Vandansambuu, Enkhjargal Dalaibaatar, Fareda Itiritiphan, and Dauryenbyek Shaimurat "Implication of relationship between natural impacts and land use/land cover (LULC) changes of urban area in Mongolia", Proc. SPIE 10431, Remote Sensing Technologies and Applications in Urban Environments II, 104310M (4 October 2017); https://doi-org.proxy.wm.edu/10.1117/12.2278360

Jadambaa, A., Spickett, J., Badrakh, B., & Norman, R. E. (2015). The Impact of the Environment on Health in Mongolia: A Systematic Review. Asia Pacific Journal of Public Health, 27(1), 45–75. https://doi.org/10.1177/1010539514545648

Nyamtseren, M., Feng, Q., & Deo, R. (2018). A Comparative Study of Temperature and Precipitation-Based Aridity Indices and Their Trends in Mongolia. International Journal of Environmental Research, 12(6), 887–899. https://doi.org/10.1007/s41742-018-0143-6

TS. Gantsog, S. Altantsetseg (n.d). Cost of Socio-Economic Reform: Problems to Ensure Human Development in Mongolia. National University of Mongolia, http://www.policy.hu/sodnomtseren/Humandevelopment.PDF

Xiong Yan, Kanako Muramatsu, Masahiro Hirata, Kazato Oishi, Ichirow Kaihotsu, Tamio Takamura, Shinobu Furumi & Noboru Fujiwara (2004) Verification of net primary production estimation method in the Mongolian Plateau using landsat ETM+data. https://doi.org/10.1007/BF02826648

#### Old Sources

Allen, R.W., Gombojav, E., Barkhasragchaa, B. et al. An assessment of air pollution and its attributable mortality in Ulaanbaatar, Mongolia. Air Qual Atmos Health 6, 137–150 (2013). https://doi.org/10.1007/s11869-011-0154-3

Caldieron, J., & Miller, R. (2013). Residential Satisfaction in the Informal Neighborhoods of Ulaanbaatar, Mongolia. Enquiry The ARCC Journal for Architectural Research, 7(1), 12-18. https://doi.org/10.17831/enq:arcc.v7i1.73

P. Kelderman, P. Batima; Water quality assessment of rivers in Mongolia. Water Sci Technol 1 3May 2006; 53 (10): 111–119. doi: https://doi.org/10.2166/wst.2006.304

Radnaabazar, G., Kuffer, M., & Hofstee, P. (2004). Monitoring the development of informal settlements in Ulaanbaatar, Mongolia. 333-339. Vienna, Austria: Vienna University of Technology. https://research.utwente.nl/en/publications/monitoring-the-development-of-informal-settlements-in-ulaanbaatar

Tsutsumida, N., Saizen, I., Matsuoka, M., & Ishii, R. (2015). Addressing urban expansion using feature-oriented spatial data in a peripheral area of Ulaanbaatar, Mongolia. https://doi.org/10.1016/j.habitatint.2015.01.024

