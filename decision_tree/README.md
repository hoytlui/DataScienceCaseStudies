# Objective
- Use decision tree to determine whether the factors such as age, gender, salary, money spent on RR Diner Coffee last week and the preceding month, 
coffee bags bought last year, online purchase, and their distance from the flagship store (as it would affect the shipping charges)
could predict their purchase of the new coffee beans from Hidden Farm


#### Analysis:
Through data cleaning and visualization, we found that
- 75% of the customers who spent less than $32 last week decided not to purchase
- 75% of the customers who spent more than $34 last week decided to purchase
![2 spent_last_week vs decision](https://user-images.githubusercontent.com/36130927/121100821-96a95b00-c7c8-11eb-90d7-2ca42a370800.png)


- customers who live further away from the flagship store did not spend more enough decide not to purchase
- customers who live close to the flagship store tend to decide to purchase with small amount of purchase last month
![3 spent_last_month vs distance](https://user-images.githubusercontent.com/36130927/121100833-9a3ce200-c7c8-11eb-86b6-e2ee578ffb7a.png)


Predict Decision


Modeling - 4 models
1. Entropy model with no max depth

![4 dt entropy1](https://user-images.githubusercontent.com/36130927/121100846-a4f77700-c7c8-11eb-9bbb-b9df100f1f4c.png)


2. Gini model with no max depth

![5 dt gini1](https://user-images.githubusercontent.com/36130927/121100851-a7f26780-c7c8-11eb-822d-0f2e0b27d1e3.png)


3. Entropy model with 3 levels of max depth

![6 dt entropy2](https://user-images.githubusercontent.com/36130927/121100854-ac1e8500-c7c8-11eb-965e-a3ec12bdfb8b.png)


4. Gini model with 3 levels of max depth

![7 dt gini2](https://user-images.githubusercontent.com/36130927/121100859-ae80df00-c7c8-11eb-872e-00c40a96c9b5.png)



Evaluation
We evaluated the models on their accuracy, precision and recall scores.
Entropy model returns the best scores in all 3 metrics, 99.2%, 98.7%, 97.6%, respectively.
However, without capping the max depth, the original entropy and gini models went as many as 5 and 6 levels, respectively, which tends to overfit the data.

To make it optimal, the max depth is capped at 3 levels.
Gini model returned the most elegant solution, at 97.5% accuracy, 97.5% precision, and 95.1% recall score.
It is also of less computational expensive because of the nature that it is not using log function in its algorithm.


Random Forest
We also tried random forest to give us a more consistent result by averaging results from different trees, leading to less randomness.
Theoretically speaking, random forest would improve predictive accuracy and control over-fitting compared to decision tree.

#### Conclusion:
To source coffee beans from the new farm, we initially set our expected rate of purchase to be 70% from our customers.
After training few models, our best result is 69.8% of people predicted to make the purchase from the new farm.
The result is close to our cut-off point. However, it is not a firm break or deal answer based on our prediction.
We also need to consider the risk level we want to take, the opportunity cost and the consequences of our decisions, and how the farmer strikes will affect our business if it happens.

#### Further work:
From the model standpoint, we can further find the optimal model through tuning hyperparameters.
We can also graph the error curve on training and test data to find the optimal max depth.


#### Skills used:
Python, data cleaning, data visualization, predictive modeling


#### Libraries:
scikit-learn, numpy, pandas, matplotlib, seaborn
