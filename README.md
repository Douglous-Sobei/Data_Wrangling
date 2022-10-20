# Data_Wrangling

**Introduction**
> Data wrangling is an important skill that people working with data have to aquire since the world's data isn't clean. To make our data clean, wrangling is essential. In any case we analyze, visualize, or model our data before wrangling, the outcome could be making mistakes. Therefore, wrangling is the best practice to reach our expections.

**Gathering summary**
>This was the first step in the data wrangling process. I was able to obtain data from the following sources:
- Got data from an existing file (twitter-archive-enhanced.csv) Reading from csv file using pandas
- Downloaded a file from the internet (image-predictions.tsv) Downloading file using requests
- Did a query of an API (tweet_json.txt) to get JSON object of all the tweet_ids using Tweepy
- Imported the data into my programming environment (Jupyter Notebook)

**Assessing**
> After gathering each of the above pieces of data, I assessed them visually and programmatically for quality and tidiness issues was our next step. We could detect and document the following quality issues and tidiness issues.

**Quality**
- Completeness, Validity, Accuracy, Consistency
- In_reply_to_status_id, in_reply_to_user_id, retweeted_status_id, retweeted_status_user_id should be intergs instead of float
- retweeted_status_timestamp, timestamp should be datetime instead of object (string)
- The numerator and denominator columns have invalid values
- In several columns null objects are non-null (None to NaN)
- We only want original ratings (no retweets) that have images
- Missing values from images dataset (2075 rows instead of 2356)
- Some tweet_ids have the same jpg_url
- This tweet_id (666020888022790149) duplicated 8 times
**tidiness**
- Changed tweet_id to type int64 in order to merge with the other 2 tables

- All tables should be part of one dataset

**Cleaning**
> Cleaning data is the third step in data wrangling. It is where we fixed the quality and tidiness issues that we identified in the assess step.

> I used the two types of cleaning, the manual and programmatic data cleaning. The process was Define, Code and Test and I was always making a copy of the dataset. I aslo made a copy in file to test the change before applying to the main dataset.

**Conclusion**
> Data wrangling indeed is a core skill that everyone who works with data should be familiar with since so much of the world's data isn't clean. If we analyze, visualize, or model our data before we wrangle it, our consequences could be making mistakes, missing out on cool insights, and wasting time. Therefore, dat wrangling is unavoidable.

**Gaps**
> I faced many challenges in my Data wrangling process. I had a hard time in signing up my twitter developer account Sometimes got different results in my gathering process against my expectations
