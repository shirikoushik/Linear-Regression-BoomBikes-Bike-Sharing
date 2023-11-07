# BoomBikes-Bike-Sharing-Assignment
![unnamed](https://github.com/shirikoushik/BoomBikes-Bike-Sharing-Assignment/assets/35067803/0acc1aca-d734-46fa-a57d-75258a8630a9)

# Problem Statement:
A US bike-sharing provider BoomBikes a Mobility Services firm has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

Essentially the company wants :

To understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19, by creating a linear model.
To identify the variables affecting their revenues i.e. Which variables are significant in predicting the demand for shared bikes.
To know the accuracy of the model, i.e. How well those variables describe the bike demands
They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

# Business Goal:
You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.

# My solution:
Built a robust linear regression model which is able to explain around 80% of the bike demand and evaluated the model on various statistical metrics like variance inflation factor, r2_score and found the factors impacting the bike demand.
  ## Insights:
  ![image](https://github.com/shirikoushik/BoomBikes-Bike-Sharing-Assignment/assets/35067803/166c3b1d-811a-4764-9828-3ee5222b2a3b)
  1) Fall has the highest bike demand
  2) The demand is increasing monthly till sep reaching max and then it is going down
  3) Not much difference in demand for bikes daywise
  4) Most demand on Clear weathersit condition
  5) The demand is decreased on holidays
  6) Demand has increased a lot compared to previous year
     
  ## Best fit line equation:
  cnt = 0.2060 + 0.2335  *  year - 0.1052  *  holiday + 0.4907 * temp - 0.1479 * windspeed - 0.0655 * season_spring + 0.0475 * season_summer + 0.0848 * season_winter - 0.0492 * month_july + 0.0760 * month_sep - 0.0483 * weekday_sun - 0.2895 * weathersit_Light_snow_rain - 0.0822 * weathersit_Mist
  
  ## Conclusions based on the LR model:
  1) The variables in our model are able to explain around 80% of bike demand
  2) Top 3 factors impacting the bike demand:
     temp(+0.4907)
     year(+0.2335)
     weathersit_Light_snow_rain + weathersit_Mist + windspeed (-0.29) 

