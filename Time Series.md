# What is a Time Series ?
* Any metric that is measured over regular time intervals makes a Time Series. 
* Example: Weather data, Stock prices, Industry forecasts, etc are some of the common ones.
# How to create a Time Series in R ?
> ts (inputData, frequency = 4, start = c(1959, 2)) # frequency 4 => Quarterly Data

> ts (1:10, frequency = 12, start = 1990) # freq 12 => Monthly data. 

> ts (inputData, start=c(2009), end=c(2014), frequency=1) # Yearly Data
# Understanding your Time Series
* Each data point (Yt) at time t in a Time Series can be expressed as either a sum or a product of 3 components, 
> namely, Seasonality (St), Trend (Tt) and Error (et) (a.k.a White Noise).
# What is a Stationary Time Series ?
> A time series is said to be stationary if it holds the following conditions true.
* The mean value of time-series is constant over time, which implies, the trend component is nullified.
* The variance does not increase over time.
* Seasonality effect is minimal. 
> This means it is devoid of trend or seasonal patterns, which makes it looks like a random white noise irrespective of the observed time interval.
# Stationarize a Time Series
### Most statistical forecasting methods are based on the assumption that the time series can be rendered approximately stationary (i.e., "stationarized") through the use of mathematical transformations. 
* A stationarized series is relatively easy to predict: you simply predict that its statistical properties will be the same in the future as they have been in the past!   (Recall our famous forecasting quotes.)  
* The predictions for the stationarized series can then be "untransformed," by reversing whatever mathematical transformations were previously used, to obtain predictions for the original series. (The details are normally taken care of by your software.) 
* Thus, finding the sequence of transformations needed to stationarize a time series often provides important clues in the search for an appropriate forecasting model.  
* Stationarizing a time series through differencing (where needed) is an important part of the process of fitting an ARIMA model.
### Another reason for trying to stationarize a time series is to be able to obtain meaningful sample statistics such as means, variances, and correlations with other variables. 
* Such statistics are useful as descriptors of future behavior only if the series is stationary. 
* For example, if the series is consistently increasing over time, the sample mean and variance will grow with the size of the sample, and they will always underestimate the mean and variance in future periods. And if the mean and variance of a series are not well-defined, then neither are its correlations with other variables. For this reason you should be cautious about trying to extrapolate regression models fitted to nonstationary data.
