# Sentiment Analysis of Tweets for Canada Post, Purolator, and UPS Canada

This repository contains a Python-based sentiment analysis scripts that analyzes tweets related to Canada Post, Purolator, and UPS Canada. The sentiment analysis is performed using the `snscrape`, `nltk`, and `textblob` libraries. The scripts allows you to extract tweets using `snscrape`, preprocess the data using `nltk`, and then conduct sentiment analysis using `textblob`.

## Libraries Used

### 1. snscrape
`snscrape` is a Python library for scraping tweets from Twitter. It provides an easy-to-use interface for fetching tweets based on search queries, usernames, or specific URLs. It allows us to collect relevant tweets from Twitter, which will be used for sentiment analysis.

### 2. nltk (Natural Language Toolkit)
`nltk` is a powerful Python library for natural language processing. It provides various tools and functionalities for text processing, tokenization, stemming, lemmatization, and more. We'll use `nltk` to preprocess the tweets before performing sentiment analysis, which involves removing stop words, punctuation, and converting the text to lowercase.

### 3. textblob
`textblob` is a simple natural language processing library built on top of `nltk`. It provides a straightforward API for common NLP tasks, such as sentiment analysis. With `textblob`, we can determine the sentiment of a given text, whether it is positive, negative, or neutral.

## Natural Language Processing (NLP) in Sentiment Analysis

Natural Language Processing (NLP) is a crucial component of sentiment analysis, enabling machines to understand and interpret human language. In this repository, we use NLP techniques to perform sentiment analysis on tweets related to Canada Post, Purolator, and UPS Canada.
Key NLP Techniques Used:

Tokenization: We break down the tweets into smaller units called tokens (words or sentences) to facilitate further analysis.

Stop Words Removal: Commonly used but uninformative words, known as stop words (e.g., "the," "and," "is"), are removed to reduce noise and improve analysis accuracy.

Stemming and Lemmatization: These processes help in reducing words to their root form, standardizing variations, and simplifying analysis.

Sentiment Analysis: We leverage textblob, an NLP library, to determine the sentiment of each tweet (positive, negative, or neutral) based on its content.

Importance in Sentiment Analysis:

Contextual Understanding: NLP enables the analysis of tweets in their context, as words may have different sentiment implications based on the context they appear in.

Handling Informal Language: Tweets often contain slang, emojis, and informal language. NLP models are designed to handle such linguistic features for accurate sentiment analysis.

Negations Handling: NLP models consider negations in sentences, reversing sentiment where appropriate (e.g., "not good" becomes negative).

By utilizing NLP techniques, we can gain valuable insights into the sentiments expressed towards Canada Post, Purolator, and UPS Canada based on user-generated content from Twitter.

## How to Use this Repository

Follow these steps to use the sentiment analysis tool for tweets related to Canada Post, Purolator, and UPS Canada:

1. Clone the Repository: Start by cloning this GitHub repository to your local machine using the following command:

```bash
git clone https://github.com/your-username/sentiment-analysis-tweets-canada.git
```

2. Install Dependencies: Make sure you have Python installed on your system. Then, install the required libraries by running the following command:

```bash
pip install snscrape nltk textblob
```

3. Extract Tweets: Open the `Twitter_Extract.ipynb` file and update the search query to fetch relevant tweets related to Canada Post, Purolator, and UPS Canada. You can customize the search query as needed to collect specific tweets. Run the script to extract the tweets and save them in a CSV file.

4. Preprocess Data: Once the tweets are extracted and saved in the CSV file, run the `CanadaPost_SentimentalAnalysis.ipynb`, `Purolator_sentimentalAnalysis.ipynb` and `UPS_sentimentalAnalysis.ipynb` scripts. This script will use `nltk` to preprocess the tweets by removing stop words, punctuation, and converting the text to lowercase, etc.

5. Sentiment Analysis: After preprocessing the data, use the same scripts to perform sentiment analysis on the tweets. The script will use `textblob` to analyze the sentiment of each tweet and classify it as positive, negative, or neutral.

6. View Results: The results of the sentiment analysis will be displayed on the console and saved in a new CSV file. You can analyze the sentiment trends and compare the sentiment scores for Canada Post, Purolator, and UPS Canada.

Please note that this is a basic sentiment analysis tool, and the accuracy of sentiment analysis may vary depending on the quality and quantity of the tweets collected. Additionally, ensure that you comply with Twitter's usage policies while scraping tweets.

Happy sentiment analysis! If you have any questions or improvements, feel free to contribute to this repository.
