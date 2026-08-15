# Unemployment Analysis with Python

**Track:** Data Science | **Task:** 2 | **Author:** Prajna K V

## Objective
Perform exploratory data analysis on unemployment data to uncover regional and temporal trends, with a focus on the impact of the COVID-19 pandemic on unemployment rates in India.

## Dataset
State-wise monthly unemployment data for India, January 2020 – October 2020 (267 records, 27 states). Includes unemployment rate, estimated employed population, labour participation rate, and geographic zone/coordinates per state.

## Tech Stack
- Python
- pandas
- matplotlib / seaborn

## Approach
1. Loaded the dataset and cleaned column names (fixed a duplicate "Region" column and whitespace issues).
2. Converted the Date column from text to a proper datetime type to enable time-series analysis.
3. Performed EDA — checked shape, data types, missing values, and date range.
4. Visualized unemployment trends over time for major states (Maharashtra, Tamil Nadu, Uttar Pradesh).
5. Identified the top 10 states by average unemployment rate using a bar chart.
6. Built a correlation heatmap between Unemployment Rate, Employed, and Labour Participation Rate.
7. Compared average, minimum, and maximum unemployment rates before vs. after India's COVID-19 lockdown (25 March 2020).

## Key Findings
1. **COVID-19 impact:** All examined states show a sharp unemployment spike around April–May 2020, coinciding with India's lockdown, followed by a gradual recovery through the rest of 2020.
2. **Regional disparity:** Haryana and Tripura recorded the highest average unemployment rates in 2020 (both above 25%), notably higher than other states.
3. **Weak correlation with labour participation:** Unemployment rate changes were only weakly correlated with employment/labour participation figures, suggesting the spike was driven by job losses among active job-seekers rather than people leaving the workforce.
4. **Magnitude of lockdown effect:** Average unemployment rose ~40% (9.23% → 12.96%) post-lockdown, with peak rates reaching as high as 75.85% in some state/month combinations.

## Business Recommendations
1. Prioritize targeted employment support programs in states like Haryana and Tripura, where elevated unemployment predates and outlasts the general pandemic trend.
2. Develop rapid-response employment schemes for future economic shocks, given how quickly unemployment spiked and how many months it took to normalize.
3. Investigate sector-specific job losses in high-unemployment states to design more targeted interventions.

## How to Run
Open `Unemployment_Analysis.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab and run all cells sequentially. Ensure `unemployment_data.csv` is in the same directory.

## Files in this Folder
- `Unemployment_Analysis.ipynb` — full notebook with code, visualizations, and analysis
- `unemployment_data.csv` — source dataset
- `screenshots/` — key visualizations (time-series, top 10 states, correlation heatmap)
