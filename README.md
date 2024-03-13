# Sentiment-Analysis-Transformers
NLP Tutorial for Roberta-base fine-tuning in order to perform Sentiment Analysis

Topics: NLP, Embeddings, Transformers Architecture.

*************************
### Goal
The objective of this notebook is to show various techniques with which to perform a sentiment analysis on a dataset containing film reviews, taken from Ibdm, and then to perform sentiment predictions for unlabelled reviews.
After loading and splitting the data, we will proceed in two directions:

- Tf-Idf word embeddings + Naive Bayes/Xgboost

- Transformer Model fine tuning

In the end, we will evaluate the goodness of the models produced by the two strategies and choose the best one.

### Get data to analyze
Data come from Ibdm source. There is a set of labelled data (1: Positive review - 0: Negative review) and there is a set of unlabelled data on which I applied Cluestering techniques.

## Files descriptions
The directory of this homework consists of several files:

1 `Sentiment_Analysis.ipynb`
> This Jupyter notebook file contains the different approaches to the task- We will first look at a solution classically used in NLP, using text classification via classical algorithms + tfidf. Then we will move on to fine-tune Roberta's data, a pre-trained text classification model based on the Transformers architecture. We will then observe the difference in performance of the different approaches.

2 `Clustering.ipynb`
> We were provided with a dataset containing unlabelled reviews of films. Our goal is to perceive whether these films, through their reviews, are perceived positively (1) or negatively (0). We will therefore apply a clustering algorithm, kmeans++, in order to identify the two described classes and label the reviews. This technique appears to be one of the most widely used in an Unsupervised Learning context. 


**********************
