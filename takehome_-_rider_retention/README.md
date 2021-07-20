# Objective
- Illustrate import features of demand and daily cycles with EDA 
- Design statistical experiment and metrics
- Predict rider retention

### Analysis:
The highlights of EDA include the following 2 graphs.

![3 boxplot](https://user-images.githubusercontent.com/36130927/126263715-b7c1e0b5-51b2-40dd-b376-516cd8ec8a6a.png)

We found that there is a wide variation between 23:00 and 05:30.
Then we break down the plot into different days.

![4 catplot](https://user-images.githubusercontent.com/36130927/126263717-85319ec9-da8b-40b5-9e67-21e1a7435b17.png)

The plots above tell us 3 important observations:
- Wide range between 23:00 and 05:30 is mainly on weekend trips. It could be due to people requesting a ride home after partying or some other reasons.
- Peak hours show between 10:30 to 13:00 on weekdays. It may be due to workers meeting their clients during this time.
- Friday between 21:30 and 22:30 has a higher variance than any other days, most likely due to people working late or going for drinks on Fridays.

The highlights of predictive modeling include the following 3 graphs.

![6 heatmap](https://user-images.githubusercontent.com/36130927/126263766-818e140e-843f-4725-8873-5778df33ec32.png)

The number of trips the user took in the first 30 days after signing up (trips_30d), whether the user took an Ultimate Black in their first 30 days (ultimate_black_30d), and if they rated the driver (rated_driver) have a higher correlation with whether the user is active or not.

![10 feature importance](https://user-images.githubusercontent.com/36130927/126263767-d06b2a55-ec6a-49f1-b25b-01dec9ec7069.png)

The features importance graph tells us the average distance per trip taken in the first 30 days is actually the most important feature to determine the active user (avg_dist_30d), followed by the percentage of trip occurring during weekdays (weekday_pct), and average rating by drivers (avg_rating_by_driver).

![12 scatterplot](https://user-images.githubusercontent.com/36130927/126263769-5b07d205-3ec6-4add-aaaa-0b4486638424.png)

Most active users tend to use our service during weekdays, so we should find ways to incentivize more drivers servicing in this period.


### Conclusion:
Projects like this truly test your skills in data wrangling, EDA, stats, data preprocessing and modeling.
But what equally important is your analytical abilities or creativity to analyze data in a different way to give new insights that may be overlooked.

### Further work:
- Other models can definitely be explored
- Hyperparameters tuning is also applicable to improve prediction accuracy

### Skills used:
Python, data cleaning, data visualization, predictive modeling, inferential statistics


### Libraries:
scikit-learn, numpy, pandas, matplotlib, seaborn
