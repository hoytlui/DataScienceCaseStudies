# Objective
- To tell a story through exploratory data analysis



### Analysis:
In this project, we will analyze adult income in the U.S.
This dataset was contributed a long time ago in 1996, but it still serves the purpose of storytelling.
Let's see what we have found here.

After a quick data cleaning and understanding, we want to craft the story in 4 aspects:
- Gender, race and working hours
- Occupation
- Relationship and marital status
- Age and education (levels and years)

We want to find out if any of the above aspects will have an impact on the surveyer's underlying annual income, which only has two outcomes: > $50K or <= $50K

![1 gender vs income](https://user-images.githubusercontent.com/36130927/126243738-673501f1-aad8-4efa-8df8-f7d21317bc00.png)

In general, 90% of the female, while only 70% of male, earned below $50K annual salary. Why is that? Does sex discrimination truly exist?

![2 working hours vs income](https://user-images.githubusercontent.com/36130927/126243740-07159531-9215-4b63-9fbd-92d33316249d.png)

Let's have a general idea first. We should agree that people working more hours tend to earn more.

![3 working hours and gender vs income](https://user-images.githubusercontent.com/36130927/126243741-7776542e-3d76-4b66-96b2-522c2af4a34c.png)

We can tell that people who earn more than $50K tend to work longer hours, with an exception of male who work more than 40 hours but earn less.
But at least this graph tells us the reason that female earning less may be due to less working hours rather than sex discrimination.

![4 race](https://user-images.githubusercontent.com/36130927/126243742-df3a5480-9b5c-4430-8c0c-18b3e374eb0f.png)

From the above graph, White and Asian-Pacific-Islander people tend to earn more than $50K a year. We will explore in further below.

![5 gender and race vs income](https://user-images.githubusercontent.com/36130927/126243744-71bf3fd5-17cd-478f-b49e-ed84500263ea.png)

It seems to be particularly true for White male and Asian male who have a significantly higher probability of earning more than $50K compared to their female races. We can also tell that Black male tends to earn a lot more than Black female, which drags down the probabilty of earning in the upper end for the Black race. Male earns more due to higher working hours has been explained in the second graph from above. But does the phenomenon differ from race to race?

![6 gender and race vs working hours](https://user-images.githubusercontent.com/36130927/126243746-cdf10ad1-f906-4e2f-b12d-f168b2ea4cee.png)

From the above graph, we can tell majority of male works longer hours than majority of female. This is true across 3 races, White, Asian-Pacific-Islander, and American-Indian-Eskimo. This leads to a clearer picture of why White and Asian male earn more than their female race and also more than the other races in general.
However, it is also true that American-Indian-Eskimo male may be underpaid. For the long working hours they provide, they should have similar probability of earning above $50K. But instead, they have the lowest probability of earning in the upper end across all races.

![7 native country vs income](https://user-images.githubusercontent.com/36130927/126243747-56c5613f-2bbb-4a11-8b6b-9c80601ec721.png)

People from France, India, or Taiwan tend to have a higher probability (~40%) of earning above $50K, highest among all native countries.

![8 workclass vs income](https://user-images.githubusercontent.com/36130927/126243749-89ee1549-d1f7-4808-93df-b62005bffac0.png)

Self-employed by an incorporated firm, the only workclass having a higher-than-50%-chance, compiles a 55% chance of earning above $50K.

![9 occupation vs income](https://user-images.githubusercontent.com/36130927/126248407-dedcadd0-f9f8-4f31-a4a4-79db36a7fc20.png)

The two most highest paid occupations are the executive managerial roles and roles in professional speciality. On the other hand, the least paid occupations are private house service, other service and handlers and cleaners.

![10 occupation and working hours vs income](https://user-images.githubusercontent.com/36130927/126243751-680fb4ee-f47f-447a-9f2e-b6c77f5cbbd5.png)

The above graph further indicates that different occupations will result in different income range. People in executive managerial type of roles or in professional specialty who work more than 40 hours most likely will earn more than $50K. However, for the same amount of working hours, those working in private house services, other services, handlers/cleaners, and farming/fishing almost guarantee to remain under $50K in salary.

![11 relationship vs income](https://user-images.githubusercontent.com/36130927/126243753-d27a3358-c256-44dc-ad99-3684bfa01267.png)

Husbands and wives have a close equality of earning power. In fact, a higher proportion of wives earns more than $50K than that of husbands.

![12 realtionship and working hours vs income](https://user-images.githubusercontent.com/36130927/126243754-fb58ba71-f1aa-44cd-ab51-460c1080b894.png)

![13 relationship and working hours vs income](https://user-images.githubusercontent.com/36130927/126243756-40ac7d79-ff02-435c-9f99-6ec932e3af76.png)

There are two interesting fact in the above 2 graphs in different presentation:
A significant portion of wives earn above $50K while working less than the median of 40 hours per week.
Husbands tend to work more than wives in general.

![14 marital status and working hours vs income](https://user-images.githubusercontent.com/36130927/126248032-6c99a75a-afe4-45a7-8e56-ac15a78b7ef4.png)

Two more interesting findings in this graph.
People who are never married, widowed, or married to an armed forces spouse earn less than $50K with less working hours.
Higher earning power from the people who are never married, divorced, or married to a spouse not living in the same household are the ones who do not mind working longer hours, meaning they would put more time into work with an absence of relationship.

![15 age vs income](https://user-images.githubusercontent.com/36130927/126243759-fb1c4939-d3e1-4bcf-99e0-ff55a7fd8d46.png)

The younger the age, the higher the probability that the person will earn less than $50K, especially those younger than late-30s. Why is that?

![16 education level and years vs income](https://user-images.githubusercontent.com/36130927/126243760-e005ec94-2a3b-4c3c-a43e-fa382ae7e129.png)

It seems that people are more common to earn more than $50K with 13 years or more of education.

![17 age and education years vs income](https://user-images.githubusercontent.com/36130927/126243761-626854f7-fcfd-42c3-a033-5921b1baead6.png)

This graph shows us that income earned is more correlated to number of years of education than age. Those who has 13 years or more in education tend to earn more than $50K, regardless of their age.



### Conclusion:
We have looked at earning power from four different perspectives.
- Gender, race, and working hours. Sex discrimination does not firmly exist. People who earn more are the ones who work longer hours.
- Occupation. If you want to have a higher chance of being rich, either be self-employed by an incorporated firm, as work as an executive managerial role or in professional specialty.
- Relationship and marital status. In a family, husbands tend to work longer than wives. However, that does not define the earning power of wives because they are equally capable of earning more than $50K with less working hours. Those who are not in relationship may work longer hours, which results in higher earning power.
- Age and education. Earning power is positively correlated with years of education.


### Further work:
Try other creative plots to give additional insights to the existing story


### Skills used:
Python, data cleaning, data visualization


### Libraries:
numpy, pandas, matplotlib, seaborn
