# Sales Prediction Using Python

**Track:** Data Science | **Task:** 5 | **Author:** Prajna K V

## Objective
Build a regression model that predicts product sales based on advertising spend across different media channels (TV, Radio, Newspaper).

## Dataset
The classic Advertising dataset — 200 records of advertising spend (in thousands of dollars) across TV, Radio, and Newspaper channels, with corresponding Sales figures.

## Tech Stack
- Python
- pandas
- matplotlib / seaborn
- scikit-learn

## Approach
1. Loaded the dataset and dropped a leftover index column.
2. Performed EDA — checked shape, data types, missing values, descriptive statistics.
3. Visualized the relationship between each advertising channel and Sales using scatter plots.
4. Built a correlation matrix/heatmap to quantify channel-sales relationships.
5. Split data into training (80%) and test (20%) sets.
6. Trained two regression models: **Linear Regression** (baseline) and **Random Forest Regressor**.
7. Evaluated both models using MAE, RMSE, and R² score.
8. Built a residual plot to check whether the best model's errors were random or systematic.
9. Interpreted feature impact via Linear Regression coefficients and Random Forest feature importances.

## Key Findings
1. **TV** has the strongest overall correlation with Sales (0.78), followed by **Radio** (0.58), while **Newspaper** is weak (0.23).
2. **Random Forest** significantly outperformed Linear Regression: R² = 0.981 vs 0.899, meaning it explains 98% of the variance in sales.
3. **Radio has the highest return per advertising dollar** (coefficient 0.19), even though TV drives more total sales due to larger typical budgets.
4. **Newspaper advertising shows minimal impact** on sales (coefficient 0.003) — likely not a cost-effective channel.
5. The residual plot shows no systematic pattern, confirming the Random Forest model performs consistently across the full range of sales values.

## Recommendation
Businesses should prioritize TV and Radio advertising spend over Newspaper, with Radio offering the best marginal return per advertising dollar.

## How to Run
Open `Sales_Prediction.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab and run all cells sequentially. Ensure `Advertising.csv` is in the same directory.

## Files in this Folder
- `Sales_Prediction.ipynb` — full notebook with code, visualizations, and analysis
- `Advertising.csv` — source dataset
- `screenshots/` — key visualizations (scatter plots, correlation heatmap, residual plot)
