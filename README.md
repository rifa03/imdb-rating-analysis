# IMDb Rating Analysis: Genre & Duration


## Project Overview

This project analyzes factors influencing IMDb movie ratings using Exploratory Data Analysis (EDA) and Multiple Linear Regression.

The analysis investigates whether movie genre and duration influence user ratings for movies released between 2010-2020.


## Objective

The objectives of this project are:

- Analyze movie rating patterns based on genre
- Investigate relationship between movie duration and rating
- Identify factors contributing to higher IMDb ratings


## Dataset

Dataset:
IMDb Top 5000 Movies

Source:
Kaggle - Tiago Adria Nunes


After filtering:
- Period: 2010-2020
- Movies analyzed: 1,619


## Methodology

CRISP-DM Framework:

1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Exploratory Data Analysis
5. Modeling
6. Evaluation


## Tools

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Jupyter Notebook


## Analysis Workflow

### Data Preparation

Performed:
- Missing value checking
- Duplicate removal
- Genre transformation
- Multi-label encoding


### Exploratory Data Analysis

Analysis:
- Rating distribution by genre
- Duration vs rating relationship
- Rating trend over years


### Modeling

Algorithm:

Multiple Linear Regression


Evaluation:

R²:
0.2359

MSE:
0.2408


## Key Findings


### Genre Influence

Positive contribution:

- Documentary (+0.9476)
- Animation (+0.3671)
- News (+0.3072)


Negative contribution:

- Horror (-0.2814)
- Musical (-0.2637)
- Romance (-0.2140)


### Duration Influence

Duration has a positive but weak relationship with movie ratings.


## Data Processing Steps

The data preparation process includes:

1. Selecting relevant attributes:
   - Year_Release
   - Duration
   - Genres
   - Rating

2. Data quality checking:
   - Missing value detection
   - Duplicate data removal

3. Feature transformation:
   - Converting genre labels into multi-label format
   - Applying MultiLabelBinarizer encoding for genre features


## Model Interpretation

The regression model was used to understand how movie characteristics contribute to IMDb ratings.

The model coefficients indicate:

- Positive coefficient → feature contributes to increasing predicted rating
- Negative coefficient → feature contributes to decreasing predicted rating


## Limitations

This analysis has several limitations:

- The dataset only uses IMDb Top 5000 Movies.
- The analysis focuses on genre, duration, and release year.
- Other factors such as actors, directors, production budget, marketing, and audience size were not included.


## Future Improvements

Possible improvements:

- Add additional variables such as:
  - Number of votes
  - Director information
  - Cast information
  - Metascore

- Compare regression performance with other machine learning algorithms.
- Develop an interactive dashboard for exploring movie insights.
