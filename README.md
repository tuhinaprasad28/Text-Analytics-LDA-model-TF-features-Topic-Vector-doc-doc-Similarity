# Text-Analytics-LDA-model-TF-features-Topic-Vector-doc-doc-Similarity

Task 1:

Preprocess the given 4 articles to get their tf features. Then fit LDA model with the tf features. Use 10 as the number of topics (K=10). The number of features should be the number of unique words in all the articles. It depends on what kind of preprocesses you will apply on the original text (remove stop words, tokenization, stemming etc.). 

After the preprocessing, you should get a matrix as below to fit into LDA model:

TF of word1	TF of word2	TF of word3	…	…	…	…	…	TF of word n

D1	10	36	43	…	…	…	…	…	1

D2	5	7	2	…	…	…	…	…	19

D3	43	0	8	…	…	…	…	…	6

D4	2	28	0	…	…	…	…	…	0

After fitting the LDA, extract and print out the top 10 words of each topic, similar to the output in page 44 of “Text Clustering” lecture slide. 


Output: (.txt)
Topic 1:   rank1 word, rank2 word, …. rank10 word
…
Topic 10: rank1 word, rank2 word, …. rank10 word


Task 2:

Extract the topic vector (topic probability distribution for a document) of each document and calculate doc-doc similarity using Cosine similarity for every pair of articles (6 pairs in total). Print out the similarity in ascending order:

The topic vector will be like below:

Probability of Topic 1	Probability of Topic 2	Probability of Topic 3	…	…	Probability of Topic 10

D1	0.12	0.32	0.56	…	…	0.003

D2	0.6	0.017	0.223	…	…	0.01

D3	0.021	0.0007	0.19	…	…	0.78

D4	0.009	0.33	0.02	…	…	0.029


Output : (.txt)
Article 1 and 2 similarity:  a float number
…..
Article 3 and 4 similarity:   a float number
