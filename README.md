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
You can use it with this:

```python
# Read the list of filenames from the configuration file
with open('file_list.txt', 'r', encoding='utf-8') as config_file:
    file_names = config_file.read().splitlines()

# Regex pattern to match the data format
pattern = r'\[(.*?)\] (.*?): (.*)'

# Initialize an empty list to store parsed data
datalist = []
stream_count = 0

# Iterate over each specified file
for file in file_names:
    full_path = "data\\" + file
    with open(full_path, 'r', encoding='utf-8') as f:
        lines = f.readlines()
        for line in lines:
            match = re.match(pattern, line)
            if match:
                date, user, message = match.groups()
                datalist.append([date, user, message, stream_count])
    stream_count += 1
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
