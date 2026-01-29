## 🎬 Movie Recommendation System
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
   - Recommended top-N similar movies for a given title.
     
2️⃣ SVD (Latent Factor Model)
   - Factorized the user–movie rating matrix into user and movie embeddings.
   - Predicted ratings for unseen movies.
   - Recommended movies with the highest predicted ratings.

## Dataset
- Movies (movies.csv): movieId, title, genres
- Ratings (ratings.csv): userId, movieId, rating, timestamp
- Fields: userId, movieId, rating, timestamp

## Example Output
Sample KNN-based recommendations:

| Rank | Title                          | Distance |
| ---- | ------------------------------ | -------- |
| 1    | Avengers, The (2012)           | 0.285319 |
| 2    | Dark Knight, The (2008)        | 0.285835 |
| 3    | WALL·E (2008)                  | 0.298138 |
| 4    | Iron Man 2 (2010)              | 0.307492 |
| 5    | Avatar (2009)                  | 0.310893 |
| 6    | Batman Begins (2005)           | 0.362759 |
| 7    | Star Trek (2009)               | 0.366029 |
| 8    | Watchmen (2009)                | 0.368558 |
| 9    | Guardians of the Galaxy (2014) | 0.368758 |
| 10   | Up (2009)                      | 0.368857 |

Sample SVD-based recommendations:

| Rank | Title                        | Similarity |
| ---- | ---------------------------- | ---------- |
| 1    | WALL·E (2008)                | 0.891437   |
| 2    | Avatar (2009)                | 0.887909   |
| 3    | Star Trek (2009)             | 0.883988   |
| 4    | Sherlock Holmes (2009)       | 0.858885   |
| 5    | District 9 (2009)            | 0.857971   |
| 6    | Up (2009)                    | 0.849528   |
| 7    | Dark Knight, The (2008)      | 0.842004   |
| 8    | Avengers, The (2012)         | 0.836555   |
| 9    | Kung Fu Panda (2008)         | 0.827870   |
| 10   | Bourne Ultimatum, The (2007) | 0.814532   |

## Future Improvements
- Combine KNN + SVD into a hybrid recommender for better accuracy.

## Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- SciPy
- Jupyter Notebook
