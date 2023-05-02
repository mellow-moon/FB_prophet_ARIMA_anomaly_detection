# FB_prophet_ARIMA_anomaly_detection

Anomaly detection using Facebook Prophet and ARIMA methods.

# Dataset

This dataset contains sales data in Walmart stores. Data has 421570 rows and 16 columns.

<img src="img/walmart_df.png" width="400"/>

In this project we will use only Weekly Sales for Store 1.

<img src="img/weekly_sales_store_one.png" width="400"/>

# Resample Data

We will resample data by day and take the mean values. Below is a plot of resampled dataset.

<img src="img/resampled_weekly_data.png" width="400"/>

# Autocorrelation and Partial Autocorrelation

Plot autocorrelation and partial autocorrelation.

<img src="img/autocorr_pacf.png" width="400"/>

# Holiday Events

We have information about holiday events that we can use in Prophet model.

<img src="img/holiday_events.png" width="400"/>

Let's create a table that we will pass to the model.

<img src="img/holiday_table.png" width="400"/>

# Train Dataset

Let's create train dataset.

<img src="img/train_data.png" width="400"/>

# Prophet Model

Let's train the model with the following parameters.

<img src="img/fb_prophet.png" width="400"/>

And then make a prediction with our model.

<img src="img/prophet_prediction.png" width="400"/>

# Anomaly Detection

To detect anomalies we need to calculate our model's errors and confidence intervals. If error is bigger than 1.5*(uncertanity) that is anomaly.

<img src="img/model_performance.png" width="400"/>

We can see that we have 8 anomalies in our data.

<img src="img/anomaly_detection_prophet.png" width="400"/>

Let's plot anomaly observations.

<img src="img/prophet_anomaly_plot.png" width="400"/>

# ARIMA model

# Split the data

Let's split the data and set the parameters of ARIMA model.

<img src="img/arima_data_split.png" width="500"/>

# ARIMA Training

Now let's train our model.

<img src="img/arima_params.png" width="500"/>

After training is over we can make a prediction and plot it.

<img src="img/arima_predictions.png" width="500"/>

# Anomaly Detection

To detect anomalies we need to calculate our model's errors and confidence intervals.

<img src="img/arima_anomaly_detection.png" width="500"/>

If error is bigger than 1.5*(uncertanity) that is anomaly.

<img src="img/arima_anomalies.png" width="500"/>

ARIMA model found two anomalies in our data. Let's plot it.

<img src="img/arima_anomalies_plot.png" width="500"/>
