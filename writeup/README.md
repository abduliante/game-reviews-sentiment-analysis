# Game Reviews Sentiment Analysis

# Abstract

In our project, we seek to identify profanity based on negative portion of reviews. Data is originally collected using Steam API but fetched from [Kaggle](https://www.kaggle.com/najzeko/steam-reviews-2021). Profanity labels where made and logistic regression model outperformed all others.

## Design: 

Labeling profanity using profanity predefined list. This might help in implementing profanity filtering in game lobbies or restrict view to underaged person.

## Data:

Our dataset is very huge consists of 21 million records with rows and 23 columns. Approximately 55% of data are in other languages so we are not concerned about it. Out of the rest 45%, negative reviews only subsetted to perform profanity labeling.
Preprocessing took place in before our modeling where we removed punctuations, lowering text, removing numbers and etc...

## Algorithms

* Labeling:

1. All of the profanity were labeling approperiatly

* Feature Engineering:

1. (NOT COMPLETED YET) In the recommendation system, we decided to use collaborative filtering engine. Yet, we don't have ratings of users so we decided to "assume" rating of users based on their median playtime.

* Tokenization:

Tokenaziation is done using both Count Vectorizer and TF-IDF; in addition to being unigram and bigram. Count Vectorizer using unigram yielded the best results.

* Models:

Logistics regression, Naive Bayes Bernoulli, Naive Bayes Multinomial 

Logistics regression yielded the best results.

* Model evaluation and selection:

Data is splitted into train, validation, testing. Scores reported as follow:


|Split|Precision                    |Recall|F1-score                                     |Accuracy|
|-----|-----------------------------|------|---------------------------------------------|--------|
|Training|0.98                         | 0.98 | 0.98                                        | 0.98   |
|Validation|0.95                         |0.86  |0.90                                         |0.96    |
|Test | 0.94                        |0.85  |0.89                                         |0.95    |

## Logistics Regression Confusion Matrix

![image](https://user-images.githubusercontent.com/49822946/147753096-ea070712-a9c8-4fc1-8a6d-3674f27ff21c.png)


# Tools 
* Pandas and Numpy for data manipulation
* better-profanity 
* Scikit-learn for modeling
* Matplotlib, Seaborn for data visualization
* Pickle
* Flask

# Communication
Along with slides, our model is deployed on heroku and can be found [here](HEROKU LINK)
