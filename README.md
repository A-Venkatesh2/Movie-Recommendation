# Movie Recommendation

A Jupyter Notebook project that builds and evaluates multiple movie recommendation approaches using a large IMDB/TMDB metadata dataset.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Requirements](#requirements)
- [Usage](#usage)
- [Notebook Contents](#notebook-contents)
- [Notes](#notes)

## Overview

This project shows how different recommendation methods can be combined in a single workflow. The notebook loads movie metadata, preprocesses text and categorical features, and builds:

- content-based recommendations using TF-IDF and cosine similarity
- personalized filtering by genre, actor, director, language, and rating
- mood-based genre suggestions
- association-rule recommendations using FP-Growth
- rating category prediction via Naive Bayes and Logistic Regression

## Features

- Text preprocessing from movie overview, genres, cast, director, composer, and original language
- Content similarity recommendations for movie titles
- User preference filtering and mood-based recommendations
- Basket-style recommendations using association rules
- Classification models to predict movie rating categories
- Export of trained models and data artifacts as `.pkl` files

## Dataset

The notebook uses an IMDB/TMDB movie metadata dataset with movie titles, genres, cast, director, ratings, and summaries. It also creates a final rating column from available rating fields and filters movies by language.

## Requirements

The notebook may require the following Python packages:

- `pandas`
- `scikit-learn`
- `imbalanced-learn`
- `mlxtend`
- `joblib`
- `kagglehub`

## Usage

1. Open `movie_recommendation.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
2. Install the required packages if needed.
3. Run the notebook cells in order to preprocess the dataset and run the recommendation methods.

## Notebook Contents

The notebook includes sections for:

- data loading and preprocessing
- TF-IDF vectorization and cosine similarity
- recommendation functions and tests
- mood-based recommendations
- FP-Growth association rules
- classification of movie rating categories
- model export to `.pkl` files
