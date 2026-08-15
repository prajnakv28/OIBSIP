# Iris Flower Classification

**Track:** Data Science | **Task:** 1 | **Author:** Prajna K V

## Objective
Train a machine learning model to identify the species of an iris flower (Setosa, Versicolor, or Virginica) based on its physical measurements (sepal length, sepal width, petal length, petal width).

## Dataset
The classic Iris dataset, loaded directly from `sklearn.datasets.load_iris()` — 150 samples, 50 per species, no external download required.

## Tech Stack
- Python
- pandas
- matplotlib / seaborn
- scikit-learn

## Approach
1. Loaded and inspected the dataset (shape, data types, missing values, descriptive statistics).
2. Confirmed the dataset is clean (no missing values) and perfectly balanced (50 samples per species).
3. Visualized feature relationships using a pairplot and boxplots to identify which measurements best separate the species.
4. Split data into training (80%) and test (20%) sets.
5. Trained two classifiers: **Logistic Regression** and **K-Nearest Neighbors (KNN)**.
6. Evaluated both models using accuracy, confusion matrix, and classification report (precision, recall, F1-score).

## Key Findings
- **Petal length and petal width** are the most discriminative features — Setosa is clearly separable from the other two species on these alone.
- Both models achieved **100% accuracy** on the test set, reflecting the strong natural separation in this dataset.
- **Logistic Regression** is recommended as the preferred model since it performs equally well while being simpler and faster than KNN.

## How to Run
Open `Iris_Flower_Classification.ipynb` in Jupyter Notebook or JupyterLab and run all cells sequentially.

## Files in this Folder
- `Iris_Flower_Classification.ipynb` — full notebook with code, visualizations, and analysis
- `screenshot_pairplot.png` — key visualization showing species separation by feature
