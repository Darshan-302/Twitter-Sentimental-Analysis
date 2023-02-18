# Twitter-Sentimental-Analysis

Natural language processing (NLP) techniques were used for this project.
I thought it would be a nice idea to find out what Twitter followers thought of the year in December 2020. 
I merely needed to figure out how to retrieve the information because Twitter users all around the world send over 500 million tweets per day.
This project made use of Python libraries such as Pandas (for data cleaning/manipulation), Tweepy (for mining tweets), NLTK (Natural Language Toolkit), TextBlob (for sentiment analysis), MatPlotlib & WordCloud (for data exploration), Emot (for identifying emojis), and Plotly (for some data visualization). 

In the Jupyter Notebook, you will leearn how I carried out the following steps for the project:

1. Import Libraries
2. Tweets Mining
3. Data Cleaning
4. Location Geocoding
5. Tweets Processing
6. Data Exploration
7. Sentiment Analysis

## Tweets Processing Steps 

The individual tweets have to be cleaned up in order to achieve the main objective.
To make this simple, I built the "preProcessTweets" function into my Python program and then applied it to the "Tweets" to get the required outcomes.
Punctuation, links, emoticons, and stop words were all removed from the tweets using this user-defined function in a single pass.
In addition, I applied an NLP principle called "Tokenization."
It is a technique for removing superfluous parts of a phrase by breaking it up into smaller chunks called "tokens."
"Lemmatization" is a further method worth mentioning.
Words are being "reverted" to their "base" form through this process.
The image below is straightforward. A simple illustration is shown below.



