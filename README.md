# Dorozea's Chat Data Analysis Project
<a href="https://www.twitch.tv/dorozea">
    <img src="https://kappa.lol/uonYy" alt="Alt text" width="200"/>
</a>

## Introduction
This project involves the analysis of twitch chat and twitch viewership data from [Dorozea](https://www.twitch.tv/dorozea)'s chat. I want to show what you can learn from twitch chat messages and minimal a viwership data. The project was undertaken to improve my data analysist skills and to undersand more about the comunity I love and I'm a part of.

## Table of Contents
1. [Data Description](#data-description)
2. [Known limitations](#known-limitations)
3. [Methodology](#methodology)
4. [Results](#results)
5. [Usage](#usage)
6. [References](#references)
7. [Contact Information](#contact-information)

## Data Description
The dataset was sourced from public Twitch and includes chat messges date and the sender's data from 2024-05-01 to last stream's date. It contains more than 300k records with columns such as Date, User, Message, and StreamID from more than 110 streames. The data was cleaned to remove duplicates and missing values. If stream crashed and 2-3 separated vod was, it is merged together.

## Known limitations
- It has __no__ chat log data when the steam was __offline__. It is also true when the stream crashed and it was offline for only few minutes.
- If a user has been __banned__ or their message has been __deleted__ in the live chat, they are not included.
- Can't handel __user name change__. If a user changed his user name it will be appear as a brand new user.

## Methodology
The analysis was performed using Python, with Pandas for data manipulation, Matplotlib and Seaborn for visualization, WordCloud and ImageColorGenerator for creating cool imagies, and Scikit-learn for predictive modeling.

## Results
### The project has 4 main jupiter notebooks. 

- [streams_stats](streams_stats.ipynb): \
This is the main file in which everything is calculated for each stream.
    - First time chater
    - Tottal messages
    - Unique chatter
    - Stream's length
    - Returning user from last stream
    - Avg viewers count
    - Max viewers count
    - Follow gainted
    - Sum of user whos only sended 1 message on the stream
    - Games was streamed
    - Tottal word count
    - Message per minutes
    - Top 5 user
    - Top 5 word
    - Prime/tier1/tier2/tier3/gift subscription data
    - Raid data
    - Active subscription data
    - etc. \

    And has has garph almost every calculated data.

    <img src="https://kappa.lol/1TrMI" alt="Alt text" width="800"/>

- [months](months.ipynb): \
Creates a monthly table of the subscriptions of the given month, divided into tiers, and calculates the income from this. calculates the possible advertising revenue from watch time.
- [Predictions](Predictions.ipynb): \
From the data so far, it tries to tell when Dorozea will reach the 300b sub number only from prime and tier1, or an average of 500 viewers, or the 5 million watched hours required for the Twitch trophy. \
From data 2024 09 09:
    - Expected to reach 500 average viewers on: 2025-08-22 
    - Expected to reach 300 active tier 1 & prime subs on: 2025-06-20 
    - Expected to reach 5000000 watch hours on: 2030-12-02
- [worldCloudWithImage](worldCloudWithImage.ipynb):
It creates a word cloud from the most frequently used chat words, which he places on dorozea's logo.
<img src="https://kappa.lol/ptfxA" alt="Alt text" width="300"/>


## Usage
You you need to read all the data from /data where all stream has the own txt file with [m-d-yy].txt format all list is the file_list.txt
[file_list.txt](file_list.txt)

## References
- Twitch Data from Twitch: [Link to Dorozea's channel](https://www.twitch.tv/dorozea)
- Twitch chat downloder: [Link](https://github.com/lay295/TwitchDownloader)
- Pandas Documentation: [Link](https://pandas.pydata.org)


## Contact Information
Author: Bálint Kardos  
Email: kard.balint@gmail.com \
LinkedIn: [Bálint Kardos](https://www.linkedin.com/in/b%C3%A1lint-kardos/)  
Twitch: [balintboss](https://www.twitch.tv/balintboss)

## License
This project has none currently.


```python
# this is just a place horder
'file_list.txt'
```