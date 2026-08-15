# Netflix Movies and TV Shows - Exploratory Data Analysis

## Overview

This project performs an Exploratory Data Analysis (EDA) on the Netflix Movies and TV Shows dataset available on Kaggle. The analysis focuses on understanding Netflix content distribution, release trends, ratings, genres, countries, and content growth over time.

The project uses Python libraries for data cleaning, visualization, and analysis to uncover useful insights about Netflix’s global streaming catalog.

Dataset Source: [Netflix Movies and TV Shows Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows?utm_source=chatgpt.com)

---

# Objectives

* Analyze the distribution of Movies and TV Shows
* Explore content trends over the years
* Identify top contributing countries
* Analyze ratings and genre distribution
* Understand Netflix content growth
* Perform data cleaning and preprocessing
* Create visualizations for better insights

---

# Tools & Technologies Used

## Programming Language

* Python

## Environment

* Jupyter Notebook

## Python Libraries

* NumPy
* Pandas
* Matplotlib
* Seaborn

---

# Dataset Information

The dataset contains information about Netflix titles including:

| Column Name  | Description              |
| ------------ | ------------------------ |
| show_id      | Unique ID for each title |
| type         | Movie or TV Show         |
| title        | Name of the title        |
| director     | Director name            |
| cast         | Actors/Actresses         |
| country      | Country of origin        |
| date_added   | Date added to Netflix    |
| release_year | Release year             |
| rating       | Content rating           |
| duration     | Duration or seasons      |
| listed_in    | Genre/category           |
| description  | Short description        |

The dataset includes over 8,000 Netflix titles.

---

# Libraries Used

## NumPy

Used for numerical computations and array operations.

## Pandas

Used for data manipulation and preprocessing.

## Matplotlib

Used for plotting graphs and charts.

## Seaborn

Used for advanced statistical visualizations.

## Wordcloud

used for making word cloud from descriptions of movies and tv shows

## ntlk

used for sentiment analysing of descriptions.

---

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from wordcloud import WordCloud
import nltk
from nltk.sentiment import SentimentIntensityAnalyzer
```

# Data Cleaning Steps

* Removed duplicate records
* Handled missing values
* Converted date columns into datetime format
* Separated duration values
* Standardized categorical data
* Cleaned country and genre fields
* cleaned Actor and directors fields
---

# Exploratory Data Analysis

## Content Distribution

* Movies dominate Netflix content compared to TV Shows.
* Approximately 70% of the content consists of Movies.

## Release Year Analysis

* Significant increase in content after 2015.
* Peak content additions were observed around 2019–2020.

## Top Countries

* Unitied States contributes the highest number of titles.
* India is among the top content-producing countries.

## sentiment analysis on descriptions
* Movies have negative sentiments
  - Having more words like Crime, murder, revenge, survival and so on.
* TV shows have positive sentiments
  - Having more words like Friendship, Family, Comedy, Adventure and so on.

## Ratings Analysis

* TV-MA is one of the most common ratings.
* Netflix focuses heavily on mature audience content.

## Genre Analysis

Popular genres include:

* Dramas
* Comedies
* International Movies
* Documentaries

## Content Growth

* Netflix rapidly expanded its catalog during the late 2010s.
* TV Shows increased steadily over time.

---

# Sample Visualizations

Common visualizations created in this project:

* Count plots
* Bar charts
* Heatmaps
* Pie charts
* Line graphs

Example:

```python
sns.countplot(x='type', data=df)
plt.title("Movies vs TV Shows")
plt.show()
```

---

# Key Findings

1. Movies are more common than TV Shows on Netflix.
2. Netflix content increased rapidly after 2015.
3. The USA contributes the most Netflix titles.
4. Drama and Comedy are the most popular genres.
5. TV-MA is the dominant rating category.
6. International content availability has increased significantly.
7. Netflix heavily focuses on global audience expansion.

---

# Conclusion

This project provides valuable insights into Netflix’s streaming content trends through Exploratory Data Analysis. Using Python and data visualization libraries, we identified patterns related to content type, genre popularity, ratings, and country contributions.

The analysis demonstrates how data science techniques can help understand streaming platform trends and user-focused content strategies.
