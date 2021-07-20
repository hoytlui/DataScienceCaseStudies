# Objective
- Build classification models (logistic regression, gradient boosting, random forest) in Spark environment
- Perform machine learning pipeline in Spark environment, including EDA, one hot encoding, train/test split, modeling, evaluating, cross validation, hyperparameters tuning, and feature importance


### Analysis:
The Spark environment is very capable of doing machine learning

We can write SQL queries

![1 spark sql](https://user-images.githubusercontent.com/36130927/126260395-4f1392a1-0fe2-4504-9606-892d63aa7c9b.png)

We can analyze with spark dataframe

![4 spark dataframe operations](https://user-images.githubusercontent.com/36130927/126260439-53a2b92c-c93e-4abd-9180-3a5ac5813874.png)

It's integrated with pandas

![5 pandas](https://user-images.githubusercontent.com/36130927/126260473-89f6459e-e864-4955-93b3-5d6dca681166.png)

We can explore data by visualizing graphs with matplotlib

![6 matplotlib](https://user-images.githubusercontent.com/36130927/126260485-b7d7d8c5-72cc-4f0e-9b57-4bc58db855c9.png)

Here's what Spark is amazing. We can run machine learning pipeline in the environment.

One hot encoding

![7 spark ml pipeline one hot encoding](https://user-images.githubusercontent.com/36130927/126260599-a99f7869-9e15-40cc-b7b8-507278fef595.png)

Train/test split

![8 train test split](https://user-images.githubusercontent.com/36130927/126260605-76dbb1de-1272-4690-abb4-3dfa404a9732.png)

Modeling and predicting

Logistic regression

![9 log reg](https://user-images.githubusercontent.com/36130927/126260629-a69d61d4-cae3-4a31-883e-35398928ec51.png)

Gradient boosting

![10 gbm](https://user-images.githubusercontent.com/36130927/126260633-60925ddf-1598-4436-8cf2-254cd73d157a.png)

Then transform and predict the outcome

![11 log reg transform predict](https://user-images.githubusercontent.com/36130927/126260749-4241979e-f2c5-4fc7-ab8d-8b5ace717a40.png)


And evaluate

![13 log reg evaluate](https://user-images.githubusercontent.com/36130927/126260799-b16032d0-051e-4ad4-ac90-f088a9b52c71.png)


We can also perform cross validation amd hyperparameters tuning and find the best parameters

![15 log reg param grid](https://user-images.githubusercontent.com/36130927/126260848-690a13b6-1222-4c18-a120-0831ba8c127d.png)

![17 log reg cv](https://user-images.githubusercontent.com/36130927/126260852-692660d7-ad39-4b1f-9ade-f85c07aa8e2a.png)

![18 log reg best params](https://user-images.githubusercontent.com/36130927/126260894-cbd90e3a-7293-4eed-a5d7-e998cd7f70a5.png)

Then modeling and predicting again on the cross validated model

![21 log reg cv predict](https://user-images.githubusercontent.com/36130927/126260918-6ded8501-1c3e-42e4-b9a5-9a025c047830.png)

![23 log reg cv evaluate](https://user-images.githubusercontent.com/36130927/126260944-d403b1d9-e148-430c-b7f6-1229b28eea76.png)

Last but not least, we can compute the feature weight and the feature importance

![25 log reg feature weight](https://user-images.githubusercontent.com/36130927/126261006-2475af2b-c60d-43ba-8a84-f494f67441cf.png)

![27 gbm cv feature importance](https://user-images.githubusercontent.com/36130927/126261019-224a5337-a99a-4441-85e8-785c145baca7.png)


### Conclusion:
- Spark is where SQL meets machine learning
- We can perform standard machine learning workflow capably in the Spark environment


### Further work:
Explore other models in Spark


### Skills used:
Python, SQL, Spark, predictive modeling


### Libraries:
pyspark, itertools, pandas, matplotlib
