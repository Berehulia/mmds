Final project MMDS - 2025
Analyzy user-movie data stream and build a Hybrid Recommendation System

Data: MovieLens 1M dataset (includes interactions and content details).

Environment: Jupyter/Colab.

Part 1: Streams (20 / 80)
You need to do: You are going to read the user-item data (u.data file) as a stream, line by line. You can't store the lines in memory or on disk. Then: (i) Create a random sample that gets approximately 10% of the movies, and count the approximate number of different users on that stream.

Technologies: Python, you can only import "random" library (no other import is allowed)

Part 2: Recsys (60 / 80)
You need to do: (i) Load, process and prepare the data in Spark, do the basic EDA; (ii) Build a Collaborative Filtering Component (e.g., ALS, etc.); (iii) Build a Content-Based Component (e.g., TFIDF, LSH, etc.); (iv) Build the recommendation fusion strategy; (v) Evaluate the final system and its components separately using Precision@K, Recall@K, and NDCG@K. Additionally evaluate the training and inference time of the system and its components.

Technologies: Apache Spark (PySpark) – mandatory, Spark MLlib – for ALS collaborative filtering, Spark ML feature engineering – TF-IDF, hashing, LSH. You may not use Pandas/Scikit-learn for the main pipeline (should be spark based).

Additional (+5 points):
(i) Implement hyperparameter tuning using MLlib pipelines; (ii) Build the second layer ranking for candidates re-ranking, or custom scoring model as a fusion strategy (e.g., Gradient-Boosted Trees, etc.);