# NYC_Taxi_Demand_Forecasting

## Datasets Used:

1. NYC Yellow Taxi Trip Data: Public dataset from NYC Taxi & Limousine Commission containing timestamped trip-level info, geospatial pickup/drop-off zones, fare breakdowns, and payment types. (Source: https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
3.  NYC DOT Traffic Volume Counts Data: Collected via Automated Traffic Recorders across NYC roads and bridges, detailing hourly vehicle volume with GPS metadata. Used to contextualize taxi demand with real-world traffic conditions.  (Source: https://data.cityofnewyork.us/Transportation/Automated-Traffic-Volume-Counts/7ym2-wayt/data_preview)

## Key Objectives 

The objective of this project is to integrate the NYC Yellow Taxi Trip Data with NYC Traffic Volume Counts Data to analyze the impact of traffic patterns on taxi operations, predict taxi demand, and identify high-congestion and high-risk zones across New York City. By combining mobility and traffic datasets, this project aims to generate actionable insights to improve transportation efficiency, demand forecasting, and urban mobility planning. 

Here are the following areas of focuses from the dataset: 

- Taxi Demand Prediction: Forecast taxi pickup demand across NYC neighborhoods by leveraging traffic volume trends, historical trip data, and temporal patterns. Time-series modeling and feature-based machine learning techniques will be employed to capture demand fluctuations and rush hour dynamics. 

- Traffic Congestion Prediction: Analyze taxi pickup and drop-off activity as a proxy for urban congestion. Develop predictive models to identify traffic hotspots, delays, and heavy congestion periods based on taxi activity levels. 

- Visualization and Geospatial Analysis: Generate spatial heatmaps of pickup and drop-off events to highlight high-demand zones across boroughs and neighborhoods. 

- Traffic Zone Analysis: Study the relationship between traffic volume (measured by ATR sensors) and taxi trip frequency to uncover correlations between traffic congestion and taxi service patterns. 

- High-Risk Zone Identification: Map and monitor zones with consistently high congestion or demand variability to support targeted urban mobility improvements.

## Data Mining Techniques Used:
1. Correlation Analysis - to determine relationship between taxi fare-related features, traffic volume indicators and temporal index features.
2. Regression Analysis - Random Forest Regressor, Linear Regression, KNN Regressor Method,  XG Boost Regression Model - To model and predict hourly taxi demand
3. Classification Model -  can we predict a sudden traffic surge in a zone/hour using real-time taxi pickup activity and trends? By creating a binary classification problem, we can predict whether traffic surge happens (0/1) based on taxi pickup activity.
4. Cluster Analysis -  To group similar NYC pickup zones together based on their average taxi demand, trip distance, total fare, traffic volume, and passenger count.
5. Association Analysis - To explore co-occurring patterns in surge activity, I applied association rule mining using the Apriori algorithm on sampled chunks of NYC taxi data. 
   

