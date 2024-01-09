# Movie Recommendation System

This repository contains the code for a movie recommendation system that suggests movies based on genre, keywords, and production details.

![recommendation](https://github.com/SimoneParvizi/Recomendation-system/assets/75120707/ae8642d6-3012-4c6d-b110-20c408b65c72)


## Overview

The recommendation system uses a content-based filtering approach. It analyzes the genres, keywords, production companies, cast, and production countries of movies to find similarities and make recommendations.

## Features

- **Content-based Filtering**: Recommendations are based on movie content.
- **Two Aspects of Similarity**:
  - Genre and Keywords Similarity
  - Production and Casting Similarity

## How It Works

The system creates TF-IDF vectors for two aspects: 'genre_keywords_similarity' and 'production_casting_similarity'. It then computes the cosine similarity of these vectors with all movies in the dataset to find the most similar movies.

## Usage
To use the recommendation system, call the `recommendation` function with the title of the movie
The function will output two lists of recommended movies:

    Based on genre and keywords.
    Based on production companies and casting.

```python
recommendation('Movie Title')
