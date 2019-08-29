# RecommendationSystem

Movie recommendation system is created based on IMDB dataset with the following approaches:
1. Using IMDB's weighted rating formula for a movie based on existing movie rating and number of votes received
2. Using **popularity** metric for a movie
3. Content Based Filtering based on movie overview, cast, crew, keywords and genres
4. Collaborative Filtering (CF) using **Singular Value Decomposition** of individual user rating on different movies

In content based filtering, **cosine similarity** among movies are obtained based on these contents.
CF was done using the **Surprise** package on small_rating dataset. It is the most preferred method for a movie or any other recommendation which is not dependent on one or two single factors. Small RMSE (root mean square error) or MAE (mean absolute error) defines good recommendation. 

Dataset: https://grouplens.org/datasets/movielens/100k/
