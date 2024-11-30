Recommendation System for Movies Using Collaborative FilteringProject Details:

This project builds a movie recommendation system based on user ratings, employing collaborative filtering and bipartite graph visualization to
suggest movies to users. The goal is to recommend top movies by analyzing user ratings and their similarity to other users (user based collaborative
filtering).

Key objectives include recommending movies to users based on similarities between users, using collaborative filtering to predict ratings for unrated movies by leveraging similar users' ratings and visualizing user-movie interactions using a bipartite graph to enhance the understanding of relationships.

Summarized Project:
Concepts & techniques used were Collaborative Filtering where we identified similar users (user-user similarity) to make recommendations. Cosine 
similarity was used to calculate the similarity between users based on their ratings. Bipartite Graph edges were formed based on user-movie 
interactions, with edge weights indicating the predicted ratings and original ratings.

The movie recommendation system begins with data preprocessing, where duplicate ratings for the same user-movie pair are averaged. The dataset 
is split into training (70%) and testing (30%) subsets using Scikit-learn's train_test_split. The training data is used to construct a user-movie
matrix, where entries indicate whether a user has rated a movie, with ratings above zero marked as "watched" (1). To measure user similarity, a 
user-user cosine similarity matrix is computed, quantifying how similar users are based on their ratings. Unrated movies are predicted using the
ratings of similar users, excluding movies the user has already rated. A bipartite graph is created in NetworkX, with users as one set of nodes 
and movies as the other. Edges represent predicted ratings, with weights indicating the strength of the recommendation. This graph is visualized
to highlight user-movie interactions, user-user similarity, and movie recommendations. The system generates top movie recommendations for each
user based on their ratings and the similarity to other users, improving the recommendation process with the bipartite graph visualization.
