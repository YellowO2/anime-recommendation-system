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

- Data preparation and cleaning
- Exploratory data analysis and visualization
- Collaborative filtering model training
- Content-based filtering model training\
- Passing in an anime and finding recommendations

## Configuration

Explain any configuration options or settings that users can adjust, such as dataset paths, model hyperparameters, etc.

## Contributing

Encourage contributions from other developers and provide guidelines for submitting bug reports, feature requests, and pull requests.

## License

Specify the license under which your project is distributed, along with any relevant terms and conditions.

## Authors

List the authors or contributors to the project, along with their roles and contributions.

## Acknowledgements

Thank any individuals or organizations that have contributed to or supported the project in any way.

## Changelog

Document the changes and updates made to the project over time, including version numbers, dates, and descriptions of changes.

## Support

Provide information on how users can seek support or assistance with the project, including links to documentation, forums, or contact information.