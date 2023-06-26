# Coronavirus-Tweet-Sentiment-Analysis

Index
1. Introduction
2. Exploratory Data Analysis./Reviwing Our Dataset
3. Data Preprocessing.
4. Model Training- MULTICLASS AND BINARY.
5. Evaluation.
6. Conclusion.


# 1. Introduction

Our objective is to build a classification model to predict the sentiment of COVID-19 tweets.The tweets have been pulled from Twitter and manual tagging has been done then. The names and usernames have been given codes to avoid any privacy concerns.

![image](https://github.com/ashishdhawas/Coronavirus-Tweet-Sentiment-Analysis/assets/86394831/6f548e37-60e4-4df1-949d-ea3068c67718)

**We are given the following information:**

Username: Unique user-IDs of the users

Location: Location of the user

Tweet At: Date at which the tweet was made

Original Tweet: The exact tweet

Sentiment: Sentiment of the tweet

**Workflow in this Project**

![image](https://github.com/ashishdhawas/Coronavirus-Tweet-Sentiment-Analysis/assets/86394831/2b38f641-cf91-49d5-bca8-fa03682c70db)


# 2. Exploratory Data Analysis
   
The original dataset has 6 columns and 41157 rows.

There are five types of sentiments- Extremely Negative, Negative, Neutral, Positive and Extremely Positive.

![image](https://github.com/ashishdhawas/Coronavirus-Tweet-Sentiment-Analysis/assets/86394831/322ec000-e931-4a59-965b-2136d889886f)

All tweets data collected from the months of March and April 2020. Bar plot shows us the number of unique values in each column.

![image](https://github.com/ashishdhawas/Coronavirus-Tweet-Sentiment-Analysis/assets/86394831/6e867b81-d163-4dd2-a155-b087f10f23b9)

The columns such as “UserName” and “ScreenName” does not give any meaningful insights for our analysis.

There are 20.87%(8567) null values in various places of location column.

Most of the tweets came from London followed by U.S.

![image](https://github.com/ashishdhawas/Coronavirus-Tweet-Sentiment-Analysis/assets/86394831/0ddda1d1-67b5-4201-87dd-4b757b5a493a)

# 3. Data Preprocessing

The preprocessing of the text data is an essential step as it makes the raw text ready for mining.

The objective of this step is to clean noise those are less relevant to find the sentiment of tweets such as punctuation, special characters, numbers, and terms which don’t carry much weightage in context to the text.

Stop words are those words in natural language that have a very little meaning, such as "is", "an", "the", etc.To remove stop words from a sentence, you can divide your text into words and then remove the word if it exits in the list of stop words provided by NLTK.

Stemming is a rule-based process of stripping the suffixes (“ing”, “ly”, “es”, “ed”, “s” etc) from a word. For example – “play”, “player”, “played”, “plays” and “playing” are the different variations of the word – “play”.

Lemmatization is a more powerful operation, and it takes into consideration morphological analysis of the words. It returns the lemma which is the base form of all its inflectional forms.

In tokenization we convert group of sentence into token . It is also called text segmentation or lexical analysis. It is basically splitting data into small chunk of words. Tokenization in python can be done by python NLTK library’s word_tokenize() function

**After cleaning text we also create wordblog**

![image](https://github.com/ashishdhawas/Coronavirus-Tweet-Sentiment-Analysis/assets/86394831/76608649-fa2e-4649-843b-83dc0b592ca2)

# 4. Model Training- MULTICLASS AND BINARY.

**Trained 7 different algorithms for each Multiclass and Binary classification. In Multiclass we have 5 different classes but in binary we have only two class i.e. Positive and Negative. The algorithms that were used -**

1. Logistic Regression

2. Support Vector Machine

3. Random Forest

4. Naive Bayes

5. Stochastic Gradient Descent

6. XGBosst

7. CatBoost






