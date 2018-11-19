---
title: Why time series analysis needs stationarity
layout: post
---
We have long been concerned that non-stationary data should be first converted into stationary data, 
so that further statistical analysis can be done on the detrended stationary data. Also, it is mentioned 
that most of the statistical tools assume that the data is stationary, that is why it is important to make 
the non-stationary data stationary. But what is exactly where the stationarity assumption is required and if 
my data is non-stationary and I still use statistical analysis which result is going to be in error? 

First let's decide what form of stationarity you are asking about. There are two types:
(1) strict stationarity: All aspects of a time series behavior are not dependent on time.

(2) weak stationarity (sometimes called covariance stationary): mean, variance, covariance not chage according to time.

strict stationarity and weak stationarity are equivalent for Gaussian processes, since a normal distribution 
is uniquely characterized by its first two moments.

Noticed that covariance and correlation are both functions of the mean and variance. So for example, if the 
series is consistently increasing over time, the sample mean and variance will grow with the size of the sample, 
and they will always underestimate the mean and variance in future periods. And if the mean and variance of a 
series are not well-defined, then neither are its correlations with other variables.

Most statistical forecasting methods are based on the assumption that the time series can be rendered approximately 
stationary (i.e., "stationarized") through the use of mathematical transformations. A stationarized series is relatively 
easy to predict: you simply predict that its statistical properties will be the same in the future as they have been in the past!

There are multiple methods for making a time series stationary, which include detrending and first differencing. You can find 
many descriptions of both on websites. The Duke U link above explains first differencing. Forecasts and means/variances can be 
made with the detrended model, and then the model can be converted back to the original.
