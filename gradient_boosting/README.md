# Objective
- Build a gradient boosting algorithm to predict survival rate in the classic Kaggle Titanic competition



#### Analysis:
After a quick and dirty data cleaning process, we fit the data into a gradient boosting model.
In the gradient boosting classifier, we tuned hyperparameters by testing multiple learning rates and finding the best rate.
Then we fit the model and predicted on the test set.
The confusion matrix, classification report and ROC curve evaluate high accuracy of the model.




#### Conclusion:
Gradient boosting sequentially reduces residual errors of the previous prediction through iterations.
In most cases, it generates a better predictions compared to the bagging method, where individual data is trained in a parallel way.



#### Further work:
The Titanic dataset is relatively small, which does not take too much time for gradient boosting model for prediction.
In case of predicting a large data file, we can compare other models like random forest and AdaBoost and find which model is the most efficient to use.


#### Skills used:
Python, data cleaning, data visualization, predictive modeling


#### Libraries:
scikit-learn, scipy, numpy, pandas, matplotlib
