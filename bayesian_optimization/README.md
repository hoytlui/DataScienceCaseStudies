# Objective
- Optimize hyperparameters with Bayesian optimization



### Analysis:
Bayesian optimization applies Gaussian process that best describe the function to optimize.
The graph below shows observation points, prediction and target lines, and 95% confidence interval for a 9-step function.

![1 gaussian process](https://user-images.githubusercontent.com/36130927/126240803-c8da2a33-0297-4879-ba31-2e93498504e6.png)


In this project, we will predict if a flight departure is going to be delayed by 15 minutes.
We will use LightGBM and Bayesian optimization to optimize our prediction accuracy.


After defining our features (both numerical and categorical), we split the data into training and test sets.
Then we define the parameters used in our LightGBM model along with the cross validation metrics.


![2 light gbm bayesian optimization](https://user-images.githubusercontent.com/36130927/126240537-58396c1f-d5be-469d-9111-eba3cd457116.png)


Our goal is to get the target value (or accuracy) as close to 1 as possible.
We see it happen at the 5th iteration, where the target is 0.7436.


### Conclusion:
Bayesian optimization is a powerful algorithm to provide insights in a black-box model, in which the parameters are identified to produce the optimal target value.


### Further work:
We can further explore the combinations of the hyperparameters to obtain a possibly higher accuracy score.
Or, we can apply Bayesian optimization in different models or different datasets.

### Skills used:
Python, feature engineering, predictive modeling


### Libraries:
scikit-learn, lightgbm, bayes_opt, numpy, pandas
