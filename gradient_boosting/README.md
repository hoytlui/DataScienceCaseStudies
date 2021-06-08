# Objective
- Build a gradient boosting algorithm to predict survival rate in the classic Kaggle Titanic competition



#### Analysis:
After a quick and dirty data cleaning process, we fit the data into a gradient boosting model.
In the gradient boosting classifier, we tuned hyperparameters by testing multiple learning rates and finding the best rate.
Then we fit the model and predicted on the test set.
The confusion matrix, classification report and ROC curve evaluate high accuracy of the model.

![1 cm training data](https://user-images.githubusercontent.com/36130927/121260444-5b1d9800-c87f-11eb-960d-89550350f9f4.png)


![2 cm test data](https://user-images.githubusercontent.com/36130927/121260460-62dd3c80-c87f-11eb-8fd8-393a7045b022.png)


![3 classification report](https://user-images.githubusercontent.com/36130927/121260470-653f9680-c87f-11eb-8656-a3142b0f941e.png)


![4 roc curve](https://user-images.githubusercontent.com/36130927/121260486-696bb400-c87f-11eb-8261-b4cc264aac62.png)



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
