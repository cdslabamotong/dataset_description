# Datasets Description and Statistics
This repo is maintained to keep track of all the retrieved dataset that the CDS lab have collected so far. The collected dataset is composed of three components - Non-network social media data, fake news data, and fact-checking data.  

## Non-network Social Media Data (26GB)
**Using Machine Learning to Detect Cyberbullying.**  (11.5MB)  
A large unlabeled Formspring dataset (187 MB, archived size), from a Summer 2010 crawl containing all of the questions and answers for 18,554 Formspring users. The dataset is about to cyberbullying related user's comments.

**GeneralData**  (13MB)   
Additional labeled cyberbullying data from Formspring. It contains 56 chatting logs which are related to Cyberbullying. The time range is unknown.

**Bullying Traces v3.0**  (3MB)  
This dataset contains data collected from Twitter stream API and labeled by experienced annotators for the study of bullying in social media. We collected tweets using the public Twitter stream API, such that each tweet contains at least one of the following keywords: "bully, bullied, bullying". It contains 7,321 annotated data during August 6-31, 2011. 

**Detecting the Presence of Cyberbullying Using Computer Software.**  (20MB)   
Human Concensus.zip - contains 11 spreadsheets.  Each spreadsheet contains the labeling information for one packet  
xml packet XXXX.zip - contains a set of xml files.  Each file is a window of 10 posts (unless a thread had less than 10 posts)

**Text Mining and Cyber Crime Data**  (53MB)   
This dataset contains the full chatting records of Cyber Crime data with coded and uncoded hate words. For the records with uncoded hate/crime words, it has 197 full text files. And 288 coded hate words. The time range is unknown.

**RF Respiration Dataverse**  (3.7GB)   
This dataset comes from Harvard database and contains the raw RF measurements, polysomnography, and patient data gathered during day 00 of a 20-day study. SpecificaLLY, This dataset is from one day in a 20-day study to use RF devices to perform respiration monitoring. Polysomnography data was being collected simultaneously which we used to get the ground truth respiration rate. The data was used to compare the effectiveness of each RF device in performing respiration monitoring.

**Stuck in the Matrix**  (20GB)   
This dataset is a massive analysis of Reddit's entire publicly available comment dataset. The dataset is ~1.7 billion JSON objects complete with the comment, score, author, subreddit, position in comment tree and other fields that are available through Reddit's API. Total Comments amount is 53,851,542 from 2014 to 2017.

**Social Discussion Forum Data (Reddit)**  (1.6GB)  
 comprehensive dataset of topic stream data and associated reply data from Reddit (retrieved by Pushshift API). It contains three sub-datasets retrieved from two subforums. Both main threads and associated replies have the same data format: ID, title, URL, author, score, text, and num_replies. 
 - NBA Dataset (2018/04 - 2018/06): 63577 main threads and 4.6 million associated replies
 - NBA Dataset (2019/04): 24874 main threads and more than 2 million associated replies.
 - Movie Dataset (2019/04 - 2019/05): 6857 main threads and 24517 replies.

## False Information Data (7GB)
**Detecting Rumors from Microblogs with Recurrent Neural Networks.** (4GB)   

- Twitter Data (Twitter.txt): This corpus contains 992 labeled events in total. Each line contains one event with the ids of relevant tweets: event_id, label, tweet_ids. For the labels, the value is 1 if the event is a rumor, and is 0 otherwise. Note that we cannot release the specific content of tweets due to the terms of use of Twitter data. Users can download the content themselves via Twitter API. 

- Weibo Data (Weibo.txt): This corpus contains 4664 labeled events in total. Each line contains one event with ids of relevent posts with format: event_id, label, post_ids. For the labels, the value is 1 if the event is a rumor, and is 0 otherwise. We also release the content of all the posts in json format which are saved in the ./Weibo directory, where each file is named as event_id.json, corresponding to individual event.

**PHEME-R: Analyzing How People Orient to and Spread Rumours in Social Media by Lookingat Conversational Threads.**  (574MB)  
This directory contains the PHEME rumour dataset collected and annotated within the journalism use case of the project. These rumours are associated with 9 different breaking news. It was created for the analysis of social media rumours, and contains Twitter conversations which are initiated by a rumourous tweet. The dataset contains 330 conversational threads (297 in English, and 33 in German), with a folder for each thread.

**PHEME.All-in-one: Multi-task Learning for Rumour Verification. **   (46.5MB)  
PHEME dataset of rumours and non-rumours related to nine events, each updated with veracity information for each of the rumours. This dataset contains 3 levels of annotation.  First, each thread is annotated as either rumour or non-rumour; second, rumours are labeled as either true, false or unverified. And third, a subset (threads usedin RumourEval) is annotated for stance classification at the tweet level through crowd-sourcing. In summary, it contains totally 6425 threads, 105354 tweets, 2402 rumors, 4023 non-rumors.

