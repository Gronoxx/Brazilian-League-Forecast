# ⚽ Football Analytics: A Data-Driven Exploration

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge&logo=matplotlib&logoColor=white)
![NumPy](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white)

<br>

<p align="center">
  <em>A collection of data analysis projects aimed at answering key questions in the world of football using statistical modeling and machine learning.</em>
</p>

<p align="center">
  <img width="1780" height="772" alt="image" src="https://github.com/user-attachments/assets/b8a4143a-c842-48e4-895b-1e6ab84f6e0f" />
</p>

---

## About This Project

This repository moves beyond simple match results to explore the underlying dynamics that shape professional football. By analyzing historical data from the Brazilian Championship (Brasileirão) and the FIFA World Cup, this project tests common hypotheses and builds predictive models to uncover actionable insights.

The central analyses aim to answer four key questions:
1.  Can **historical performance** accurately predict the top contenders in a league season?
2.  How significant is the **home-field advantage** in professional football?
3.  Does the **time of day** a match is played have any real impact on goal-scoring?
4.  Is modern football truly becoming **more defensive** over time?

## Analyses and Key Findings

Each question was investigated using a dedicated data analysis notebook. Here are the main findings:

### 1. Predicting the Brazilian Championship Top 5
> Can we use a team's track record to forecast its success in an upcoming season?

-   **Methodology:** A **Logistic Regression** model was trained on data from 2003-2018. The features consisted of a team's history of finishing in the Top 5 in the preceding years.
-   **💡 Key Finding:** The model achieved an impressive **97.7% accuracy** in predicting the Top 5 for the 2019 season. This confirms that past performance is an overwhelmingly strong predictor of future success, highlighting the consistent dominance of a few elite teams in the league.

---

### 2. The Power of Home-Field Advantage
> Is the "home advantage" a real, quantifiable phenomenon?

-   **Methodology:** A statistical analysis of match results from the Brazilian league was performed, comparing goals scored and matches won by home vs. away teams.
-   **💡 Key Finding:** The data shows a powerful home-field advantage. Home teams won **4,001 matches** compared to just **1,901** for away teams and scored over **50% more goals on average** (1.55 for home teams vs. 1.02 for away teams).

---

### 3. The Influence of Match Timing
> Does the kickoff time affect player performance and the number of goals scored?

-   **Methodology:** World Cup match data was cleaned and grouped by start time. A regression analysis and Pearson correlation were used to measure the relationship between match time and total goals.
-   **💡 Key Finding:** The analysis revealed a **near-zero correlation (0.004)**, indicating no statistically significant link between the time of day a match is played and the number of goals scored.

---

### 4. Goal Scoring Trends in the World Cup
> Has football become more offensive or defensive over time?

-   **Methodology:** An OLS (Ordinary Least Squares) regression was performed on the total goals per match for every World Cup year.
-   **💡 Key Finding:** The regression model showed a **statistically significant negative coefficient** for the `Year` variable. This suggests that, on average, the number of goals scored per match has slightly decreased over the history of the World Cup, lending data-driven support to the idea that modern football has become more strategically defensive.

## Tech Stack

-   **Data Manipulation & Analysis:** `Pandas`, `NumPy`
-   **Statistical Modeling:** `Scikit-learn`, `Statsmodels`, `SciPy`
-   **Data Visualization:** `Matplotlib`, `Seaborn`
-   **Environment:** `Jupyter / Google Colab Notebooks`

## Getting Started

To explore these analyses yourself, simply clone the repository and run the notebooks in an environment with the required libraries installed.

```bash
# Clone the repository
git clone [https://github.com/Gronoxx/Brazilian-League-Forecast.git](https://github.com/Gronoxx/Brazilian-League-Forecast.git)

# Navigate to the project directory
cd Brazilian-League-Forecast
```
From there, you can open and run any of the `.ipynb` files.
