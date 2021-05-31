# Objective
- Implement linear regression, specifically ordinary least squares regression (OLS), and statistical models to evaluate relationships of variables in the red wine dataset
- Build predictive model to predict acidity of red wine
- Identify situations of using classification and regression

#### Analysis:
To predict the quality of wine would be ideal, but its discrete type is only suitable for classification analysis.
While all other variables are continuous, regression analysis is subsequently performed.

The pairplot below confirms that the horizontal bands of quality was caused by its discrete feature.
[pic]

Fixed acidity is an interesting factor, and will be used for the regression analysis.
The correlation heatmap shows that density and fixed acidity have high correlation.
[pic]

Scatter plot and line of best fit also suggests a linear regression between these two variables.
[pciture]


Let's model it with a 0.75/0.25 train/test split.


Linear regression model 1 - base model
[pic]
Linear regression model shows the positive correlation. But there are lots of noises in the graph. R-squared is 0.447.


Linear regression model 2 - OLS, adding a constant
[pic]
Adding a constant to OLS seems to have less variance than the base model, but R-squared is the same at 0.447.

Linear regression model 3 - multiple linear regression
[pic]
Using multiple variables on top of model 2 gives a much higher R-squared of 0.877.

Linear regression model 4 - multiple linear regression less positively correlated explantory variables
[pic]
Further dropping more correlated columns avoid the redundancy that may adversely affect the predictive power.
But R-squared shows 0.855, 0.022 less than that of model 3.


To check model accuracy, root mean squared error can be used along with R-squared, although the analysis in this case study was driven by R-squared.


#### Conclusion:
In conclusion, R-squared indicates the most predictively powerful model using multiple linear regression.
However, by removing couple correlated columns, we get a more elegant model just 2% shy of the predictive power of the multiple linear regression.


#### Further work:
- Explore other regression algorithms to further investigate the best relationships for prediction


#### Skills used:
Python, statistical models


#### Libraries:
scikit-learn, statsmodels, numpy, pandas, matplotlib, seaborn
