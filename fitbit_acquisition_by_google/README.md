# Fitbit-acquisition-by-Google
### Team: Neha Anna John, Rawini Dias, Chris Henson, Sadhana Koneni, Satya Naren Pachigolla


Look at the slide deck in this repository for a summary of our findings


## Overview:

Google announced that they are planning to acquire 'Fitbit' on 1st November,2019. Google has been trying to get into the wearables space for quite some time and Fitbit who were the disruptors in this space have been facing tough competition from Apple, Samsung and Sony lately. Hence, this acquisition is a win-win for both the companies. 

In our project, we looked at the customer discussions/perceptions about Fitbit before the acquisition news was announced and then tracked them along the way.

Following are the steps we followed for this project : 

### Data Collection:

Reddit and Twitter were the datasources for our project. Using 'psaw' library we got the Reddit data and by using 'TwitterScraper' we got the Twitter data. From both of these sites, we got any mentions which contained the keyword 'Fitbit'

### Time Period:

We split our analysis to 3 time periods. The period before the announcement was released (before 28th Oct) is the 'Pre Period'. The time during the announcement (28th Oct - 2nd Nov) is the 'Peak Period' and the dates after that is the 'Post Period'

### Analysis done:

#### Data Cleaning: 

After getting the data from Reddit and Twitter, we tokenized the data, removed stopwords, punctuations and some badwords, lemmatized the words using spacy

#### Word Clouds:

Using the 'Wordcloud' package in Python, we got the wordclouds of customer conversations during the 3 periods

#### Topic Modelling:

Using 'LDA' package, we got details about the main conversational topics. Looking at these topics, provided us insights into what the customers were talking about. An interesting observation was that after the acquisition news was announced, few customers were concerned about their data privacy and were thinking of not using their Fitbits anymore.

#### Sentiment Analysis:

We got the sentiment scores using the 'Vader' library in python. It gives us a compounded sentiment score along with individual positive and negative scores as well. We got the user tweet locations using 'Tweepy' and looked at how the sentiment scores changed across various geographies

#### MDS Plot:

Using 'sklearn' we created MDS plots for the lift values between different brands for all three periods in the project. Using these MDS plots, we could clearly see that Fitbit is moving closer to companies like 'Apple' and 'Samsung' after the acquisition news was announced.

