
# Worked in a team of 4 @pei00033 @ZHI00009 @bose0084 @SHARM746 to Analyze Twitter Population Behavior based on Timber Wolves wins & losses 

This analysis allows us to quantify the sentiment of the Timberwolves fans based on the NBA games that Timberwolves win or lose. This system can be extended to quantify and analyze the behavior of the population on a new public policy or a major event. Our repository provides a step-by-step guide to scrape data from Twitter and associate a sentiment to each tweet using NLTK.

## Problem Statement and Motivation
Post implementing a change it's important to track the sentiment of the population towards the change. In our case, we are leveraging tweets from timberwolves Twitter handle to track the sentiment of people post timberwolves wins and losses.

#### Decision Making Scenarios
From this analysis, we aim at enabling the decision-making process in the following ways:
A brand wants to know when the fans are most likely to purchase the timberwolves merchandise 
Help advertisement investors to determine whether  to sponsor the team

## Steps to Run
Post running the Sentiment_Analysis.ipynb notebook do the following
  1. Set up your access_token, access_token_secret, consumer_key, and consumer_secret variables
  2. Set up your AWS bucket and pass your aws_access_key_id, aws_secret_access_key, region_name, and aws_session_token
  3. Run the .ipynb notebook tweets with sentiment associated to them would be stored in your S3 bucket

## Process Flow
Tweets are scraped from specific user-defined Twitter handles.
The scraped data is cleaned to remove emojis & special characters.
An NLTK-based sentiment analysis model runs on top of the tweet data to associate sentiments for each tweet.
Positive
Neutral
Negative
Post sentiment analysis the data is stored in an S3 bucket using BOTO 3 for storage.

_* All the above defined procceses run through the Sentiment_Analysis.ipynb notebook _
## References

https://www.nba.com/timberwolves

https://twitter.com/

https://python.plainenglish.io/scraping-tweets-with-tweepy-python-59413046e788

