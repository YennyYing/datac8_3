# Movie Text Analysis

## Description
This project analyzes movie plot text by converting each movie’s script into numerical features. We perform text preprocessing, create a word–frequency feature table, and then use these features to explore similarity between movies through Euclidean distances. Several visualizations are included to help interpret patterns in word usage across genres.

## Author
Yuan Ying  

## Date
05/02/2025  

---
## How it is made:
This project converts movie plot summaries into numerical features and uses them to analyze similarity between films.

**1. Text Processing & Stemming**

Plot text is cleaned and stemmed so that different word forms (e.g., running/run/runs) map to a shared root.
This reduces dimensionality and standardizes vocabulary.

**2. Feature Matrix Construction**

Each movie becomes a numeric vector:

First five columns: Title, Year, Rating, Genre, # Words

Remaining columns: proportion of each stemmed word in the movie

This turns unstructured text into a structured dataset suitable for analysis.

**3. Similarity via Euclidean Distance**

We compute movie similarity using a custom distance function applied to the word-proportion features (columns after index 5).
Smaller distances represent more similar plot content.

**4. Visual Exploration**

Plots illustrate word-frequency patterns, genre differences, and movie clusters, helping interpret relationships in the text-derived features.

## Visualizations

The project includes several plots that demonstrate:
- Distribution of word frequencies
- Differences in word usage across genres
- Patterns in high-dimensional feature space

These generated figures help highlight relationships in the text-derived features.

---
## Lessons Learned：
- How to convert text into structured numerical features
- How stemming affects feature creation
- How to compute similarity between movies using Euclidean distance
- How to interpret high-dimensional text data through visualizations
- How text preprocessing affects downstream modeling and analysis


