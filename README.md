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

![Tweet process](https://github.com/Darshan-302/Twitter-Sentimental-Analysis/blob/main/tweet%20process.jpg)

## Word Cloud Generation

With the help of the POS-tag (Parts of Speech tagging) module in the NLTK library, I was able to compile a list of the most often used terms to represent 2020.
One can create a Word Cloud based on word frequency and overlay these words on any image by using the WordCloud library.
In this instance, I displayed the image using Matplotlib with the Twitter logo.
The Word Cloud displays the more frequent terms in larger text sizes, while the less frequent words are displayed in smaller letter sizes. 

![Word Cloud](https://github.com/Darshan-302/Twitter-Sentimental-Analysis/blob/main/wordcloud.png)

## Visulizing Most Common Words

The Plot below was genrated using Plotly Library for Python.

![Most words](https://github.com/Darshan-302/Twitter-Sentimental-Analysis/blob/main/Most%20words.png)

## Sentiment Analysis

My choice for this analysis was TextBlob.
By assigning a Subjectivity and Polarity score to each tweet, Text Blob evaluates each statement.
One can identify which tweets were positive, negative, or neutral based on the Polarity scores.
A Polarity score of 0 indicates a negative, neutral, or > 0 indicates a positive.
I returned the appropriate Sentiment Category by applying the "apply" method to the "Polarity" column in my data frame.
Below is a breakdown of the sentiment categories.
On the Tableau dashboard, you can also check the distribution of sentiment categories by continent and nation. 

![Distribution of Sentiment](https://github.com/Darshan-302/Twitter-Sentimental-Analysis/blob/main/Distribution%20of%20Sentiment.png)

## Final Dashboard

Here is a complete look of FInal Dashboard on Tableau.

![Final Dashboard](https://github.com/Darshan-302/Twitter-Sentimental-Analysis/blob/main/Final%20Dashboard.png)

We can see live Dashboard on my teammate's account. Link is provided below.

https://public.tableau.com/app/profile/helly7895/viz/TwitterSentimentalAnalysisDashboard/FinalDashboard?publish=yes

