# Objective
- Find out if apps on Google Play Store are ranked higher than those on Apple App Store
- Apply permutation test when data is not normally distributed
- Frame null and alternative hypotheses, then challenge them


#### Analysis:
For simplicity, we used the data on Kaggle. Alternatively, the data can be scraped with iTunes Search API and on Google Play Store.

First, we screened the data to see which columns to keep for the analysis.

Second, we cleaned, transformed and visualized the data.
The boxplot below shows that the mean of rating for Google is indeed higher than that for Apple.



Next, we tested if the data is statistically significant enough to conclude our hypothesis
- Ho: rating of apps has no difference in either platform
- Ha: rating of apps on Google is higher than on Apple
To determine which test to use, we need to find out if the data are normally distributted.


Since the data are not normally distributed, permutation test is applied.
And here's the result of the difference of mean in both platforms' ratings after permutation.

Lastly, we computed the p-value is 0, meaning the null hypothesis of no difference is rejected.


#### Conclusion:
And we concluded that apps being put on Google Play Store do have higher ratings than those being put on Apple App Store.
- How does that impact the developers on their marketing strategies?


#### Further work:
Dig deeper to find out if any genres are given a higher overall ratings
Explore other opportunities for using different kinds of statistical tests


#### Skills used:
Python, data wrangling, statistics


#### Libraries:
numpy, pandas, scipy, matplotlib, seaborn
