One Page Technical Report

Chosen Algorithm : Seasonal Naive Forecasting

Model Parameters

1. Seasonal Period
→ A  14-day lag is used so the model looks back two weeks instead of one. 
→ This avoids the effect of abnormal values in the last few days and gives a more stable seasonal reference.

2. Forecast Horizon
→ The prediction window is set  to 7 days, meaning the model forecasts ridership for the next week.

3. Frequency
→ The data is daily (freq='D'), so the model generates one forecast value per day.


Final Observation
My dataset has many missing days , sudden drops(holidays) and uneven seasonality . So I chose the Seasonal Naive Model.
This model predicts future ridership by repeating the values observed exactly 14 days earlier. The 14-day lag was selected because it provided a more stable and reliable seasonal pattern than a 7-day lag, especially considering the unusual fluctuations present in the final week of the dataset.
Using this approach,next-week forecasts for Local Route, Light Rail, Peak Service, Rapid Route, and School services were produced.
The predictions closely follow the established weekly seasonality observed during EDA higher ridership on weekdays and lower values on weekends. 
This behavior aligns with real operational patterns such as school closures, peak-hour variations, and reduced weekend demand.
To clearly interpret the results, the historical data and forecast values were plotted together. 
These visualizations highlight how the model continues the existing seasonal structure into the next week and provides a simple yet reliable estimate of expected ridership across all service types. 
The forecasted trends offer useful short-term planning insights for capacity management, resource allocation, and service scheduling.


