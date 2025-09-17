# Movie Correlation Analysis Project

This project analyzes a movie dataset to explore relationships between different features, such as budget, gross earnings, votes, and other movie-related attributes. The goal is to identify strong correlations and visualize how key factors interact with each other in the movie industry.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Correlation Analysis](#correlation-analysis)
- [Visualizations](#visualizations)
- [Findings](#findings)
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

### Budget vs Gross Earnings
![Budget vs Gross](images/budget_vs_gross.png)  
*Scatter plot with regression line showing the positive relationship between budget and gross earnings.*

### Correlation Matrix (Numerical Features)
![Correlation Matrix](images/correlation_matrix_numeric.png)  
*Heatmap showing correlations between numeric variables.*

### Correlation Matrix (All Features)
![Correlation Matrix All](images/correlation_matrix_all.png)  
*Heatmap including label-encoded categorical variables.*

---

## Findings

1. **Relationship between Budget and Gross Earnings**  
   - There is a strong positive correlation between the movie budget and gross earnings.  
   - Higher-budget movies generally earn more revenue.

2. **Votes and Gross Earnings**  
   - The number of votes a movie receives is also strongly positively correlated with its gross earnings.  
   - Popular movies with more votes tend to generate higher revenue.

3. **Other Features**  
   - After label encoding categorical features (e.g., director, genre, actors), some directors and genres were found to have a higher influence on revenue.  
   - However, many features showed weak correlation and did not significantly affect gross earnings.

4. **Missing Data and Cleaning**  
   - Missing values were handled with median and mode imputation, preventing data loss.  
   - Duplicate entries were removed, ensuring data integrity.

5. **Overall Conclusion**  
   - Movie budget and number of votes are the strongest predictors of movie success (gross earnings).  
   - These findings highlight the importance of budget planning and marketing/vote-gathering strategies in the film industry.

---

## Strong Correlations
Some of the key strong correlations found in this dataset:

| Feature 1      | Feature 2       | Correlation |
|----------------|----------------|------------|
| Gross Earnings | Votes          | 0.63       |
| Budget         | Gross Earnings | 0.75       |

---

## Technologies Used
- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn

---

## How to Run
1. Clone the repository:
   ```bash
   git clone <https://github.com/Dzsn/Portfolio_Projects.git>
