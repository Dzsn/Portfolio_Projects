# Movie Correlation Analysis Project

This project analyzes a movie dataset to explore relationships between different features, such as budget, gross earnings, and other movie-related attributes. The goal is to identify strong correlations and visualize how key factors interact with each other in the movie industry.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Correlation Analysis](#correlation-analysis)
- [Visualizations](#visualizations)
- [Strong Correlations](#strong-correlations)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Author](#author)

---

## Project Overview
The aim of this project is to explore relationships between different numerical and categorical features in a movie dataset. Special focus is given to understanding how budget, gross earnings, votes, and other movie attributes are correlated. The analysis includes:

- Data cleaning and missing value handling.
- Conversion of data types for analysis.
- Label encoding of categorical features.
- Visual exploration of feature relationships.
- Identifying strong correlations.

---

## Dataset
The dataset used in this project is a CSV file (`movies.csv`) containing information about various movies. Key features include:

- `budget`: The budget of the movie.
- `gross`: The gross earnings of the movie.
- `released`: Release date of the movie.
- `votes`: Number of votes received.
- Other categorical features such as director, genre, and actor names.

---

## Data Cleaning and Preprocessing
- **Missing values**:  
  - Numeric columns: Missing values are filled with the median.  
  - Categorical columns: Missing values are filled with the mode.  

- **Data type conversions**:  
  - `budget` and `gross` converted to integer (`int64`).  
  - `released` column processed to extract the correct release year.

- **Duplicate removal**: Duplicate rows were dropped.

---

## Exploratory Data Analysis (EDA)
- Scatter plots and regression plots were used to visualize the relationship between `budget` and `gross`.
- Distribution and trends of other features were examined using Pandas and Seaborn.

---

## Correlation Analysis
- Pearson correlation was used to measure linear relationships between numerical variables.
- Categorical features were label encoded to include them in the correlation matrix.
- A comprehensive correlation matrix was generated to identify strong relationships.

---

## Visualizations
- **Budget vs Gross Earnings** s
