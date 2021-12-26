# Game Reviews Sentiment Analysis

In our project, we envoked 2 approaches; supervised and unsupervised learning. In the supervised learning approach, we used the "recommended" column(which is a button that the user clicks) that tells us whether the reviewer recommends (positive review), or not (negative review). On the other hand, in the unsupervised learning, we used Kmeans clustering of 2 to identify 2 clusters while SVD assuming that they are (positive, negative) as well to ensure that the reviewer did not cast their review wrongfully. All of the two approaches were done using Counter Vectorizer document matrix.


## Supervised learning

Our approach goes as follow:

* Preprocessing
* Vectorization
* Modeling

Running logistics regression and naive bayes algorithms yields these results:


||LogReg                       |NB    |
|------|-----------------------------|------|
|Accuracy|0.928                        |0.923 |
|Precision|0.935                        |0.948 |
|Recall|0.987                        |0.966 |
|F1 Score|0.960                        |0.957 |


#### Confusion matrix:

![confmatrix](https://user-images.githubusercontent.com/49822946/147419346-b5633446-89e8-43a5-9825-b77989a35aa9.png)



## Unsupervised learning

We were able to at least cluster the positive reviews by applying SVD algorithm. 

#### Review topic matrix:

![image](https://user-images.githubusercontent.com/49822946/147419374-8970211b-8894-4742-9b42-23f585fb8743.png)

