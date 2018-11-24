# K.AI--Take-home

<h3>Solution:</h2>

Unsupervised models used for generating word vectors: Word2vec and Tf-IDF

Clusters identified from the Bank chatbot conversation data:
  
<li>Loan requirement questions</li>
<li>Asking the bot to clear bills</li>
<li>Outstanding balance-check questions</li>
<li>Money Transfer queries</li>
<li>FAQs</li>

The Inference for all approaches is mentioned at the bottom of the repective ipynb files


##TF-IDF with K-means pipeline :

Data -> Delete duplicates -> vectorization with stop words, stemming and tokenization -> Creation of Elbow plot -> identifying clusters -> PLotting clusters using different dimentionality reduction and visualization techniques -> Grouping words by their respective clusters -> Inference



Tf-idf
Inference:
The elbow curve tells us that the optimal number of clusters are 5,6 or 7. When we go through the word groupings we understand that the data is talking about the following queries

1.Loan requirement questions
2.Asking the bot to clear bills
3.Outstanding balance check questions
4.Money Transfer queries
5.FAQs

According to the TF-IDF word embedding technique which we just used, these five groups of data are classified in 6 clusters, since there is a significant amount of noise in the dataset and because TF-Idf is essentially a scoring algorithm which creates a score for every word based on their occurences and non occurences. The distribution of these scores, given theor weights creates a slight bias for the noisy data as well. This is vizualized in the various plots we have.

Although, the ideal number of cluster remain at 5

w2v
Inference:
The elbow curve tells us that the optimal number of clusters are 4,5. Plotting these cluster values shows us a clear distiction in the intents. Visualization from the Word2Vec model shows us how the model is more capable of differtiating between noisy data points, due to its nature of creating contexts based on their semantic meanings.

The word2vec technique combined with the TF-IDF word embedding technique, provides a clear conclusion to the number of intents and clusters we have in our data. It solidifies our understnading of the clusters(5) and their names, which are

1.Loan requirement questions
2.Asking the bot to clear bills
3.Outstanding balance check questions
4.Money Transfer queries
5.FAQs

​
