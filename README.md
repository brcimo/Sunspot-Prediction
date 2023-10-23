# Sunspot-Prediction
Jupyter Notebook that uses NASA data to predict sunspots. Comparing ARIMA and LSTM.

In a paper by Saa and Ranathunga they compare autoregressive integrated moving average (ARIMA), a statistical method, against machine learning models including LSTM. Their paper is a study of a time-series of hourly temperature data. They found that by using a machine learning model, they can make a better prediction than the common statistical method, ARIMA.
Similarly, this project will also use an ARIMA and LSTM model to make a time-series forecast and compare the predicted values from each. (De Saa and Ranathunga 2020)

Data:

Sunspot data from National Oceanic and Atmospheric Administration, NOAA, will be used. The data is available in JSON, this format can be easily read into a python notebook using pandas. The dataset has current data back to the year 1749 and is available here: https://services.swpc.noaa.gov/json/solar-cycle/observed-solar-cycle-indices.json.

Data from the NOAA dataset is in JSON format and will be converted and transformed to a format to use in forecasting sunspot numbers. The project will load the data in a Pandas dataframe.

The data for this project is easy to obtain at the site listed above. It is in a publicly accessible website, in a JSON format. For this project the data will be manually downloaded by the ML Engineer for use in the project.

In the project we are planning to use Python Pandas to massage the data, delete nulls, and fix any missing values. First, we will load the data using Pandas as a dataframe. Then we will check the data for standard deviation and look for missing values and outliers. Next, we calculate a mean value for the data and check data types and convert if necessary. After that, we will rename and combine columns if needed.

If there is any missing data, it can be fixed several ways. We might insert a mean value or delete the row or change the missing value to 0, depending on what is needed. After this, we will look at grouping and sorting the data. Finally, we will check if the data needs to be transformed. We can use the Pandas map function to perform calculations on the data.

De Saa, E., & Ranathunga, L. (2020). Comparison between ARIMA and Deep Learning Models for Temperature Forecasting. ArXiv:2011.04452 [Cs]. Retrieved June 14, 2022, from https://arxiv.org/abs/2011.04452
