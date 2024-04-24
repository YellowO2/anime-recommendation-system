# Anime Recommendation System

## Overview

This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence). Our project aims to develop a recommendation system for anime enthusiasts, leveraging machine learning techniques to recommend anime you might enjoy based on your preferences.

## Problem Definition

The anime industry has boomed in recent years, with new shows every season. This abundance of content makes it challenging to find hidden gems that resonate with your taste. Our recommendation system aims to address this challenge.

## Project Files

* **Data Preparation & Cleaning.ipynb**: Jupyter Notebook for preparing and cleaning the anime dataset.
* **Exploratory Data Analysis & Visualization.ipynb**: Jupyter Notebook for exploring and visualizing the anime dataset.
* **Model Training Collaborative Filtering.ipynb**: Jupyter Notebook for training the collaborative filtering model.
* **Model Training Content-Based Filtering.ipynb**: Jupyter Notebook for training the content-based filtering model.

## Dataset

* **anime_info_2020.csv** ([anime_info_2020](https://www.kaggle.com/datasets/marlesson/myanimelist-dataset-animes-profiles-reviews?select=animes.csv)): A list of animes up to 2020.
* **anime_review_2020.csv** ([anime_review_2020](https://www.kaggle.com/datasets/marlesson/myanimelist-dataset-animes-profiles-reviews?select=reviews.csv)): Reviews of the anime_info_2020 anime.
* **anime-dataset-2023.csv** ([anime_info](https://www.kaggle.com/datasets/dbdmobile/myanimelist-dataset?select=anime-dataset-2023.csv)): A list of animes up to 2023 (used to fill NaN values).

## Installation

You may need to install `scikit-surprise` before running the code:


```
!pip install scikit-surprise
```

## Features

* Data preparation and cleaning
* Exploratory data analysis and visualization
* Collaborative filtering model training
* Content-based filtering model training
* Recommending anime based on a user's input

## Contributors

1. @YellowO2 (Yuxuan)
2. @JianAn-S (Jian An)
3. @mayukhii (Mayukhi)

## Conclusion

Collaborative filtering surpasses content-based filtering by uncovering deeper connections between users and anime, leading to more in-depth recommendations beyond a simple word search.

## Key Learning Points

* Data cleaning techniques (handling NaN values, duplicates, etc.)
* K-nearest neighbors (KNN), Term Frequency-Inverse Document Frequency (TF-IDF), and Cosine Similarity concepts
* Python libraries for collaborative filtering and nearest neighbor algorithms
* Evaluating recommendations using Hit Rate at K
* User-item matrix creation
* New data visualization methods (word cloud)

## Brief Process Walkthrough (In Order)

1. [Data Preparation & Cleaning](<Data Preparation & Cleaning.ipynb>)
   * Clean Anime Info Dataset:
      * Remove duplicate rows.
      * Drop variables like 'ranked', 'img_url', and 'link'.
      * Handle NaN values by:
         * Dropping anime not yet aired.
         * Dropping anime without reviews.
         * Filling NaN values using the 2023 anime dataset.
         * Dropping anomalies.
   * Clean Anime Review Dataset:
      * Remove duplicate rows.
      * Drop variables like 'text', 'uid', and 'link'.

2. [Exploratory Data Analysis](<Exploratory Data Analysis & Visualization.ipynb>)
   * Anime Info Dataset EDA:
      * Barplot of Top 10 anime based on popularity.
      * Wordcloud of genres.
      * Barplot of genres.
      * Barplot of Top 10 genres based on MyAnimeList score.
      * Score distribution for anime with scores from MAL (violin plot, histogram, and boxplot).
      * Correlation matrix.
      * Pairplot.
   * Anime Review Dataset EDA:
      * Barplot of Top 10 anime based on user ratings.
      * Score distribution for anime with scores from user rating (violin plot, histogram, and boxplot).
      * Scatterplot of mean rating against aired year.

3. [Model Training: Content-Based](<Model Training Content-Based Filtering.ipynb>)
   * Similarity Calculation: Calculate cosine similarity between content.
   * Recommendation Generation: Generate recommendations using similarity rating.

4. [Model Training: Collaborative Filtering](<Model Training Collaborative Filtering.ipynb>)
   * Collaborative filtering comes in two forms:
      * **User-based:** Recommends items by finding similar users and suggesting items they liked.
      * **Item-based:** Recommends items similar to those the user has shown interest in (based on user interactions, not content).
   * **Interacting with the recommender:** Allow users to input an anime to get recommendations.

## References

* [Anime Recommendation Engine - Content & Collaborative Filtering](https://medium.com/analytics-vidhya/anime-recommendation-engine-content-collaborative-filtering-c6e69be29d29)
* [Movie Analysis - Collaborative Filtering with Surprise](https://github.com/nicklimmm/movie-analysis/tree/main)
