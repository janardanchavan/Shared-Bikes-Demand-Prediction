# Shared Bikes Demand Prediction Model
> A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

> Company wants to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

> - Which variables are significant in predicting the demand for shared bikes.
> - How well those variables describe the bike demands


## Table of Contents
* [Importing Data]()
* [Reading data]()
* [Data preparation]()
    * [Outlier Analysis]()
* [Exploratory Data Anlysis]()
    * [Visualizing Numerical variables]()
    * [Feature Elimination - I]()
    * [Visualizing Numerical variables]()
    * [Feature Elimination - II]()
    * [Dummy Variables]()
* [Splitting data into the Training and Test Sets]()
* [Rescalling the features]()
* [Building Linear Regression Model]()
    * [RFE - Recursive Feature Elimination]()
    * [Building model using statsmodel]()
    * [Calculating VIF for the Model]()
* [Residual Analysis of the train data]()
* [Model Evaluation](Model-Evaluation)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- The Objective is to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.
- Data Source - Bike Demand data source is used in this code module. Below are the field details:
    - instant: record index
    - dteday : date
    - season : season (1:spring, 2:summer, 3:fall, 4:winter)
    - yr : year (0: 2018, 1:2019)
    - mnth : month ( 1 to 12)
    - holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
    - weekday : day of the week
    - workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
    + weathersit : 
        - 1: Clear, Few clouds, Partly cloudy, Partly cloudy
        - 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
        - 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
        - 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
    - temp : temperature in Celsius
    - atemp: feeling temperature in Celsius
    - hum: humidity
    - windspeed: wind speed
    - casual: count of casual users
    - registered: count of registered users
    - cnt: count of total rental bikes including both casual and registered

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- We can see that the climate has some impact on the modelling, eg. LightSnow and Mist
- As per above model, we can see that the users are perferring more shared bike either at the beginning of the year (Jan+Feb) or beginning of the quarter (Jul, Oct).

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Python libraries Used
- pandas - version: 1.4.4
- numpy - version: 1.21.5
- matplotlib - version: 3.5.2
- seaborn - version: 0.11.2
- sklearn - version: 0.0.post5
- statsmodels - version: 0.13.2
- warnings - version: 

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- This project is part of my upGrad master's degree program.


## Contact
Created by [@janardanchavan] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->