# Netflix Recommendation System
Recommendation System from Netflix Prize dataset, using famous SVD algorithm from scikit surprise module for millions of users.

# Netflix
Netflix is the world's leading streaming entertainment service with 100s of millions paid customers worldwide.

# Problem Statement
Netflix kind of content platforms will definitely have a huge content library of waste variety, so some users will often face difficulties to find out content of their likelihood. That's where the role of recommender systems comes into play. Recommender system will automatically sort a high quality content with best relevance to user's likelihood preferences, that leads to better user experience success.

# Dataset
This dataset was made public by Netflix for recommendation system competition. This dataset contains more than 17K titles and more than 100M of user ratings.
Netflix Prize data: https://www.kaggle.com/netflix-inc/netflix-prize-data

# Preprocessing
In this recommendation system time stamp is not used to fit the data to algo within a limitation of VM instance of notebook. Userid, Movieid, Rating is used. In preprocessing of dataset easiest method chosen to feed this dataframe to SVD, this method is pandas ffill method. 
Less active users data also dropped, less popular movies data was also dropped which leads to need of less computing power and its other benefit is more high quality recommendations to user also.

# Model
Algorithm SVD was used from scikit surprise. Fit time in this algorithm is around 90m for first 24M user rating data, here 24M users ratings only due to instance limitation.

# Predictions
User Defined Function to predict recommendation for user by entering user id, returns list of all titles sort by descending order for estimated rating by user on each movie.

![Recommendation to user](https://user-images.githubusercontent.com/75474944/117961104-5c6cab00-b33b-11eb-94d8-8fbf10b3dbe3.PNG)
