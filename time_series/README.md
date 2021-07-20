# Objective
- To predict Cowboy Cigarettes sales using the ARIMA model


### Analysis:
After cleaning the data, we break down time series into trend, seasonality and noise components.

![1 seasonality decomp](https://user-images.githubusercontent.com/36130927/126249517-af3bbb6e-cae6-496d-99b8-2a877999d14f.png)

We test its stationarity with KPSS test.

![2 sales](https://user-images.githubusercontent.com/36130927/126249545-ae6f72c0-f5c8-4b71-b9f0-0537062cbee5.png)

We see both the mean and variance increase as time progresses. To make the variance constant, we log transform the time series, as shown below.

![3 log of sales](https://user-images.githubusercontent.com/36130927/126249560-95e092e9-526c-4202-a887-80b04fd34c9d.png)

Then we use differencing to make the mean constant prior to building the ARIMA model. And here's the result.

![4 arima](https://user-images.githubusercontent.com/36130927/126249571-0dc87b26-7cf2-46f3-b450-94263d9802ea.png)

We plot the original vs predicted trends, and clearly we see seasonality still exists.
But the prediction captures the variance.

![5 original vs predicted](https://user-images.githubusercontent.com/36130927/126249602-d032e661-21c4-4b0a-b90e-d48a9e5d88f5.png)

The trend prediction is shown below.

![6 trend prediction](https://user-images.githubusercontent.com/36130927/126249578-2579e0b3-da17-4f4c-9df6-e277364f6bed.png)


### Conclusion:
- The trend is increasing in general. Cigarettes are sold more in summer and less in winter. Perhaps due to the good weather in summer for a more relaxing outdoor activities lifestyle.
- This ARIMA model has done well in the univariate time series analysis.


### Further work:
We can execute a regression analysis on top of the time series analysis to discover the causes of the sales trajectory


### Skills used:
Python, data cleaning, data visualization, predictive modeling, time series analysis


### Libraries:
numpy, pandas, matplotlib
