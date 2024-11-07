# Recommendation System 
This repository demonstrates various types of recommendation systems using both Collaborative Filtering and Content-Based Filtering. The project includes user-based collaborative filtering, item-based collaborative filtering, matrix factorization techniques like SVD (Singular Value Decomposition) and NMF (Non-negative Matrix Factorization), as well as a content-based recommendation system.

## Project Overview
Recommendation systems are used to predict the preferences or ratings that a user would give to an item. They are widely used in platforms like Netflix, Amazon, and Spotify to recommend movies, products, or music. This project showcases multiple approaches to building a recommendation system:

## 1. Collaborative Filtering (CF)
  
### 1.1 Collaborative Filtering
<li><b>User-Based Collaborative Filtering:</b> 
<li><b>Item-Based Collaborative Filtering:</b> 
<li>Implemented with KNNBasic, KNNWithMeans, and KNNBaseline from the surprise library.

### 1.2 Matrix Factorization
<li><b>SVD (Singular Value Decomposition):</b> 
<li><b>NMF (Non-negative Matrix Factorization):</b> 
<li>Both algorithms are implemented using the surprise library.

## 2. Content-Based Filtering
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
