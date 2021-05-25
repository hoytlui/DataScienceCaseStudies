# Objective
Apply frequentist inference and Central Limit Theorem on theoretical and real-world problems
Frame null and alternative hypotheses
Get familiar with using t-test

#### Analysis:
As stated in the Central Limit Theorem, the graph aligns with the theory that as sample size increases, sampling distributions become narrower.

![frequentist_inference1](https://user-images.githubusercontent.com/36130927/119580024-a74fdf00-bd8d-11eb-855f-aef06b12ab2e.png)

In standard normal distribution, the probability covered in 1 SD, 2 SD, and 3 SD are 68%, 95%, and 99.7%, respectively.
The graph shown below shows the probablity of 1 SD or less from the mean is 50% + 68%/2 = 84%.

![frequentist_inference2](https://user-images.githubusercontent.com/36130927/119580061-b46cce00-bd8d-11eb-843f-2661d980793b.png)

One-tailed test is used when we want to find out whether the value is below (or above) a critical value.
In this case, whether the actual charge has fallen below 12,000.

![frequentist_inference3](https://user-images.githubusercontent.com/36130927/119579999-9a32f000-bd8d-11eb-9cd5-d7edebc5274e.png)


#### Conclusion:
When performing exploratory data analysis (EDA), we need to think ahead before actually delving in finding the statistics.
- Do we know the population standard deviation?
- How big is the sample?
- Do we use t-test or z-test?
- What are the hypotheses in quest?
- One-tailed or two-tailed test?
- What is the comfortable confidence interval?

After working on the statistics part, we reflect few things.
- What do the numbers tell?
- Was the right test used?
- Which part might have done differently?

Forming a (right) conclusion can be difficult as it can be subjective, particularly on changing the confidence interval. Therefore, always think ahead.


#### Further work:
Plot ppf and cdf to further explain the difference between t-test and z-test


#### Skills used:
Python, statistics


#### Libraries:
numpy, pandas, scipy, matplotlib

