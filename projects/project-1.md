---
layout: project
type: project
image: images/project-1.png
title: Automated Twitter Keyword and Hashtag Sentiment Analysis
permalink: projects/micromouse
# All dates must be YYYY-MM-DD format!
date: 2020-07-14
labels:
  - Python
  - Object-oreiented programming
  - Tweepy
  - Textblob
  - Regular Expression
  - Plotly
summary: TwitAnlysis-to-csv scrapes user specified keywords and hashtags, performs sentiment analysis using textblob lexicon and plots the result with a click.
---

<img class="ui fluid image"  src="../images/overview.gif">

More and more people are turning online to voice their opinions, whether on products, services, politics, or daily issues. To get a better picture of how the crowd is feeling, it is important to analyze their opinions. 

In this project, using python, I have written a block of code that will semi-automatically scrape twitter (using your input keyword), perform sentiment analysis, and plot the sentiments values onto two graphs. The data was scrapped from Twitter using [Tweepy](http://docs.tweepy.org/en/v3.5.0/api.html), [Textblob](https://textblob.readthedocs.io/en/dev/) was used to perform sentiment analysis (lexicon method) and [Plotly](https://plotly.com/python/) was used for data visualization.

This project incorporates the understanding of API, object-oriented programming, regular expression and data visualization. I had fun making the project, especially while writing the code for automatic graph plotting!


## Getting Started

The instructions below will help you set up the environment.

### Prerequisites

To use the program, you need to statisfy the conditions below:

```
1. Anaconda (to get Jupyter Notebook)
1. Jupyter Notebook (or any other python software)
2. Twitter Developer Account (to get credential tokens)
```

All are free to use and getting these tools will take about 10 minutes to do so. Once you have those tools, go ahead and open the downloaded file ‘Twitter Scrapper Lexicon Analysis.ipynb’ on your computer. 

Next, you would need to navigate back to Twitter developer account. Now, create an application (free), and grab the API key (consumer key), API key secret (consumer secret key), access token and access token secret key from your ‘Project & App’ tab. 

Finally, you are ready to use the program!

### Demonstration of program

**Step 1:** Import the libraries. 

* If you dont have these libraries installed, type in the code below and hit SHIFT+ENTER.

```
!pip install textblob
!pip install tweepy
!pip install plotly
```

**Step 2:** Insert Twitter authentication keys that you have obtained.

<img class="ui fluid image"  src="../images/Settinguptwitter.PNG">

**Step 3:** Excecute the cell. A prompt will appear requesting for your input, insert the keyword that you wish to find and hit ENTER. 

* For the keyword, you can insert one or more words, the end result is dependent on Twitter search algorithm.
* As an example, I will be searching for the keyword 'jamus lim', a Singaporean politician who is currently a local internet sentation.

<img class="ui fluid image"  src="../images/searchtwitter.PNG">

**Step 4:** That's all! 

* The results are generated and an excel CSV file, under the name of 'Twitter_Analysis.csv' will be saved in the same folder where 'Twitter Scrapper Lexicon Analysis.ipynb' was. 

* Here are the results

<img class="ui fluid image"  src="../images/result_1.png">

<img class="ui fluid image"  src="../images/result_2.png">

The result is accurate to a certain extend. Singaporeans have high admiration for Jamus Lim and it was well reflected by the sentiment analysis. Out of the 34 scrapped tweets, 17 (50%) were deemed positive, 15(44%) were deemed neutral or objective and 2 (5%) were deemed negative. 

Although this program is not 100% accurate (especially so when we are analysing tweets where people are more likely to use short forms and slangs), it does give a very rough sense of what people are feeling. You can evalute the sentiment by looking at the CSV file. 

### What I wish to do next

```
1. Make a stand alone exe file using python Tkinter GUI and Pyinstaller
2. Create a looping automatic tweet scrapper (Stream Tweets) into a database (SQLite)
```
## Code

* [Link to this project](https://github.com/thongekchakrit/TwitAnlysis-to-csv/blob/master/notebook/Twitter%20Scrapper%20Lexicon%20Analysis.ipynb)

## Built With

* [Anaconda](https://www.anaconda.com/) - Required for Jupyter Notebook
* [Jupyter Notebook](https://jupyter.org/)
* [Plotly](https://plotly.com/python/) - Use to visualize data
* [Tweepy](http://docs.tweepy.org/en/v3.5.0/api.html) - Use to scrape twitter API
* [Textblob](https://textblob.readthedocs.io/en/dev/) - Use for sentiment analysis
* [Twitter Developer Account](https://developer.twitter.com/en)


## Author

* [Chakrit Thong Ek](https://github.com/thongekchakrit)


