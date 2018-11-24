# K.AI--Take-home
Problem statement: With the enclosed data, cluster the utterances using unsupervised learning techniques and explain the reasons for choice of algorithms you use. Assume there is noise in data. Identify important clusters and assign a suitable name to non-noise clusters.


Inference for all approaches is mentioned at the bottom of the repective ipynb files

Tf-idf
Inference:
The elbow curve tells us that the optimal number of clusters are 5,6 or 7. When we go through the word groupings we understand that the data is talking about the following queries

Loan requirement questions
Asking the bot to clear bills
Outstanding balance check questions
Money Transfer queries
FAQs
According to the TF-IDF word embedding technique which we just used, these five groups of data are classified in 6 clusters, since there is a significant amount of noise in the dataset (vizualized in the various plots)

Although, the ideal number of cluster remain at 5

w2v
Inference:
The elbow curve tells us that the optimal number of clusters are 4,5. Plotting these cluster values shows us a clear distiction in the intents. Visualization from the Word2Vec model shows us how the model is more capable of differtiatig between noisy data points.

The word2vec model combined with the TF-IDF word embedding model, provides a clear conclusion to the number of intents and clusters we have in our data. It solidifies our understnading of the clusters(5) and their names which are

Loan requirement questions
Asking the bot to clear bills
Outstanding balance check questions
Money Transfer queries
FAQs

​
