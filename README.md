# Election-Result-Prediction-using-Social-Network-Analysis-Twitter
General Lok Sabha Elections 2019 result prediction using twitter network analysis, sentiment analysis on election related tweets.

## Twitter and Lok Sabha Elections 2019
Indian General Lok Sabha elections were held in 2019 between the timestamp of 11 April to 19 May. Various parties, particularly political leaders, used Twitter extensively during general election campaign. Twitter served as a site for real-time public discussions about the #LokSabhaElections2019. The volume of conversation surrounding #LokSabhaElections2019, including Tweets from candidates, political parties, citizens, and the news media, resulted in more than **396 million Tweets** on the platform from 1 January 2019 to 23 May 2019, representing a nearly 600% increase from 2014. 


## Data Info
Keeping this in mind, Election related tweets has been extracted from twitter between the timeline from 1 January 2019 to 23 May 2019. Use of popular keywords and hashtags were made that were trending at the time of campaign. Also used the usernames of the political leaders and political parties.

**Poular Hashtags** - #LokSabhaElections2019, #IndianElection2019, #NarendraModi, #RahulGandhi, #BJP, #INC Keywords - Jobs, Religion, National Security, Agriculture, employment, Demonetisation

Between the same timeline tweets from Narendra Modi & Rahul Gandhi are also collected extracted with some constraints to maintain the relevant to election. Only Tweets written in English are collected hence total tweets count is lower than expected. The data is collected and then cleaned so as to get unique tweets.

**Data contains:**

Date - timestamp of the tweet being public

User - Twitter username of user of which the tweet belongs to

Tweet - full text tweet by user 

<img width="800" alt="image" src="https://github.com/Yoge-sh/Election-Result-Prediction-using-Social-Network-Analysis-Twitter/assets/93325653/9f205ac3-f933-45da-a83d-fc8b14d595d1">

## Sentiment Analysis
Three popular frameworks were used to find the sentiments of the tweets
1. **Bert
2. textBlob
3. vader sentiment
4. get nrc sentiment
5. flair**

With some differences seen in calculation of the sentiment score based on different models, the final output data looked like this:

<img width="908" alt="image" src="https://github.com/Yoge-sh/Election-Result-Prediction-using-Social-Network-Analysis-Twitter/assets/93325653/142aacd3-429e-4c5f-b270-2c75948acfb9">


## Analysis
Glimpse of the network is as seen below:

<img width="500" alt="image" src="https://github.com/Yoge-sh/Election-Result-Prediction-using-Social-Network-Analysis-Twitter/assets/93325653/70832de3-1aa9-42ff-9b24-43bab57a3544">

The overall sentiment score comparison of the two models (flair and VS) for Narendra Modi and Rahul Gandhi related tweets is as follow:

![image](https://github.com/Yoge-sh/Election-Result-Prediction-using-Social-Network-Analysis-Twitter/assets/93325653/4e914255-38a3-44e6-8063-ad4ccebde148)

## Result and Conclusions
📌 Both candidate have RELATIVELY same no. of tweets so we can assume somewhat same engagement from both sides.

📌 Though if we see the negative polarity score is more for Rahul Gandhi's tweets than Narendra Modi's tweets, It may be beneficial for both the sides as RG is the leader of opposition and NaMo was present PM, But POSITIVE APPROACH OF MODI'S TWEETS MAY BE SLIGHTLY MORE THAN RAHUL GANDHI'S NEGATIVE TWEETS.

📌 If we see by using Vader Sentiments on raw data, we see that positive tweets percentage for Narendra Modi is more than Rahul Gandhi (though slightly)

📌 No. of tweets mentioning about Rahul Gandhi (14148) is very less than Narendra Modi(25683)

📌 If we see analysis with get_nrc_sentiment (R library) we see there is sudden difference between Disgust and joy curve in Narendra Modi but it almost same in case of Rahul Gandhi
So if we consider only on the twitter data we can say that Narendra Modi is ahead of Rahul Gandhi in terms of twitter popularity, overall polarity and audience engagement.
So all the way it goes into favor of Narendra Modi.

**Hence chances of Narendra Modi to win the election was more than Rahul Gandhi.**

The detailed analysis and result can be found in result folder in the form of ppt and also as the output of the respective jupiter notebook files
