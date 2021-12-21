# Game Reviews Sentiment Analysis

# Abstract
The game industry is projected to grow to 9.64% by 2026 (mordointelligence.com). The exponential growth rate leads to better understanding of gamers need in order to compete in this industry. Therefore, in our project we try to find out which game studio is serving the global gaming community based on the cumulative reviews of their products.

# Research Hypothesis:
In our project, we are trying to identify whether the review made by player is a positive one or negative. In addition, we may find out the worthiness of every game based on our sentiment analysis.

Moreover, negative reviews are segmented aside and to be analyzed for the level of toxicity of every reviewer.

# Data Description
This data has been obtained from [Kaggle](https://www.kaggle.com/najzeko/steam-reviews-2021) originally fetched using SteamAPI. The data is around 21 million records with 23 features (21 million reviews across more than 300 games). The features lists as follow:

|Feature                       |Description|
|------------------------------|-----------|
|app_id                        | AppID of the game|
|app_name                      | name of the game|
|review_id                     | intuitive  |
|language                      | language the user indicated when authoring the review|
|review                        | text-based review|
|timestamp_created             | date the review was created (unix timestamp)|
|timestamp_updated             | date the review was last updated (unix timestamp)|
|recommended                   | whether review recommends the app|
|votes_helpful                 |  the number of users that found this review helpful|
|votes_funny                   |  the number of users that found this review funny|
|weighted_vote_score           |  helpfulness score|
|comment_count                 | number of comments posted on this review|
|steam_purchase                | true if the user purchased the game on Steam|
|received_for_free             | true if the user checked a box saying they got the app for free|
|written_during_early_access   | true if the user posted this review while the game was in Early Access|
|author.steamid                | the user’s SteamID|
|author.num_games_owned        | number of games owned by the user|
|author.num_reviews            | number of reviews written by the user|
|author.playtime_forever       | lifetime playtime tracked in this app|
|author.playtime_last_two_weeks| playtime tracked in the past two weeks for this app |
|author.playtime_at_review     | playtime when the review was written|
|author.last_played            | time for when the user last played|


# Tools
* Python
* Pandas
* Numpy
* Scikit-learn 
* Matplotlib
* Seaborn
