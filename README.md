# Time Series Analysis and Forecasting Depth To Underground Water of Luco Aquifer
[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
![Magic](https://img.shields.io/badge/Made%20with-Time-yellow?style=for-the-badge&logo=data:image/svg%2bxml;base64,PHN2ZyBpZD0iQ2FwYV8xIiBlbmFibGUtYmFja2dyb3VuZD0ibmV3IDAgMCA1MTIgNTEyIiBoZWlnaHQ9IjUxMiIgdmlld0JveD0iMCAwIDUxMiA1MTIiIHdpZHRoPSI1MTIiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGc+PHBhdGggZD0ibTM5NS44MiAxODIuNjE2LTE4OC43MiAxODguNzItMTIuOTEgMS43Mi05LjM1IDIwLjU0LTM0LjMxIDM0LjMxLTExLjAxLS43My0xMS4yNSAyMi45OS01Ni40OCA1Ni40OGMtMi45MyAyLjkzLTYuNzcgNC4zOS0xMC42MSA0LjM5cy03LjY4LTEuNDYtMTAuNjEtNC4zOWwtMjIuNjItMjIuNjJoLS4wMWwtMjIuNjItMjIuNjNjLTUuODYtNS44Ni01Ljg2LTE1LjM2IDAtMjEuMjJsNzcuNjMtNzcuNjMgMTYuNi03LjAzIDUuNjYtMTUuMjMgMzQuMzEtMzQuMzEgMTQuODQtNC45MiA3LjQyLTE3LjM0IDE2Ny41Ny0xNjcuNTcgMzMuMjQgMzMuMjR6IiBmaWxsPSIjZjY2Ii8+PHBhdGggZD0ibTM5NS44MiAxMTYuMTQ2djY2LjQ3bC0xODguNzIgMTg4LjcyLTEyLjkxIDEuNzItOS4zNSAyMC41NC0zNC4zMSAzNC4zMS0xMS4wMS0uNzMtMTEuMjUgMjIuOTktNTYuNDggNTYuNDhjLTIuOTMgMi45My02Ljc3IDQuMzktMTAuNjEgNC4zOXMtNy42OC0xLjQ2LTEwLjYxLTQuMzlsLTIyLjYyLTIyLjYyIDMzNC42NC0zMzQuNjR6IiBmaWxsPSIjZTYyZTZiIi8+PHBhdGggZD0ibTUwNi42MSAyMDkuMDA2LTY5LjE0LTY5LjEzIDQzLjA1LTg4LjM4YzIuOC01Ljc1IDEuNjUtMTIuNjUtMi44OC0xNy4xNy00LjUyLTQuNTMtMTEuNDItNS42OC0xNy4xNy0yLjg4bC04OC4zOCA0My4wNS02OS4xMy02OS4xNGMtNC4zNS00LjM1LTEwLjkyLTUuNi0xNi41Ni0zLjE2LTUuNjUgMi40NS05LjIzIDguMDktOS4wNCAxNC4yNGwyLjg2IDkwLjQ1LTg1LjM3IDU3LjgzYy00LjkxIDMuMzItNy40IDkuMjItNi4zNiAxNS4wNCAxLjA0IDUuODMgNS40IDEwLjUxIDExLjE1IDExLjk0bDk2LjYyIDI0LjAxIDI0LjAxIDk2LjYyYzEuNDMgNS43NSA2LjExIDEwLjExIDExLjk0IDExLjE1Ljg3LjE2IDEuNzUuMjMgMi42Mi4yMyA0LjkyIDAgOS42LTIuNDIgMTIuNDItNi41OWw1Ny44My04NS4zNyA5MC40NSAyLjg2YzYuMTQuMTkgMTEuNzktMy4zOSAxNC4yNC05LjA0IDIuNDQtNS42NCAxLjE5LTEyLjIxLTMuMTYtMTYuNTZ6IiBmaWxsPSIjZmFiZTJjIi8+PHBhdGggZD0ibTI5Ni4yNiAyMTUuNzA2IDI0LjAxIDk2LjYyYzEuNDMgNS43NSA2LjExIDEwLjExIDExLjk0IDExLjE1Ljg3LjE2IDEuNzUuMjMgMi42Mi4yMyA0LjkyIDAgOS42LTIuNDIgMTIuNDItNi41OWw1Ny44My04NS4zNyA5MC40NSAyLjg2YzYuMTQuMTkgMTEuNzktMy4zOSAxNC4yNC05LjA0IDIuNDQtNS42NCAxLjE5LTEyLjIxLTMuMTYtMTYuNTZsLTY5LjE0LTY5LjEzIDQzLjA1LTg4LjM4YzIuOC01Ljc1IDEuNjUtMTIuNjUtMi44OC0xNy4xN3oiIGZpbGw9IiNmZDkwMjUiLz48cGF0aCBkPSJtNDY1IDQxNi45NjZjLTI1LjkyIDAtNDcgMjEuMDgtNDcgNDdzMjEuMDggNDcgNDcgNDcgNDctMjEuMDggNDctNDctMjEuMDgtNDctNDctNDd6IiBmaWxsPSIjZmFiZTJjIi8+PHBhdGggZD0ibTEwNCAyOC45NjZoLTEzdi0xM2MwLTguMjg0LTYuNzE2LTE1LTE1LTE1cy0xNSA2LjcxNi0xNSAxNXYxM2gtMTNjLTguMjg0IDAtMTUgNi43MTYtMTUgMTVzNi43MTYgMTUgMTUgMTVoMTN2MTNjMCA4LjI4NCA2LjcxNiAxNSAxNSAxNXMxNS02LjcxNiAxNS0xNXYtMTNoMTNjOC4yODQgMCAxNS02LjcxNiAxNS0xNXMtNi43MTYtMTUtMTUtMTV6IiBmaWxsPSIjZmVkODQzIi8+PHBhdGggZD0ibTIwNy4xIDM3MS4zMzYtMjIuMjYgMjIuMjYtNDUuMzItODcuNjIgMjIuMjYtMjIuMjZ6IiBmaWxsPSIjZmVkODQzIi8+PHBhdGggZD0ibTE4NC44NCAzOTMuNTk2IDIyLjI2LTIyLjI2LTIyLjY2LTQzLjgxLTIyLjI2NSAyMi4yNjV6IiBmaWxsPSIjZmFiZTJjIi8+PHBhdGggZD0ibTE1MC41MyA0MjcuOTA2LTIyLjI2IDIyLjI2LTQ1LjMyLTg3LjYyIDIyLjI2LTIyLjI2eiIgZmlsbD0iI2ZlZDg0MyIvPjxwYXRoIGQ9Im0xMjguMjcgNDUwLjE2NiAyMi4yNi0yMi4yNi0yMi42NTUtNDMuODE1LTIyLjI2IDIyLjI2eiIgZmlsbD0iI2ZhYmUyYyIvPjxjaXJjbGUgY3g9IjE1IiBjeT0iMTE5Ljk2OSIgZmlsbD0iIzVlZDhkMyIgcj0iMTUiLz48Y2lyY2xlIGN4PSIxMjgiIGN5PSIxOTkuOTY5IiBmaWxsPSIjZDU5OWVkIiByPSIxNSIvPjxjaXJjbGUgY3g9IjE5MiIgY3k9IjYzLjk2NCIgZmlsbD0iI2Y2NiIgcj0iMTUiLz48Y2lyY2xlIGN4PSIzMjgiIGN5PSI0MTUuOTY3IiBmaWxsPSIjMzFiZWJlIiByPSIxNSIvPjxjaXJjbGUgY3g9IjQ0MCIgY3k9IjMyNy45NjciIGZpbGw9IiNhZDc3ZTMiIHI9IjE0Ljk5OSIvPjwvZz48L3N2Zz4=)
![Time](https://img.shields.io/badge/Time%20Series-Analysis-yellow?style=for-the-badge&logo=data:image/svg%2bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA1MTIgNTEyIj48cGF0aCBkPSJNMTQ5Ljk0NCAxMDEuNjA3bC0yOS44OTYtMjkuOTU4Yy02LjkzNS02Ljk0OS0xNi4xNi0xMC43NzUtMjUuOTc3LTEwLjc3NXMtMTkuMDQyIDMuODI3LTI1Ljk3NiAxMC43NzVMNDYuNDI0IDkzLjM2N2MtMTQuMjY1IDE0LjI5My0xNC4yNjUgMzcuNTUxIDAgNTEuODQ1bDI5Ljk1OSAzMC4wMjFhMTQuOTUyIDE0Ljk1MiAwIDAwMTAuNjE4IDQuNDA0YzMuODMzIDAgNy42NjgtMS40NjEgMTAuNTk2LTQuMzgyIDUuODY0LTUuODUyIDQ2LjQ3LTQ2LjU5MSA1Mi4zMjYtNTIuNDM1IDUuODYzLTUuODUxIDUuODczLTE1LjM0OC4wMjEtMjEuMjEzeiIgZmlsbD0iIzEwNWM2ZSIvPjxwYXRoIGQ9Ik0yNTYgM2MtOC4yODQgMC0xNSA2LjcxNi0xNSAxNXY0OGMwIDguMjg0IDYuNzE2IDE1IDE1IDE1IDguMjg0IDAgMTUtNi43MTYgMTUtMTVWMThjMC04LjI4NC02LjcxNi0xNS0xNS0xNXoiIGZpbGw9IiMyNjg3OWMiLz48cGF0aCBkPSJNMjkzIDBoLTc0Yy04LjI4NCAwLTE1IDYuNzE2LTE1IDE1czYuNzE2IDE1IDE1IDE1aDc0YzguMjg0IDAgMTUtNi43MTYgMTUtMTVzLTYuNzE2LTE1LTE1LTE1eiIgZmlsbD0iI2RlNTEzYyIvPjxwYXRoIGQ9Ik0yNTYgMGgtMzdjLTguMjg0IDAtMTUgNi43MTYtMTUgMTVzNi43MTYgMTUgMTUgMTVoMzdWMHoiIGZpbGw9IiNmYzYyNDkiLz48cGF0aCBkPSJNNDE4LjY0NSAxMTguNjE1QzM3NS4yMDMgNzUuMDgzIDMxNy40NDEgNTEuMTA4IDI1NiA1MS4xMDhTMTM2Ljc5NyA3NS4wODMgOTMuMzU1IDExOC42MTVjLTQzLjQzNCA0My41MjQtNjcuMzU0IDEwMS4zOTEtNjcuMzU0IDE2Mi45MzlzMjMuOTIgMTE5LjQxNSA2Ny4zNTQgMTYyLjkzOUMxMzYuNzk3IDQ4OC4wMjUgMTk0LjU1OSA1MTIgMjU2IDUxMnMxMTkuMjAzLTIzLjk3NSAxNjIuNjQ1LTY3LjUwN2M0My40MzQtNDMuNTI0IDY3LjM1NC0xMDEuMzkxIDY3LjM1NC0xNjIuOTM5cy0yMy45Mi0xMTkuNDE1LTY3LjM1NC0xNjIuOTM5eiIgZmlsbD0iI2RlNTEzYyIvPjxwYXRoIGQ9Ik0yNTYgNTEuMTA4Yy02MS40NDEgMC0xMTkuMjAzIDIzLjk3NS0xNjIuNjQ1IDY3LjUwNy00My40MzQgNDMuNTI0LTY3LjM1NCAxMDEuMzkxLTY3LjM1NCAxNjIuOTM5czIzLjkyIDExOS40MTUgNjcuMzU0IDE2Mi45MzlDMTM2Ljc5NyA0ODguMDI1IDE5NC41NTkgNTEyIDI1NiA1MTJWNTEuMTA4eiIgZmlsbD0iI2ZjNjI0OSIvPjxwYXRoIGQ9Ik0yNTYgMTA4LjUzOGMtOTUuMjE4IDAtMTcyLjY4NCA3Ny42MTQtMTcyLjY4NCAxNzMuMDE1UzE2MC43ODIgNDU0LjU2OSAyNTYgNDU0LjU2OXMxNzIuNjg0LTc3LjYxNSAxNzIuNjg0LTE3My4wMTZTMzUxLjIxOCAxMDguNTM4IDI1NiAxMDguNTM4eiIgZmlsbD0iIzk2ZDFkOSIvPjxwYXRoIGQ9Ik0yNTYgMTA4LjUzOGMtOTUuMjE4IDAtMTcyLjY4NCA3Ny42MTQtMTcyLjY4NCAxNzMuMDE1UzE2MC43ODIgNDU0LjU2OSAyNTYgNDU0LjU2OVYxMDguNTM4eiIgZmlsbD0iI2Y0ZjJlNiIvPjxnIGZpbGw9IiMxMDVjNmUiPjxwYXRoIGQ9Ik0yNTYgMTQ2LjAwN2M4LjI4NCAwIDE1LTYuNzE2IDE1LTE1di0yMS44MDhjLTQuOTQ1LS40MjgtOS45NDYtLjY2LTE1LS42NnMtMTAuMDU1LjIzMi0xNSAuNjZ2MjEuODA4YzAgOC4yODQgNi43MTYgMTUgMTUgMTV6TTI1NiA0MTcuMTAxYy04LjI4NCAwLTE1IDYuNzE2LTE1IDE1djIxLjgwOGM0Ljk0NS40MjggOS45NDYuNjYgMTUgLjY2czEwLjA1NS0uMjMyIDE1LS42NnYtMjEuODA4YzAtOC4yODQtNi43MTYtMTUtMTUtMTV6TTQyOC4wMjggMjY2LjU1NGgtMjEuNDgxYy04LjI4NCAwLTE1IDYuNzE2LTE1IDE1czYuNzE2IDE1IDE1IDE1aDIxLjQ4MWMuNDI2LTQuOTQ1LjY1Ni05Ljk0Ni42NTYtMTVzLS4yMy0xMC4wNTUtLjY1Ni0xNXpNMTIwLjQ1MyAyODEuNTU0YzAtOC4yODQtNi43MTYtMTUtMTUtMTVIODMuOTcyYy0uNDI2IDQuOTQ1LS42NTYgOS45NDYtLjY1NiAxNXMuMjMgMTAuMDU1LjY1NiAxNWgyMS40ODFjOC4yODQgMCAxNS02LjcxNiAxNS0xNXpNMjkzIDI3Mi44OTdoLTIxLjE2MlYyMTIuMjNjMC04LjI4NC02LjcxNi0xNS0xNS0xNS04LjI4NCAwLTE1IDYuNzE2LTE1IDE1djc1LjY2N2MwIDguMjg0IDYuNzE2IDE1IDE1IDE1SDI5M2M4LjI4NCAwIDE1LTYuNzE2IDE1LTE1cy02LjcxNi0xNS0xNS0xNXoiLz48L2c+PC9zdmc+)

## Introduction
This is a time series analysis project to analyse and predict the depth to underground water level of Luco Aquifer. Here, I performed univariate analysis but I will go through the steps for cleaning the data in general and subset variables which I think might be useful for downstream multivariate analysis. 

The data was provided from The Acea Group fromItaly. The Acea Group is one of the leading Italian multiutility operators. Listed on the Italian Stock Exchange since 1999, the company manages and develops water and electricity networks and environmental services. Acea is the foremost Italian operator in the water services sector supplying 9 million inhabitants in Lazio, Tuscany, Umbria, Molise, Campania.

They've provided several datasets on several waterbody in Italy. As it is easy to imagine, a water supply company struggles with the need to forecast the water level in a waterbody (water spring, lake, river, or aquifer) to handle daily consumption. During fall and winter waterbodies are refilled, but during spring and summer they start to drain. To help preserve the health of these waterbodies it is important to predict the most efficient water availability, in terms of level and water flow for each day of the year. The Acea Group deals with four different type of waterbodies: water springs, lakes, rivers and aquifers. In this analytics, we'll look specifically at Luco Aquifer.

## Table of content

- [Background](#background)
- [Data Wrangling](#Data-Wrangling)
- [Exploratory Analysis](#Exploratory-Analysis)
- [Fitting Models And Forecasting](#Fitting-Models-And-Forecasting)
- [Conclusion](#Conclusion)

## Background
[Back to top](#table-of-content)

### Problem definition
For this project, we are trying to answer the question of *What is the future depth to underground water level for Luco Aquifer?*

### What is an aquifer?
According to NationalGeography, an aquifer is a body of rock and/or sediment that holds groundwater. Groundwater is the word used to describe precipitation that has infiltrated the soil beyond the surface and collected in empty spaces underground. A common misconception about aquifers is that they are underground rivers or lakes. While groundwater can seep into or out of aquifers due to their porous nature, it cannot move fast enough to flow like a river. The rate at which groundwater moves through an aquifer varies depending on the rock’s permeability. When a water-bearing rock readily transmits water to wells and springs, it is called an aquifer. The picture below taken from [Wikipedia](https://commons.wikimedia.org/w/index.php?curid=2152154) (By © Hans Hillewaert) illustrates two different types of aquifer.

<p align="center">
    <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/Aquifer_en.svg" alt="Wikipedia examples of different types of Aquifers">
</p>


## Data Wrangling
[Back to top](#table-of-content)

The data obtained started from `2000-01-01`until `2020-06-30` with 22 columns/ variables. However, there were quite a few missing values. As such, I decided to explore the missing values and impute them.

### Missing Values
#### Missing values per variables
The table below shows the amount of missing values in the original dataframe. As you can see, given that the dimension of the data is 7487 x 23, some variables have *a lot* of missing data.

<p align="center">
    <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/miss_var_table.png" alt="Missing values for different variables">
</p>

#### Patterns of Missing Variables
The graph below shows the variables that tend to be missing together. The Dept to Underground water variables tend to be missing together, and the same goes for the different volume of different pozzo. Knowing these patterns help to identify what variables to keep/ discard if we wanted to use multivariate analysis later.

<p align="center">
    <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/Missing_patterns.png" alt="Patterns of Missing Variables">
</p>

#### Patterns of Missing Values By Year
The chart below shows the patterns of missing values for each variables by year. The target output is `Depth_to_Groundwater_Podere_Casetta`, which was missing prior to 2008 and after 2018. Therefore, I decided to use subset the dataset and used the data between 2008 and 2018. Based on the missing paterns, I decided to keep only 'Date', 'Depth_to_Groundwater_Podere_Casetta', 'Temperature_Pentolina', 'Temperature_Monteroni_Arbia_Biena','Rainfall_Simignano', 'Rainfall_Montalcinello', 'Rainfall_Sovicille', 'Rainfall_Scorgiano', 'Rainfall_Pentolina' for a possible multivariate analysis but my main focus here is univariate analysis which consist of 'Date', 'Depth_to_Groundwater_Podere_Casetta'.

<p align="center">
    <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/Missing_by_year.png" alt="Patterns of Missing Variables by year">
</p>

### Univariate Imputation
#### Missing Values Gaps In Time Series
Even after subsetting the original data, it is still not perfect. The graph below shows the gaps in the data. The red bars are the gaps.

<p align="center">
    <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/Missing_values_ts.png" alt="Gaps of Missing Values in Time Series" height=400>
</p>

#### Imputation
To perform time series analysis, you'll need regular data. As such, I decided to impute the missing values using the following methods and the graphs aftewards showed how well the imputation fits. From the chart below, seasonal decomposition imputation presented the best fit compared to other methods.

- NOCB: next observation carried backward, fill na with next observation
- Mean: fill na with mean
- Exponential: fill na by using exponential weighted moving average
- Linear: impute na by using linear interpolation
- Stine: impute na by using Stineman interpolation
- Seadec: impute missing values using seasonal decomposition

<img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/imp_nocb.png" width="400"/> <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/imp_mean.png" width="400"/>
<img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/imp_ewma.png" width="400"/> <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/imp_linear.png" width="400"/>
<img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/imp_stineman.png" width="400"/> <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/imp_seadec.png" width="400"/>

## Exploratory Analysis
### Correlation Matrix
Here's the correlation matrix for the variables that I've chosen. Even though I am not doing the multivariate analysis, it is interesting to see that Temperature Monteroni is hightly correlated with Temperature of Pentolina while Rainfall at Montalcinello is highly correlated with rainfull of Siminnano and Sovicelle. 

<p align="center">
    <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/correlation_plot.png" alt="Correlation plot for variables">
</p>

### Time Series Plot
Here's how the time series look like after the imputation.

<p align="center">
    <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/Time_plot.png" alt="Time Series Plot" height=400>
</p>

### Seasonality Plot
Here's a run-down of the series by year. In each year, there seems to be a gradual increase from Q1 to Q2 before dropping. Then, around Q3 it climbed slowly towards the end of the year.

<p align="center">
    <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/Seasonal_plot.png" alt="Seasonal Plot">
</p>

## Fitting Models And Forecasting
[Back to top](#table-of-content)

In order to train and select the models, I've split the time series into training and test data. In contrast to the conventional machine learning challenges, you can't randomly subset the data because there is a chronology element to the data. The training data starts from 2008-01-01 and ends at 2016-12-31. The test data starts from 2017-01-01 onwards. 5 models were used because of the seasonality components:

- Naive seasonal forecast
- Seasonal arima (Sarima)
- Exponential Smoothing
- Seasonal decomposition + Arima on seasonally adjusted data
- Seasonal decomposition + Exponential Smoothing on seasonally adjusted data

### Accuracy of Models
The forecasts from the 5 models were then compared against the test data for accuracy. The table below shows that Exponential Smoothing has the lowest root mean square error (RMSE) and better accuracy in general but we'll see that the plot shows otherwise.

<p align="center">
    <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/accuracy_table.png" alt="Accuracy for the 5 models">
</p>

### Forecast Plot
From the forecast plot, we could see that even Exponential Smoothing gave the lowest RMSE in general, it has just predicted the mean. Snaive had basically predicted the same pattern from one season ago. Seasonal arima had the next best scores in terms of accuracy and we could see that for the first year, the prediction was quite close of the actual values but in 2018, there was a sharp increase from the start. Even though Sarima's prediction for 2018 was off by a bit, it had generally preserved the pattern.

<p align="center">
    <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/Forecast_plot.png" alt="Forecast from the 5 models">
</p>

### Diagnostics of Seasonal Arima 
Let's look at the diagnostics of Arima. Here, the best model identified using `auto.arima` which employed AICc to identify the best model revealed that the best fit is Arima(3,1,0)(0,1,0)[365]. The Ljung-Box test showed that there is still autocorrelation in the residuals (p < 0.05). This is echoed in ACF of the residuals. Looking at the residual plot, there seem to be some sudden increase in flanking 2012. Maybe a model capturing the changing variance might be useful.

<p align="center">
    <img src="https://github.com/hannz88/Time_Series_Analysis_Luco_Aquifer/blob/main/Images/sarima_diagnostics.png" alt="Diagnostics of the Sarima model">
</p>

## Conclusion
[Back to top](#table-of-content)

There appears to be a seasonal component in the depth to underground water in Luco Aquifer. The level seems to rise during early quarter of the year before falling only to gradually climb again from Q3. The best model we get using the daily data is Arima(3,1,0)(0,1,0). It is capable of accurately predicting the depth in 2017 but the prediction is would be off by 2018. Looking at accuracy itself is not enough. It is imperative to plot the predictions to understand if the forecast is reasonable. A model capturing the changing variance like G-ARCH might be useful. However, given that the water level is more likely to be contributed by other water bodies, Vector Autoregression (VAR) of other endogenous input could be useful, too.

*[Source of the clock image for the badge](https://www.flaticon.com/free-icon/chronometer_850960?term=time&page=1&position=6&page=1&position=6&related_id=850960&origin=search)
