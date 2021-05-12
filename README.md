# Netflix-Recommendation-System
Recommendation System from Netflix Prize dataset, using famous SVD algorithm from scikit-learn surprise module for millions of users.

# Netflix
Netflix is the world's leading streaming entertainment service with 100s of millions paid customers worldwide.

# Problem Statement
Netflix kind of content platforms will definitely have a huge content library of waste variety, so some users will often face difficulties to find out content of their likelihood. That's where the role of recommender systems comes into play. Recommender system will automatically sort a high quality content with best relevance to user's likelihood preferences, that leads to better user experience success.

# Dataset
This dataset was made public by Netflix for recommendation system competition. This dataset contains more than 17K titles and more than 100M of user ratings.
Netflix Prize data https://www.kaggle.com/netflix-inc/netflix-prize-data

# Preprocessing
In this recommendation system time stamp is not used to fit the data to algo within a limitation of VM instance of notebook. Userid, Movieid, Rating is used. In preprocessing of dataset easiest method chosen to feed this dataframe to SVD, this method is pandas ffill method. Less active users data also dropped. Less popular movies data was also dropped.

# Model
Algorithm SVD was used from scikit surprise. Fit time in this algorithm is around 90m for first 24M user rating data, here 24M users only due to instance limitation.

# Predictions
User Defined Function to predict recommendation for user by entering user id, returns list of all titles sort by descending order for estimated rating by user on each movie.

# Reference
1. Adopted method from most upvoted kernel for this dataset on kaggle, and made change in preprocessing for short route. Less popular movie and less active user threshold to give more high quality recommendations to users.
https://www.kaggle.com/laowingkin/netflix-movie-recommendation
2. It is the most upvoted kernel on EDA on this dataset, referred for EDA if needed.
https://www.kaggle.com/morrisb/how-to-recommend-anything-deep-recommender
