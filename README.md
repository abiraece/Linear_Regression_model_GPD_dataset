Table of Content:
1. Introduction and Data Description
2. Data Preprocessing
3. Modeling Phase
4. Evalution Metrics
5. Conclusion

Introduction and Data Description:

Our Objective is to predict GDP of the country

The data definition is as follows: Country,Population of the country,Area_sqm,Population_Density_Per_sqm,Coastline (coast/area ratio), Country,Population,Area_sqm,Pop_Density_per sqm,,Net migration,Infant mortality (per 1000 births), GDP ($ per capita),Literacy (%),Phones (per 1000),Arable (%),Crops (%),Other (%),Climate,Birthrate,Deathrate,Agriculture, Industry,Service.

Data Preprocessing:

    1. Finded datatypes of entire dataset
    2. Imputed Null Values and missing values are imputed based on KNNImputer
    3. To avoid outlier to affect model performance, outlier are treated by capping method.
    
Modeling Phase:

    1. Basic Least Square model is built.
    2. To check for 5 assumption to build Linear Regression model further. 
        a. Multicollinearity effect is statisfied for some input features
        b. Normality test is statisfied with skewness of 0.2         
        c. Linearity test is statisfied 
        d. Autocorrelation test is statisfied         
        e. Homoscadacity test is also statisfied
    3. Different Feature selection algorithm are performed
    
Conclusion:
    
    Overall Performance of the model was 79.7%
