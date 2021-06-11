# Objective
- Apply cosine similarity to compare text values and measure how the tested documents are similar to each other.



#### Analysis:

To compare documents, we first combine the documents into a corpus.
Then we count vectorizer to the corpus to transform it into vectors using `CountVectorizer()` from scikit-learn.



Next, we output the counts onto a dataframe before applying TF-IDF to convert the vectors to unique frequency measures using `TfidfVectorizer()`

Finally, we measure the similarity for the compared documents with `cosine_similarity`

Here, we compared the following paragraphs/documents.
"Starbucks Coffee" and "Essence of Coffee" returns a 26.1% similarity


An apple article from Healthline and "An apple a day keeps the doctor away" returns a 8.8% similarity



#### Conclusion:
- Cosine similarity can be used in recommender system, search query, and many other use cases.



#### Further work:
- Effectively apply cosine similarity in other projects


#### Skills used:
Python, data cleaning, data visualization, predictive modeling


#### Libraries:
scikit-learn, scipy, numpy, pandas, matplotlib
