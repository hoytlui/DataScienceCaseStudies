# Objective
- Implement linear regression, specifically ordinary least squares regression (OLS), and statistical models to evaluate relationships of variables in the red wine dataset
- Build predictive model to predict acidity of red wine
- Identify situations of using classification and regression

#### Analysis:
To predict the quality of wine would be ideal, but its discrete type is only suitable for classification analysis.
While all other variables are continuous, regression analysis is subsequently performed.

The pairplot below confirms that the horizontal bands of quality was caused by its discrete feature.
![2 pairplot](https://user-images.githubusercontent.com/36130927/120146263-cf3aaa80-c1b2-11eb-8ca4-7bbe41883a3a.png)


Fixed acidity is an interesting factor, and will be used for the regression analysis.
The correlation heatmap shows that density and fixed acidity have high correlation.
![3 correlation heatmap](https://user-images.githubusercontent.com/36130927/120146289-dd88c680-c1b2-11eb-9c70-709e6997b033.png)


Scatter plot and line of best fit also suggests a linear regression between these two variables.
![5 fixed acidity vs density with line of best fit](https://user-images.githubusercontent.com/36130927/120146310-e4173e00-c1b2-11eb-8948-eb44399caf49.png)



Let's model it with a 0.75/0.25 train/test split.


Linear regression model 1 - base model

![6 model1](https://user-images.githubusercontent.com/36130927/120146325-e9748880-c1b2-11eb-8d4a-4af9bba3613c.png)

Linear regression model shows the positive correlation. But there are lots of noises in the graph. R-squared is 0.447.


Linear regression model 2 - OLS, adding a constant

![7 model2](https://user-images.githubusercontent.com/36130927/120146354-f2655a00-c1b2-11eb-97a2-18e944ce23a1.png)

Adding a constant to OLS seems to have less variance than the base model, but R-squared is the same at 0.447.


Linear regression model 3 - multiple linear regression

![8 model3](https://user-images.githubusercontent.com/36130927/120146382-fb562b80-c1b2-11eb-84ef-76895e81eff2.png)

Using multiple variables on top of model 2 gives a much higher R-squared of 0.877.


Linear regression model 4 - multiple linear regression less positively correlated explantory variables

![9 model4](https://user-images.githubusercontent.com/36130927/120146655-6869c100-c1b3-11eb-948e-fc21c551e3f4.png)

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
