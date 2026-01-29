# 🎬 Movie Recommendation System
This project implements two collaborative filtering approaches for movie recommendation:
   - K-Nearest Neighbors (KNN) with cosine similarity
   - Matrix Factorization using Singular Value Decomposition (SVD)
Both methods were developed and analyzed independently on a large-scale movie ratings dataset.

## Project Overview
Recommender systems personalize content by learning user preferences from historical data. In this project, I built:
   - A memory-based recommender using similarity search (KNN).
   - A model-based recommender using latent factor modeling (SVD).

## Methodology
1️⃣ KNN + Cosine Similarity (Collaborative Filtering)
   - Represented the user–movie ratings matrix in sparse format.
   - Used cosine similarity to measure closeness between users or items.
   - Applied KNN to retrieve the most similar movies or users.
2️⃣ SVD (Latent Factor Model)
   - Decomposed the user–movie ratings matrix into latent user and movie embeddings.
   - Learned hidden factors that explain user preferences and movie characteristics.
   - Used the reconstructed matrix for rating prediction and recommendations.

## Dataset
- Dataset: MovieLens (100k+ ratings)
- Fields: userId, movieId, rating, timestamp

## Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- SciPy
- Jupyter Notebook

## Example Output
Sample KNN-based recommendations:

Sample SVD-based recommendations:
