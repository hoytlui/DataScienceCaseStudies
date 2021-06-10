# Objective
- Build a random forest model to predict whether the COVID-19 patient in South Korea is "released", "isolated", or "deceased"

#### Analysis:
A lot of data was cleaned in the dataset
- age and birth_year were inconsistently input, so we calculated true_age from birth_year, 
then imputed the original values in age to calculate birth_year and dropped age
- replaced missing values in global_num, infection_order, infected_by, and contact_number with their mean values
- replaced missing values in infection_case and city with 'etc', which seems to be the 'unknown' recorded in the dataset
- found that 143 out of 145 patients were sexless at age 0, classified them as 'fetus', the remaining 2 were classified as female, the mode of sex
- filled missing values in state as 'missing'
- dropped symptom_onset_date, confirmed_date, released_date, deceased_date

Did a final check on the number and percentage of the unique values of each column,
statistical range of the dataframe, 
number of the unique values of the object columns,
find the correlation heat map within the features,

![1 heatmap](https://user-images.githubusercontent.com/36130927/121431775-d64a8100-c947-11eb-8611-a1992700c0c8.png)

and plot boxplots to check for outliers, then we are good to go ahead with training the model

![2 boxplot](https://user-images.githubusercontent.com/36130927/121431776-d6e31780-c947-11eb-86a3-2a957893f013.png)


We built a random forest model to predict whether patients with such features will likely be released, isolated, or deceased from COVID.
Once we normalized the data, the confusion matrix showed a high accuracy of the classification.

![4 confusion matrix normalized](https://user-images.githubusercontent.com/36130927/121431782-d77bae00-c947-11eb-9fb5-1c70f1b01288.png)


Random forest model is expected to perform well in a multitude of data situations, where it handles highly correlated features like this case.
It is also efficient to investigate the feature importance with a large dataset.

![5 barh graph](https://user-images.githubusercontent.com/36130927/121431784-d77bae00-c947-11eb-8583-bc294709ee1f.png)



#### Conclusion:
While 0.854 accuracy score and 0.827 F1 score show that random forest model is effective in this case, 
one thing to keep in mind is that the model may be subject to the imbalance class of the dataset.

The state column contains 81% isolated, 14% released, 1% deceased, 4% missing values.
It is easy for the model to predict the correct answer if it guesses isolated every time - 81% correct

![6 df state](https://user-images.githubusercontent.com/36130927/121434650-a309f100-c94b-11eb-8c15-234f38ca4677.png)



#### Further work:
- Collect more data to combat the imbalance problem
- Resample or bootstrap the data
- Penalize models using penalized-SVM or penalized-LDA
- Use other alogorithms to build model
- Splitting should be done before imputing missing values when data is used to "learn", this will avoid data leakage

#### Skills used:
Python, data cleaning, data visualization, predictive modeling


#### Libraries:
scikit-learn, numpy, pandas, matplotlib, seaborn
