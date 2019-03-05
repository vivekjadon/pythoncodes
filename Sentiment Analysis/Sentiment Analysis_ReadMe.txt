Sentiment Analysis 

Purpose: This assignment will cover sentiment analysis that is used to understand sentiment of the textual information. The goal is that students understand what is sentiment analysis, how text can be classified into positive/neutral/negative sentiment, and what conclusions can be made based on sentiment analysis. 

1. For this assignment, we will implement sentiment analysis of tweets using Python and NLTK (the natural language toolkit). We essentially would like to classify a given tweet as “positive” or “negative” tweet in terms of user sentiment. We will be using a pre-defined list of tweets (see below) as actually doing a live analysis of twitter feeds will be done in a later assignment. 

2. Create two lists, one of positive tweets, and the other of negative tweets as follows: 

pos_tweets = [('I love this car', 'positive'), ('This view is amazing', 'positive'), ('I feel great this morning', 'positive'), ('I am so excited about the concert', 'positive'), ('He is my best friend', 'positive')] 

neg_tweets = [('I do not like this car', 'negative'), ('This view is horrible', 'negative'), ('I feel tired this morning', 'negative'), ('I am not looking forward to the concert', 'negative'), ('He is my enemy', 'negative')] 

3. Now take both of these lists and create a single list, where the first element is an array containing the words and second element is the sentiment: ‘positive’ / ‘negative’, call this list ‘tweets’. Further, exclude items that are smaller than 2 characters in length, and convert all text to lowercase. 

4. Now create a list of “test tweets” from the following: 
a.	I feel happy this morning. positive. 
b.	Larry is my friend. positive. 
c.	I do not like that man. negative. 
d.	My house is not great. negative. 
e.	Your song is annoying. negative. 

5. Use the nltk.FreqDist function to get a list of distinct words ordered by frequency of appearance. 

6. Now that you have your training set, use the Naive Bayes classifier to train a classifier to actually appropriately classify a tweet as “positive” or “negative”, using the nltk.NaiveBayesClassifier.train function. 

7. Using the classifier you have just created, input some test tweets (you can obtain these from the list above) to get a probability measure of ‘positive’ or ‘negative’. 
