# RecommendationSystem

Movie recommendation system is created based on IMDB dataset with the following approaches:
1. **IMDB's weighted rating formula** for a movie based on existing movie rating and number of votes received
2. **Popularity** metric for a movie given in the dataset
3. **Content Based Filtering** based on movie overview, cast, crew, keywords and genres
4. **Collaborative Filtering** (CF) using **Singular Value Decomposition** of individual user rating on different movies

In content based filtering, **cosine similarity** among movies are obtained based on these contents.
CF was done using the **Surprise** package on small_rating dataset. It is the most preferred method for a movie or any other recommendation which is not dependent on one or two single factors. Small RMSE (root mean square error) or MAE (mean absolute error) defines good recommendation. 

Dataset: https://grouplens.org/datasets/movielens/100k/

This work is based on the [Kaggle kernel by Ibtesam Ahmed and few others](https://www.kaggle.com/ibtesama/getting-started-with-a-movie-recommendation-system), [Medium article by Den Sublett](https://towardsdatascience.com/beginners-recommendation-systems-with-python-ee1b08d2efb6) and [article on Analyticsvidya by Pulkit Sharma](https://www.analyticsvidhya.com/blog/2018/06/comprehensive-guide-recommendation-engine-python/). Thanks to them in particular and many others.
