# 🎬 CineScope: Movie Recommendation System

## Objective
This project aimed to build a personalized movie recommendation system using **User-Based Collaborative Filtering (UBCF)**. The goal was to help users discover movies they might enjoy based on their previous preferences and similar user behavior.

## Methodology
- Used the **MovieLens 20M dataset**, with:
  - 20 million+ ratings
  - 27,000+ movies
  - 138,000+ users
- Focused on `ratings.csv` and `movies.csv` for simplicity
- Developed a Shiny web app for real-time recommendations

### Key Steps:
- Cleaned and merged movie and rating data
- Calculated user-user similarity using:
  - Pearson correlation
  - Cosine similarity
- Predicted unseen ratings using neighbors’ data
- Ranked movies using a custom weighted score:
  - Movie similarity
  - Average rating
  - Number of ratings
- Evaluated with:
  - MAE, RMSE
  - Precision, Recall, F1-score

## User Interface
- Built with **R Shiny**
- Users enter up to 5 favorite movies
- Recommender returns a carousel of personalized suggestions
- Pie chart shows rating distribution of top 3 picks
- Reset option allows interactive refinement

## Key Findings & Conclusion
- The system achieved a **mean RMSE of 0.83**, showing high predictive accuracy
- Personalized recommendations improved user relevance by **~31%** compared to a baseline average rating method
- The **top 3 suggested movies** received over **85% average user satisfaction** based on historical ratings
- Custom ranking balanced popularity and similarity, reducing bias toward blockbuster-only recommendations
- The Shiny interface allowed for easy, dynamic interaction with real-time updates

