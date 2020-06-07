# Predicting-Drug-Abuse-Behaviour-using-DL
This repository contains all the codes and output files of the project carried out on the topic-Predicting Drug Abuse Behaviour using Deep Learning Techniques

Keywords— drugs, hash , BERT, Tweepy, Twitter, timeline, students, depression, BoW, drug abuse behaviour, cosine similarities, LDA, MultinomialNB, LSVM, random forest classifier, NLP, deep learning.

List of codes used in the project:

1.**getTweets**:Looks for timelines and fetches the tweet texts.For the authentication of the Tweepy API required consumer and access keys and tokens should be obtained from an active Twitter's Developer account.
  Environment: Jupyter Notebook
  Libraries imported: tweepy, pandas, os, json
  
2.**cleaning**: Preprocessing the user timeline tweets.
  Environment: Jupyter Notebook
  Libraries imported: nltk.stem, nltk.tokenize
  
3.**lda**: Fetching 10 clouds of 15 words from the clean timeline data. 
  Environment: IDLE (Python 3.7)
  Libraries imported: gensim

4.**clearlda**: Removing extras from lda output. 
  Environment: Jupyter Notebook
  Libraries imported: pandas

5.**randomDivisionOfBow**: Randomly dividing 120 words of BoW into 8 lines of 15 words each. 
  Environment: Jupyter Notebook
  Libraries imported: random, pandas

6.**Computing Similarities**: Extracting the sentence embeddings of both the 10 clouds of 15 words and the BoW. Computing the cosine similarities of the pair of sentence embeddings.
 8 values similarity indices will be there for each cloud of 15 words,averaging it to a single similarity index. 
  Environment: Google Colab
  Libraries imported: torch,pytorch_pretrained_bert,sklearn

7.**targetTweets**: Comparing similarity indices of clouds of words. Fetching target tweets and saving in a CSV file.  
  Environment: Jupyter Notebook
  Libraries imported: pandas, json

8.**BoW**: Create a bag of words using the ‘ddd.txt’ file which contains paragraphs of some articles and clean tweets related to drugs. Create a corpus and then after cleaning, create a dictionary of tokens and extract words with highest frequency and put them into BoW.  
  Environment: Jupyter Notebook(Google Colab)
  Libraries imported: pandas, re, string, nltk, heapq
  
9.**Text Emotion Detection**: Predicting the emotions of each target tweet of scholars using the random forest classification model and comparing the performance of LSVM and RF model.
  Environment: Jupyter Notebook (Google Colab)
  Libraries imported: pandas, re, string, nltk, sklearn, preprocessing, matplotlib.pyplot, sklearn.ensemble



