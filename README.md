
## Problem Statement

Time-series forecasting and Regression


- To find number of pickups, given location cordinates(latitude and longitude) and time, in the query reigion and surrounding regions.


## Data Information

Get the data from : http://www.nyc.gov/html/tlc/html/about/trip_record_data.shtml (2016 data) The data used in the attached datasets were collected and provided to the NYC Taxi and Limousine Commission (TLC)

We Have collected all yellow taxi trips data from july-2022 to November-2022.


## Performance metrics

 -  Mean Absolute percentage error.
 -  Mean Squared error.


### Information on taxis:


- Yellow Taxi: Yellow Medallion Taxicabs 
These are the famous NYC yellow taxis that provide transportation exclusively through street-hails. The number of taxicabs is limited by a finite number of medallions issued by the TLC. You access this mode of transportation by standing in the street and hailing an available taxi with your hand. The pickups are not pre-arranged.

- For Hire Vehicles (FHVs) :
FHV transportation is accessed by a pre-arrangement with a dispatcher or limo company. These FHVs are not permitted to pick up passengers via street hails, as those rides are not considered pre-arranged.

- Green Taxi: Street Hail Livery (SHL) 
The SHL program will allow livery vehicle owners to license and outfit their vehicles with green borough taxi branding, meters, credit card machines, and ultimately the right to accept street hails in addition to pre-arranged rides.

Credits: Quora




## Features in the dataset:


| Feature Name        | Description  | 
| ------------- |:-------------:| 
| VendorID      | A code indicating the TPEP provider that provided the record. 1. Creative Mobile Technologies 2. VeriFone Inc. | 
| tpep_pickup_datetime      | The date and time when the meter was engaged.      | 
| tpep_dropoff_datetime | The date and time when the meter was disengaged.     | 
| Passenger_count | The number of passengers in the vehicle. This is a driver-entered value.      |
| Trip_distance | The elapsed trip distance in miles reported by the taximeter.     |
| Pickup_longitude | Longitude where the meter was engaged.     |
| Pickup_latitude | Latitude where the meter was engaged.     |
| RateCodeID | The final rate code in effect at the end of the trip. 1. Standard rate 2. JFK 3. Newark 4. Nassau or Westchester 5. Negotiated fare 6. Group ride|
| Store_and_fwd_flag | This flag indicates whether the trip record was held in vehicle memory before sending to the vendor, aka “store and forward,” because the vehicle did not have a connection to the server. Y= store and forward trip N= not a store and forward trip      |



## Data Modeling
```
1. Data preparation: Clean and prepare the data by handling missing values, transforming variables, and aggregating the data if necessary.
2. Model selection: Select the appropriate time series model based on the characteristics of the data, such as trend, seasonality, and autocorrelation.
3. Model fitting: Fit the selected model to the data using an appropriate method such as maximum likelihood estimation.
4. Model evaluation: Evaluate the performance of the model using metrics such as mean absolute error, mean squared error, and root mean squared error.
5. Model tuning: Fine-tune the model by adjusting its parameters to improve its performance.
6. Model deployment: Deploy the model for use in a production environment, making predictions about future values.

```


## Observation
This Observation on Cluster 1 region and there are 30 Cluster regions. To find all the forecasting just import the cluster file in coding block and you'll get the 
predicted value.

![Observation](https://i.ibb.co/Gxrtw82/time-series.png)

- MAE : 13.06087039129284
- MSE : 299.81293832847683



## Conclusion

- In conclusion, time series forecasting is a widely used and important technique for predicting future values based on past data. It is a crucial tool for many industries, including finance, economics, and retail, where accurate predictions are critical for making informed decisions. Time series forecasting can be performed using a variety of methods, ranging from traditional statistical models such as ARIMA and SARIMAX, to more advanced techniques such as exponential smoothing and deep learning models.
Regardless of the method used, the process of time series forecasting involves several key steps, including data preparation, model selection, model fitting, model evaluation, model tuning, and model deployment. It is important to choose the appropriate model based on the characteristics of the data and the specific use case, and to evaluate the performance of the model to ensure that it is making accurate predictions.

