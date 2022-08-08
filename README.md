# Vaccine-Twitter-Sentiment-Analysis
Using VADER to classify sentiment of tweets and annotate data. Python Notebook included in main root.

 Analysis and report conclusion created May 4, 2021. 
 
 Note: Orignal data source has been updated since then.
 
 Dataset Source:  https://www.kaggle.com/gpreda/pfizer-vaccine-tweets


This project will focus on finding the sentiment of tweets concerning the Covid vaccine produced by Pfizer. Understanding the sentiment around the Pfizer vaccine will be helpful in understanding how the public feels, and indicate how receptive they are to taking the vaccine. To do this I will use an unannotated twitter dataset from Kaggle and perform an NLP Sentiment Analysis with a combination of various techniques. There are 2 ways to perform this analysis:

- I will first use a Positive Word and Negative Word lexicon (each drawn from text files) to conduct exploratory analysis and find the number of positive words and negative words total in the tweets from the dataset

- Secondly I will use VADER(Valence Aware Dictionary and sEntiment Reasoner) which is a lexicon and rule-based sentiment analysis tool that works especially well with social media texts. VADER is unique because it gives us polarity scores and can give us the intesity of the positive or negative tweet. VADER is able to not only map positive and negative words to the correct sentiment, but uses the context of the surrounding words to understand the tweets true sentiment. For example, a person might tweet,"did not love", and VADER will classify it as negative, and not be confused by the positive word 'love'. This shows that VADER has been trained to better classify nuance in text. For this reason it works better for social media commments than a traditional Lexicon Word Counter. It is downloadable from the NLTK package and can be applied to unlabeled data.
    The VADER tools source can be found here: https://github.com/cjhutto/vaderSentiment

    Citation: Hutto, C.J. & Gilbert, E.E. (2014). VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Eighth International Conference on Weblogs and Social Media (ICWSM-14). Ann Arbor, MI, June 2014.

With the SentimentIntensityAnalyzer imported from VADER, we can not only gather count of sentiment for the tweets, but classify them and create a new column that labels the tweet Positive, Negative, or Neutral. This labeling can be used to show difference between sentiment. I will also show how sentiment has looked over time.
