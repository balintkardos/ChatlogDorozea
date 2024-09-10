# Dorozea's Chat Data Analysis Project

## Introduction
This project involves the analysis of twitch chat and twitch viewership data from [Dorozea](https://www.twitch.tv/dorozea)'s chat. The project was undertaken to improve my data analysist skills and to undersand more about the comunity I love and I'm a part of.

## Table of Contents
1. [Data Description](#data-description)
2. [Methodology](#methodology)
3. [Results](#results)
4. [Conclusion](#conclusion)
5. [Usage](#usage)
6. [References](#references)
7. [Contact Information](#contact-information)

## Data Description
The dataset was sourced from public Twitch and includes chat messges date and the sender's data from 2024-05-01 to 2024-08-31. It contains more than 300k records with columns such as Date, User, Message, and StreamID. The data was cleaned to remove duplicates and missing values. If stream crashed and 2 separated vod was, it is merged together.

## Methodology
The analysis was performed using Python, with Pandas for data manipulation, Matplotlib and Seaborn for visualization, WordCloud and ImageColorGenerator for creating cool imagies, and Scikit-learn for predictive modeling.

## Results
//TODO

## Conclusion
//TODO

## Usage
You you need to read all the data from /data where all stream has the own txt file with [m-d-yy].txt format all list is the file_list.txt

```python
# Read the list of filenames from the configuration file
'file_list.txt'
```

## References
- Twitch Data from Twitch: [Link to Dataset](https://www.twitch.tv/dorozea)
- Pandas Documentation: [Link](https://pandas.pydata.org/)
- 

## Contact Information
Author: Bálint Kardos  
Email: kard.balint@gmail.com
LinkedIn: [link](https://www.linkedin.com/in/b%C3%A1lint-kardos/)  

## License
This project has none currently.
