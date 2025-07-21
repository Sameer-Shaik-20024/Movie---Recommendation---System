# 🎬 CineScope: Movie Recommendation System

## 📌 Objective
This project presents a personalized movie recommendation system using **User-Based Collaborative Filtering (UBCF)**, integrated with an interactive **Shiny web application**. It aims to:

- Deliver accurate movie recommendations based on user preferences
- Evaluate the performance using key recommender metrics
- Provide a dynamic and user-friendly interface for movie discovery

---

## 🧠 Methodology

### 🔹 Data Source
- Dataset: [MovieLens 20M](https://grouplens.org/datasets/movielens/)
- 20 million+ ratings
- Metadata for 27,000+ movies
- Data collected from ~138,000 users

### 🔹 Preprocessing
- Merged `ratings.csv` and `movies.csv` on `movieId`
- Cleaned missing values and duplicates
- Standardized genres and normalized ratings

### 🔹 Collaborative Filtering
- Implemented **User-Based Collaborative Filtering (UBCF)** using:
  - **Pearson Correlation**
  - **Cosine Similarity**
- Predicted scores for unseen movies using a weighted average of ratings from similar users

### 🔹 Custom Weighted Scoring
Final ranking of recommended movies is based on:
- Movie similarity
- Average user ratings
- Number of ratings

---

## 📊 Evaluation

- Train/Test split for performance evaluation
- Metrics used:
  - ✅ Mean Absolute Error (MAE)
  - ✅ Root Mean Squared Error (RMSE)
  - ✅ Precision, Recall, F1 Score

---

## 🖥️ Shiny Web Application

The interactive user interface was built using **R Shiny**, allowing users to:
- Input up to 5 preferred movies
- View recommendations in a **carousel**
- Explore a **pie chart** of top movie ratings
- Reset inputs to personalize results dynamically

---

## 🔍 Key Insights

- The recommender system achieved reliable accuracy and relevance.
- Custom scoring helped avoid bias toward overly popular movies.
- Cold-start and sparsity issues were observed, suggesting hybrid or ML-based enhancements in the future.
- The UI enhanced user engagement with visual feedback and intuitive design.

---
