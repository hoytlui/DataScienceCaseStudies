# Objective
- Apply cosine similarity to compare text values and measure how the tested documents are similar to each other



#### Analysis:

To compare documents, we first combine the documents into a corpus.
Then we count vectorizer to the corpus to transform it into vectors using `CountVectorizer()` from scikit-learn.

![1 vectorizer](https://user-images.githubusercontent.com/36130927/121612203-e8035580-ca27-11eb-9273-dd7cf4eb7eb7.png)


Next, we output the counts onto a dataframe before applying TF-IDF to convert the vectors to unique frequency measures using `TfidfVectorizer()`.

Finally, we measure the similarity for the compared documents with `cosine_similarity`.

Here, we compared the following paragraphs/documents.
"Starbucks Coffee" and "Essence of Coffee" returns a 26.1% similarity.

![2 cosine similarity coffee](https://user-images.githubusercontent.com/36130927/121612216-eb96dc80-ca27-11eb-967b-d999ef1036fd.png)


An apple article from Healthline and "An apple a day keeps the doctor away" returns a 8.8% similarity.

![3 cosine similarity apple](https://user-images.githubusercontent.com/36130927/121612218-edf93680-ca27-11eb-9a45-711b510c6f5c.png)


#### Conclusion:
- Cosine similarity can be used in recommender system, search query, and many other use cases.



#### Further work:
- Effectively apply cosine similarity in other projects


#### Skills used:
Python, data cleaning, data visualization, predictive modeling


#### Libraries:
scikit-learn, scipy, numpy, pandas, matplotlib
