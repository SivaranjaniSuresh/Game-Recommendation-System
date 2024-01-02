# Game-Recommendation-System

## Game Recommendations on Steam 🎮

## Overview

Welcome to the "Game Recommendations on Steam" project repository! 🚀 This project aims to elevate your gaming experience on the Steam platform by providing personalized game recommendations. Leveraging collaborative filtering, content-based filtering, and hybrid models, we're here to deliver accurate and diverse suggestions tailored to your gaming preferences. 🕹️

## Datasets 📊

The project relies on three key datasets:

1. **games.csv:** Comprehensive game and add-on information.
2. **users.csv:** Public user profiles data.
3. **recommendations.csv:** Captures user reviews and recommendations.

## Data Modeling 🤖

### Collaborative Filtering Techniques

1. **Singular Value Decomposition (SVD) Algorithm:** Decomposes the user-item interaction matrix into three matrices representing users, latent factors, and items.

2. **Slope One Collaborative Filtering:** Predicts user preferences based on the average difference in ratings between items.

3. **Item-Based k-NN Collaborative Filtering:** Computes similarities between items and predicts user preferences.

4. **Alternating Least Squares (ALS) Collaborative Filtering:** Factorizes the user-item matrix by alternating between fixing users' and items' factors.

5. **Non-Negative Matrix Factorization (NMF) Collaborative Filtering:** Approximates the user-item matrix as the product of two non-negative matrices.

6. **BaselineOnly Collaborative Filtering:** Predicts ratings based on baseline estimates, considering biases associated with users and items.

### Content Filtering Technique

1. **TF-IDF Based Content Filtering:** Computes the similarity between items based on the words present in their titles.

## Hybrid Model 🔄

1. **Ensemble Model:** Combines predictions from multiple models (SVD and k-NN) using a simple average (voting) to enhance recommendation accuracy.

## User Recommendations 🌟

For each model, a handy function (`get_top_n_recommendations`) is provided to snag top N recommendations for a specific user.

## Fairness-Bias Aware Recommendation System 🤝

In addition to collaborative and content-based recommendation techniques, our project incorporates fairness-aware methodologies using the AIF360 library. The goal is to mitigate potential biases in the recommendation system and ensure equitable treatment across different user groups.

## Data Sparsity and Cold Start ❄️

### Data Sparsity

- **Matrix Factorization (SVD):** Effectively handles sparse matrices by decomposing the user-item interaction matrix.

- **Content-Based Filtering:** Utilizes item features and user preferences to enhance recommendations, especially when there are few interactions.

### Cold Start

- **Content-Based Filtering for New Items:** Provides recommendations based on the features of the item itself, addressing the cold start problem for new items.

- **Hybrid Models:** Combining collaborative filtering and content-based filtering in hybrid models provides a balance for both data sparsity and the cold start problem.

- **Popularity-Based Recommendations:** For new users or users with very few interactions, providing recommendations based on the popularity of items can be a simple yet effective strategy.

## Conclusion 🎉

Explore and experiment with different recommendation techniques in this repository. Feel free to contribute, report issues, or suggest improvements. Happy gaming and coding! 🚀🎮

Data Sparsity
Matrix Factorization (SVD): Effectively handles sparse matrices by decomposing the user-item interaction matrix.
Content-Based Filtering: Utilizes item features and user preferences to enhance recommendations, especially when there are few interactions.
Cold Start
Content-Based Filtering for New Items: Provides recommendations based on the features of the item itself, addressing the cold start problem for new items.
Hybrid Models: Combining collaborative filtering and content-based filtering in hybrid models provides a balance for both data sparsity and the cold start problem.
Popularity-Based Recommendations: For new users or users with very few interactions, providing recommendations based on the popularity of items can be a simple yet effective strategy.
Conclusion

Explore and experiment with different recommendation techniques in this repository. Feel free to contribute, report issues, or suggest improvements. Happy gaming and coding!
