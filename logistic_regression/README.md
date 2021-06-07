# Objective
- Understand the mechanics behind logistic regression with the help of hyperparameter tuning and grid search

#### Analysis:
Use logistic regression to predict gender using the weight and height features

![plot1](https://user-images.githubusercontent.com/36130927/121052056-00554500-c788-11eb-9326-bf9b2fb76adf.png)


Base model (with cross-validation) accuracy: 0.9172


Hyperparameter turning

Regularization parameter ***C*** controls for unlikely high regression coefficients or for feature selection.
We tuned ***C*** with 0.001, 0.1, 1, 10, and 100, and we found that the highest average score on training data is 0.9172 at C = 0.1.
We then used the best parameter of C = 0.1 on test data and predicted with an accuracy score of 0.9252.


Now, using Grid Search, we found that the best accuracy is 0.9252 at C = 1

***C*** is the regularization strength, the smaller the ***C***, the stronger the regularization,
in which it tries to prevent features from having terribly high weights,
thus implementing a form of feature selection


The figure below shows that the logistic regression with the best parameters returns a 92.52% accuracy.
Red is Female, blue is Male.
Circle is training data, square is test data.
Grid boundary is split into red and blue, which is the maximum classifier separating the predicted labels.

![plot2](https://user-images.githubusercontent.com/36130927/121052093-0814e980-c788-11eb-890d-f719e4b255d8.png)



#### Conclusion:
Logistc regression is a type of classification which uses the sigmoid function to separate values into 1 and 0.
This is particularly helpful if the underlying data can be discretely and clearly defined.
Hyperparameter tuning can further improve the model accuracy.

#### Further work:
- Explore other algorithm that can perform better than logistic regression in other situation.


#### Skills used:
Python


#### Libraries:
scikit-learn, scipy, numpy, pandas, matplotlib, seaborn