**Getting Real about Fake News - Kaggle Dataset**  (56.7MB)  
The dataset contains text and metadata from 244 websites and represents 12,999 posts in total from the past 30 days. Each website was labeled according to the BS Detector as documented here. Data sources that were missing a label were simply assigned a label of "bs". There are (ostensibly) no genuine, reliable, or trustworthy news sources represented in this dataset (so far).

**This Just In: Fake News Packs a Lot in Title, Uses Simpler, Repetitive Content in Text Body, More Similar to Satire than Real News**   (2MB)  
This repository contains two independent news datasets:  
1. Buzzfeed Political News Data:
	* News originally analyzed by Craig Silverman of Buzzfeed News in article entitled " This Analysis Shows How Viral Fake Election News Stories Outperformed Real News On Facebook."
	* BuzzFeed News used  keyword search on the content analysis tool BuzzSumo to find news stories 
	* Post the analysis of Buzzfeed News, we collect the body text and body title of all articles and use the ground truth as set by Buzzfeed as actual ground truth.
	* This data set has less clear restrictions on the ground truth, including opinion-based real stories and satire-based fake stories. In our study, we manually filter this data set down to contain only "hard" news stories and malicious fake news stories. This repository contains the whole dataset with no filtering.     
  
2. Random Political News Data: 
	* Randomly collected from three types of sources during 2016. 
	* Sources ground truth determined through: Business Insider’s “Most Trusted” list and Zimdars 2016 Fake news list
	* Sources:
		- Real: Wall Street Journal, The Economist, BBC, NPR, ABC, CBS, USA Today, The Guardian, NBC, The Washington Post
		- Satire: The Onion, Huffington Post Satire, Borowitz Report, The Beaverton, Satire Wire, and Faking News
		- Fake: Ending The Fed, True Pundit, abcnews.com.co, DC Gazette, Liberty Writers News, Before its News, InfoWars, Real News Right Now

**Who starts and who debunks rumors - Kaggle Dataset**  (10MB)  
This dataset consists of three files. One file is a collection of all webpages cited in Emergent.info, and the second is a collection of webpages cited in Snopes.com, and the third is a similar collection from Politifact.com. The webpages were often cited because they had started a rumor, shared a rumor, or debunked a rumor. This dataset is created to study domains that frequently start, propagate, or debunk rumors. By studying these domains and people who follow them, we can gain some insight into the dynamics of rumor propagation on the web, as well as social media. 

**FakeNewsNet** (44.1MB)    
FakeNewsNet: A Data Repository with News Content, Social Context andDynamic Information for Studying Fake News on Social Media. This dataset contain 4 sample files: gossipcop_fake.csv, gossipcop_real.csv, politifact_fact.csv, and politifact_real.csv, which are fake/real news collected from PolitiFact and GossipCop. Additionally, this dataset has the code for downloading any additional data. Each of the above CSV files is comma separated file and have the following columns:
- id: Unique identifider for each news
- url: Url of the article from web that published that news
- title: Title of the news article
- tweet_ids: Tweet ids of tweets sharing the news. This field is list of tweet ids separated by tab.

**Rumor Dection ACL_2017** (89.4MB)     
Detect Rumors in Microblog Posts Using Propagation Structure via Kernel Learning. The dataset contains two Twitter dataset: tweeter15 (1,490 tweets, retrieved from 2015) and twitter16 (818 tweets, retrieved from 2016).

**FEVER: A Large-scale Dataset for Fact Extraction and VERification**（1.8GB）    
The dataset was constructed in two stages: 
- Claim Generation Extracting: information from Wikipedia and generating claims from it.
- Claim Labeling: Classifying whether a claim is supported or refuted by Wikipedia and selecting the evidence for it, or deciding there’s not enough information to make a decision.

This dataset contains 145449 training set and 19998 testing set.

## Debunking Information Data (2.7GB)

**Snopes Debunking information dataset**  (200MB)  
The debunking information is retrieved from Snopes.com, and it contains the fact-checking news from 2017/01 to 2018/12, and it has 4532 debunking information.

**Fake News vs Satire: A Dataset and Analysis **  (7MB)     
The dataset includes full text of the articles, labels indicating their type (fake news or satire) and themes, and debunking articles for all fake news. It contain 493 articles with two classes - rumor(292) and non-rumor(201). 

**Twitter Debunking Information Dataset**  (2.6GB)  
This dataset is the complete tweets dataset retrieved between 04/17 to 09/17 from Twitter, which is about Snopes debunking information related tweets. Totally it contains 215 rumors topics with over 0.5 million tweets. 
