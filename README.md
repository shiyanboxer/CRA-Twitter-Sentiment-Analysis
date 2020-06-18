CRA Twitter Sentiment Analysis
==========================
## Results
![Graph](https://github.com/shiyanboxer/CRA-Twitter-Sentiment-Analysis/blob/master/Graph.png)
![Results](https://github.com/shiyanboxer/CRA-Twitter-Sentiment-Analysis/blob/master/SAResults.png)
## Notion Link
https://www.notion.so/shiyanboxer/Twitter-Sentiment-Analysis-v2-ef739d444a944254a2e43da829dc45a3

## Quickstart
***Install Dependencies In Anaconda Command Prompt***
- conda install -c conda-forge textblob
- conda install -c conda-forge tweepy
- conda install -c conda-forge wordcloud
- conda install -c anaconda nltk
- pip install stop-words (in command prompt)

## Tech
- **Python** — a programming language
- **Tweepy** — type of RESTful API specifically for Twitter
- **NLTK** — symbolic and statistical natural language processing libraries. It takes care of any processing that we need to perform on text to change its form or extract certain components from it. The class constructor removes stop words.
- **Regular Expression** — parsing strings and modifying dataset library sequence of characters that form a search pattern
- **Pandas** — data manipulation and analysis library
- **NumPy** — scientific computing library
- **Matplotlib** — plotting library
- **JSON** — file type

## The Problem
The purpose of CRA's chatbot is to help Canadians find more information regarding CERB and CESB. Currently, CRA is using Fine-grained Sentiment Analysis - a 5 point ranking survey given to the user after they have completed their interaction to determine customer satisfaction. Although this is a simple approach, it does not provide an in-depth analysis of the customer’s experience nor does it allow real-time personalization to increase satisfaction and improve future iterations.

## Resources
### Authentication and Extracting Tweets
[https://www.earthdatascience.org/courses/use-data-open-source-python/intro-to-apis/twitter-data-in-python/](https://www.earthdatascience.org/courses/use-data-open-source-python/intro-to-apis/twitter-data-in-python/)

### Cursor Method
[http://docs.tweepy.org/en/v3.5.0/cursor_tutorial.html](http://docs.tweepy.org/en/v3.5.0/cursor_tutorial.html)

### YouTube Tutorial
[https://www.youtube.com/watch?v=ujId4ipkBio](https://www.youtube.com/watch?v=ujId4ipkBio)[https://medium.com/better-programming/twitter-sentiment-analysis-15d8892c0082](https://medium.com/better-programming/twitter-sentiment-analysis-15d8892c0082)

### Tutorial for ML Naives Bayes Classifier
[https://towardsdatascience.com/creating-the-twitter-sentiment-analysis-program-in-python-with-naive-bayes-classification-672e5589a7ed](https://towardsdatascience.com/creating-the-twitter-sentiment-analysis-program-in-python-with-naive-bayes-classification-672e5589a7ed)

***Resources for Future Development***
- https://colab.research.google.com/notebooks/intro.ipynb#recent=true
- https://azure.microsoft.com/en-us/services/cognitive-services/text-analytics/#features
- https://nlp.stanford.edu/sentiment/

## twitter-sentiment-training
Training set of 5513 hand-classified tweets for sentiment classifiers.  This is an upgrade to the original script by Niek J. Sanders available [here] (http://www.sananalytics.com/lab/twitter-sentiment/). Twitter's [REST API v1.1] (https://dev.twitter.com/docs/api/1.1) has made it mandatory for all requests to be authenticated using [oauth](https://dev.twitter.com/docs/auth/oauth#v1-1) and hence the script required to incorporate the authentication capability.

Consequently, you must get an access token, access key, consumer token, consumer key by registering your application with twitter, in order to make such authenticated requests. Refer to [this](https://dev.twitter.com/docs/auth/tokens-devtwittercom) guide for getting these tokens, and provide them as global variables in the `install.py` script.

*It is advised to go through the original Readme file given [here](http://www.sananalytics.com/lab/twitter-sentiment/sanders-twitter-0.2.zip) for a better understanding of the project and the install script in particular.*

### Installation
Because of restrictions in Twitter’s Terms of Service, the actual tweets can not be distributed
with the sentiment corpus. A small Python script is included to download all of the tweets. Due
to limitations in Twitter’s API, the download process takes about 43 hours.

Just four easy steps:  
1. Set your access key and secret, consumer key and secret to the global variables declared at the beginning of install.py  
2. Start the tweet downloader script: `python install.py`  
3. Hit enter three times to accept the defaults.  
4. Wait till the script indicates that it’s done.  

Note: the script is smart enough to resume where it left off if downloading is interrupted.
The completed corpus will be in full-corpus.csv. A copy of all the raw data downloaded from Twitter is kept in rawdata/.

----

### Credits
The original work by Niek J. Sanders is a Twitter Sentiment Classifier which can be found [here] (http://www.sananalytics.com/lab/twitter-sentiment/). 
My work is just a little modification to the code written in 2011 to comply with the latest Twitter API v1.1 requirements.

### Support
You may write to me for any help, I'll try and help you to the best of my capability.

Karan Luthra 
karanluthra06@gmail.com


