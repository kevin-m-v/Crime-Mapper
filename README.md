# Miami Crime Mapper

"Crime Mapper.ipynb" contains my project's source code, implementation process, and figures. "Miami_Dade_0.csv" is the dataset webscraped from crimemapping.com.

This project aimed to analyze the risk of violent crime in different regions of Miami-Dade County. First, the county is divided into a grid where every square is attributed to a neighborhood in Miami. Each grid square was classified according to the total number of crimes, the number of violent crimes, and wealth disparity(quantified using the Gini-Index, obtained with the U.S. Census API). Machine learning was implemented to offer efficient predictive analysis of rising crime in a region. Using the provided classifications, the decision tree algorithm observed the common trends between the features of each grid square within a class. The resulting tree offered more accurate metrics to base future classifications on. After research and testing with K-Nearest-Neighbor, Decision Tree, and Random Forest, Decision Tree proved to be the most applicable machine learning algorithm for the final implementation.

![alt text](https://github.com/kevin-m-v/Crime-Mapper/blob/main/Decision%20Tree.png)

The Google Maps API was instrumental in the classification step. The raw crime data provides street addresses that could not be mapped to a grid. However, latitude and longitude coordinates, obtained by sending the street address through the Google Maps API, were quantifiable metrics that allowed me to attribute crimes to individual grid squares.

![alt text]([https://github.com/kevin-m-v/Crime-Mapper/blob/main/Decision%20Tree.png](https://github.com/kevin-m-v/Crime-Mapper/blob/main/Crime%20Hotspot%20Map.png))

The Crime Mapper can be an invaluable asset to visitors, locals, and law enforcement by clearly identifying high-risk areas in Miami and offering insights into the association between crime and socio-economic conditions.
