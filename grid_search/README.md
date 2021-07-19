# Objective
- Optimize hyperparameters with grid search in the modeling steps of KNN and random forest



### Analysis:
In this project, we will predict which patients have diabetes from 8 variables.
They are pregnancies, glucose, blood pressure, skin thickness, insulin, BMI, diabetes pedigree function, and age.

![2 hist after imputation](https://user-images.githubusercontent.com/36130927/126227392-f721911d-b7b5-4e09-8eb5-69605754ddb1.png)



We see that glucose and BMI have the highest correlation with the diabetes outcome.

![3 heatmap](https://user-images.githubusercontent.com/36130927/126227381-60f84faa-1c84-4f07-b283-9583a60481fa.png)



But what is the degree of the nearest neighbors should we define to make the best predictions?
The chart below shows the 8 is the ideal k, which is the closest point between the training and test scores.

![4 train vs test score](https://user-images.githubusercontent.com/36130927/126227370-abe651ac-c8d1-4a53-893e-173ee8528169.png)

![6 classification report](https://user-images.githubusercontent.com/36130927/126227468-f804863f-46da-415d-90cf-af0a5c51c170.png)

An accuracy of 74% is not bad. But can we improve the score?

![7 grid search knn](https://user-images.githubusercontent.com/36130927/126227322-adeaa3b7-54b2-444f-a5f7-961f406165de.png)


If we use grid search to tune the hyperparameter of searching k in range of 1 to 50, we will find that the best score reaches 75.3% at k = 31

![8 grid search knn](https://user-images.githubusercontent.com/36130927/126227309-10385f8f-5501-4d32-9546-4da6d1e2fd59.png)


If we use grid search on random forest model. The result is even better at 77.6% at the optimal level when n estimators = 560.

![9 grid search random forest](https://user-images.githubusercontent.com/36130927/126227278-9f33b47d-7b21-4d8a-b498-fad74c4c2f94.png)



### Conclusion:
By using grid search in the models, we can improve our accuracy through tuning the hyperparameters.
However, we still have to be aware of overfitting despite the existence of cross validation in the grid search process.

### Further work:
To ensure we are not overfitting the model, we can play around with the parameters, or try adding regularization on top to see if the prediction results.


### Skills used:
Python, data cleaning, data visualization, predictive modeling


### Libraries:
scikit-learn, numpy, pandas, matplotlib, seaborn
