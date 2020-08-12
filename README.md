# Air-Pollution-Forecasting
An LSTM model to predict the pollution levels in the next hour using the weather conditions and pollution levels in the current hour. I have trained the model using both uni-variate(if we consider only one feature) and multi-variate(when we consider multiple features for prediction).

## Dataset
In this, I have used the Air Quality dataset. This is a dataset that reports on the weather and the level of pollution each hour for five years at the US embassy in Beijing, China. The data includes the date-time, the pollution called PM2.5 concentration, and the weather information including dew point, temperature, pressure, wind direction, wind speed and the cumulative number of hours of snow and rain. 

## Steps followed
- Data preparation
- Data visualization
- LSTM data preparation
- Fit model along with regularization term
- Evaluate model

### Data preparation
- Replace NA values
- Parse date-time into pandas dataframe index
- Specified clear names for each columns

### Data visualization
- Used boxplot
- Correlation matrix

### LSTM data preparation
- Normalized data
- Transformed dataset into supervised learning problem

### Model Fitting
- Split data into train and test
- Split into i/p and o/p
- Reshape into 3D
- Define 3 layer LSTM architecture with 50 neuron followed by 1 nueron LSTM
- Add dropout at 20% after every layer

### Evaluate model
- Make prediction
- Invert scaling
- Plot the line graph between actual vs predicted values
- Calculate RMSE(root mean squared errot) and MAPE(mean absolute percentage error)

### Results
<div style="float:left">
<div style="float:left"><img src="https://github.com/jyoti0225/Air-Pollution-Forecasting/blob/master/output_graph.png" />
</div>
<br />
