# Recommendation System 
This repository demonstrates various types of recommendation systems using both Collaborative Filtering and Content-Based Filtering. The project includes user-based collaborative filtering, item-based collaborative filtering, matrix factorization techniques like SVD (Singular Value Decomposition) and NMF (Non-negative Matrix Factorization), as well as a content-based recommendation system.

## Project Overview
Recommendation systems are used to predict the preferences or ratings that a user would give to an item. They are widely used in platforms like Netflix, Amazon, and Spotify to recommend movies, products, or music. This project showcases multiple approaches to building a recommendation system:

## Collaborative Filtering (CF)
<li>User-Based Collaborative Filtering: Recommendations based on the preferences of similar users.
<li>Item-Based Collaborative Filtering: Recommendations based on the similarity between items (books, movies, etc.).
<li>Matrix Factorization: Techniques like Singular Value Decomposition (SVD) and Non-negative Matrix Factorization (NMF) to discover latent factors behind ratings.
Content-Based Filtering: Recommendations based on the features of the items themselves, such as the genre, keywords, etc.
Algorithms Used
## 1. Collaborative Filtering
<li><b>User-Based Collaborative Filtering:</b> This method computes the similarity between users and recommends items based on the preferences of similar users.
<li><b>Item-Based Collaborative Filtering:</b> This method computes the similarity between items, recommending items that are similar to what the user has rated highly.
<li>Implemented with KNNBasic, KNNWithMeans, and KNNBaseline from the surprise library.

## 2. Matrix Factorization
<li><b>SVD (Singular Value Decomposition):</b> A matrix factorization technique that reduces the dimensionality of the user-item interaction matrix and captures latent factors.
<li><b>NMF (Non-negative Matrix Factorization):</b> A variant of matrix factorization that imposes non-negativity constraints, making it interpretable for some datasets.
<li>Both algorithms are implemented using the surprise library.

## 3. Content-Based Filtering
<li>A simple content-based recommender can be built based on item features such as genre, description, etc. In this case, book titles and authors are used as features.
Installation

Dataset
This project uses a book dataset containing user ratings, book titles, and book authors. You can replace the dataset with any other that fits the requirements for building recommendation systems. The dataset should have the following columns:


## Evaluation
Each algorithm was evaluated using two common metrics in recommendation systems:
<li>RMSE (Root Mean Squared Error)
<li>MAE (Mean Absolute Error)
<li>These metrics help evaluate how well the model predicts ratings for unseen items. Cross-validation was used to assess performance across multiple splits of the dataset.


## Hyperparameter Tuning
Hyperparameter tuning was performed using GridSearchCV to find the best parameters for the models. The following parameters were tuned:
<li>k (Number of Neighbors) for KNN-based models
<li>n_factors (Number of Latent Factors) for Matrix Factorization models
<li>n_epochs (Number of Training Epochs) for Matrix Factorization models
  
## Results
The performance of each algorithm was evaluated before and after hyperparameter tuning. The results showed improvements in the accuracy of the models after tuning, as measured by RMSE and MAE.
