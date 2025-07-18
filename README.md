# Data-Analytics--UE22CS342AA2 Hackathon 

## About the dataset 
RideWave, a versatile urban mobility service, has been operating in Quahog City for the past five years. The company offers three types of vehicles: bikes, autos (three-wheeled vehicles), and cars. As they face increasing competition, RideWave wants to leverage its historical data to optimize pricing strategies for each vehicle type in Quahog City.

## Task
The dataset contains hourly data from 2021 to 2023 for bikes, autos and cars from RideWave.The task provided was to analyze the provided data, develop predictive models for fare forecasting, and provide actionable insights to help RideWave implement dynamic pricing across its multi-vehicle fleet in Quahog City.

## Evaluation Metric 
<img width="954" height="233" alt="image" src="https://github.com/user-attachments/assets/a9ec5a5b-62ff-45f6-aa72-c6eb7e8b14bd" />

## Approach
Used the Holt Winters Model for forecasting the usage of Holt Winters Model is justified for the following reasons : 
1. Presence of Seasonality
* Holt-Winters is specifically designed to handle seasonality in time series data. It works well when the data exhibits clear periodic trends (seasonality) and/or a trend component. In your case, if the data has repeating patterns (e.g., weekly, monthly), the seasonal component of the Holt-Winters method is particularly useful.

* The additive or multiplicative seasonal components in the Holt-Winters method can capture regular seasonal fluctuations, making it a good choice for datasets where these seasonal effects are prominent, like transportation fare data that might exhibit patterns related to time of day, week, or year.

2. Incorporation of Trend
* Holt-Winters also accounts for the trend in the data. If the data has a consistent upward or downward trend (e.g., increasing fares over time), the trend component in Holt-Winters helps model this aspect and make forecasts accordingly.

## Result 
* sMAPE for Bike: 16
* sMAPE for Auto: 16
* sMAPE for Car: 0
* Overall sMAPE: 11

  
