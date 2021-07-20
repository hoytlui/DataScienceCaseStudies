# Objective
- Predict future user adoption with different variables



### Analysis:
After cleaning the data, the following graphs summarize our findings.

![1 heatmap](https://user-images.githubusercontent.com/36130927/126266956-9a019413-5625-428a-9011-1ab287174c87.png)

No features seem to be correlated with the target variable.
The two most correlated variables are the organization the users belong to (org_id) and user joining invitation (invited_by_user_id),
yet none of them has a correlation of higher than 0.1.

![2 classification report](https://user-images.githubusercontent.com/36130927/126267086-815dda68-c8f6-4f3b-9412-a806acf82574.png)

Random forest model generates an accuracy of 79% weighted F-1 score to predict whether the user is adopted or not.

![3 confusion matrix](https://user-images.githubusercontent.com/36130927/126267859-c82db94c-b6a1-440e-ab9c-02fc45310a94.png)

However, we have to be aware that the data is imbalanced.
The model predicted more than 99% negative, and more than 85% of them are correctly predicted. It is because most customers are not adopted users.
It seems that the model does not have a high predictive power.

![4 feature importance](https://user-images.githubusercontent.com/36130927/126267088-8a664c30-9a00-4fd8-9f31-9b276f38aa0f.png)

The two most important features for the model are the organization the users belong to (org_id) and user joining invitation (invited_by_user_id).


### Conclusion:
Since the data is imbalanced, the model prediction most likely will be lenient towards the majority class.
One of the ways to improve data quality is to either downsample the majority class, or upsample the minority class.
But keep in mind that downsampling may cause info loss, while upsampling may result in overfitting.


### Further work:
Collect more data or feature engineer to create new variables


### Skills used:
Python, data cleaning, data visualization, predictive modeling


### Libraries:
scikit-learn, numpy, pandas, matplotlib, seaborn
