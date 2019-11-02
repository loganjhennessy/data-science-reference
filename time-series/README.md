# Definitions

What is the big idea?

Measurements of a single quantity are taken over time.

## Time series

Time series is a specific type of data, where measurements of single
quantity are taken over time.

##  Time-series data

The data that results from a time series.

# Fundamentals

##  Trend

Pretty intuitive. Defined as a gradual change in average level as time
moves on.

Trends can be increasing, decreasing, or neither.

A linear regression can be performed to draw a trend line.

Sometimes it is useful to look at a **detrended** series by subtracting
off the trend line that we just drew.

##  Seasonality

Does not have to strictly refer to "seasons", but more or less refers
to any cyclical process inherent in a time series.

##  Stickyness

Time series have high stickyness if there is a strong relationship
between the current point and any future point. This is as opposed to
them being independent.

# Classical decomposition

Breaking a time series down into it's components.

Typically, the components are:
- Raw series
- Trend component
- Seasonal component
- Residual component

# Stationarity vs independence

With white noise, the random distribution of the value of any
individual point is the same.

## Stationarity

A time series is stationary (or has high stationarity) if the
correlation between one data point and the next data point (i.e. the
stickyness) is the same no matter where the data is observed.

Stationary time series cannot show trends, and they cannot show
seasonality, and the variance of a station time series cannot change
over time.

However, stationary time series *can* be sticky. They just can't have
a varying amount of strickyness at different points in the series.

Stationary time series
ARIMA models
