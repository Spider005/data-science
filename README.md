Project: **Movie recommendations**

Recommendation systems are becoming increasingly important in today’s extremely busy world. People are always short on time with the myriad tasks they need to accomplish in the limited 24 hours. Therefore, the recommendation systems are important as they help them make the right choices, without having to expend their cognitive resources.

The purpose of a recommendation system basically is to search for content that would be interesting to an individual. Moreover, it involves a number of factors to create personalised lists of useful and interesting content specific to each user/individual. Recommendation systems are Artificial Intelligence based algorithms that skim through all possible options and create a customized list of items that are interesting and relevant to an individual.

Types of Recommendation System :
1 ) Content Based :
Content-based systems, which use characteristic information and takes item attriubutes into consideration .

Twitter , Youtube .

Which music you are listening , what singer are you watching . Form embeddings for the features .

User specific actions or similar items reccomendation .

It will create a vector of it .

These systems make recommendations using a user's item and profile features. They hypothesize that if a user was interested in an item in the past, they will once again be interested in it in the future

One issue that arises is making obvious recommendations because of excessive specialization (user A is only interested in categories B, C, and D, and the system is not able to recommend items outside those categories, even though they could be interesting to them).

2 ) Collaborative Based :
Collaborative filtering systems, which are based on user-item interactions.

Clusters of users with same ratings , similar users .

Book recommendation , so use cluster mechanism .

We take only one parameter , ratings or comments .

In short, collaborative filtering systems are based on the assumption that if a user likes item A and another user likes the same item A as well as another item, item B, the first user could also be interested in the second item .

Issues are :

User-Item nXn matrix , so computationally expensive .

Only famous items will get reccomended .

New items might not get reccomended at all .

3 ) Hybrid Based :
Hybrid systems, which combine both types of information with the aim of avoiding problems that are generated when working with just one kind.

Combination of both and used now a days .

Uses : word2vec , embedding .

About this project:
This is a streamlit web application that can recommend various kinds of similar movies based on an user interest. here is a demo,

Click here to run it live on server
Demo:
workflow

workflow

workflow

Dataset has been used:
Dataset link
Concept used to build the model.pkl file : cosine_similarity
1 . Cosine Similarity is a metric that allows you to measure the similarity of the documents.

2 . In order to demonstrate cosine similarity function we need vectors. Here vectors are numpy array.

3 . Finally, Once we have vectors, We can call cosine_similarity() by passing both vectors. It will calculate the cosine similarity between these two.

4 . It will be a value between [0,1]. If it is 0 then both vectors are complete different. But in the place of that if it is 1, It will be completely similar.


Objectives :
All entertainment websites or online stores have millions/billions of items. It becomes challenging for the customer to select the right one. At this place, recommender systems come into the picture and help the user to find the right item by minimizing the options.

Recommendation Systems in the world of machine learning have become very popular and are a huge advantage to tech giants like Netflix, Amazon and many more to target their content to a specific audience. These recommendation engines are so strong in their predictions that they can dynamically alter the state of what the user sees on their page based on the user’s interaction with the app.

The business objective for us is:

To create a Collaborative Filtering based Movie Recommendation System
Predict the rating that a user would give to a movie that he has not yet rated
Minimize the difference between predicted and actual rating (RMSE and MAPE)
Data Collection :
The dataset has been obtained from Grouplens.

Link : https://grouplens.org/datasets/movielens/20m/

This dataset (ml-20m) describes 5-star rating and free-text tagging activity from MovieLens, a movie recommendation service. It contains 20000263 ratings and 465564 tag applications across 27278 movies. These data were created by 138493 users between January 09, 1995 and March 31, 2015. This dataset was generated on October 17, 2016.

Users were selected at random for inclusion. All selected users had rated at least 20 movies. No demographic information is included. Each user is represented by an id, and no other information is provided.

The data are contained in the files genome-scores.csv, genome-tags.csv, links.csv, movies.csv, ratings.csv and tags.csv.

For our objective, we would be using "ratings.csv" and "movies.csv" data files.

Modelling :
The following modelling approach was used in the project:

Loading & exploring the Movie and User ratings data
Creating User-Item Matrix, User-User and Item-Item similarity matrices for Movie Recommendations
Creating feature and applying ML models to predict the ratings for unseen movies for a user
The detailed analysis and model creation can be found in the .ipynb file.

Resul
![M_1](https://github.com/user-attachments/assets/7bee12e6-7be4-48a8-8863-6f81521bbe69)
t :

Some of the test images are given below.
![M_2](https://github.com/user-attachments/assets/323d2e9c-0f53-45b8-84bd-09edb82db278)

The results from Movie-Movie Similarity is as below:
![M_3](https://github.com/user-attachments/assets/2ebf7f97-a1a4-4ee9-a1d6-ec3c932b42ad)

test

The results from User-User Similarity is as below:

test
![image](https://github.com/user-attachments/assets/01646c0e-df5c-4372-9608-10d593c5aa86)


The Feature Importance for predicting ratings is as below:

![M_4](https://github.com/user-attachments/assets/399c8660-5646-4f76-b6da-86e468f9d18e)

test

The results from different ML models are as follows:

![M_5](https://github.com/user-attachments/assets/a4ab99dd-8a3a-4768-8820-93d78041b944)

test

The sample movie recommendation based on Collaborative Filtering is as follows:

test

Conclusions :
In this project, we learned the importance of Recommendation Systems, the types of recommender systems being implemented, and how to use matrix factorization to enhance a system.

We then built a movie recommendation system that considers user-user similarity, movie-movie similarity, global averages and matrix factorization. These concepts can be applied to any other user-item interactions systems.

We tried generating recommendations based on similarity matrix and Collaborative Filtering techniques.

We tried to predict the ratings for movies that the user might give based on its past rating behaviours and measure the accuracy using RMSE and MAPE error metrics.

Surely, there is huge scope of improvement and tring out different techniques and ML/DL algorithms.
