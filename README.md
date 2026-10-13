# Iris Flower Classification

**Internship:** Oasis Infobyte — Data Science  
**Project:** Iris Flower Classification  
**Intern:** Sumit Kumar

## Overview
This project uses the Iris dataset included with scikit-learn to classify flowers into three species:
- Setosa
- Versicolor
- Virginica

The model uses four measurements: sepal length, sepal width, petal length, and petal width.

## Objectives
- Inspect and understand the dataset.
- Perform exploratory data analysis (EDA).
- Visualize feature distributions with a pairplot and boxplots.
- Train and compare Logistic Regression and Decision Tree classifiers.
- Evaluate predictions using accuracy, precision, recall, F1-score, and confusion matrices.

## Tools and Libraries
- Python
- Jupyter Notebook
- pandas
- matplotlib
- seaborn
- scikit-learn

## Dataset
The project loads the Iris dataset directly from `sklearn.datasets.load_iris()`. No external dataset download is required.

The dataset contains 150 samples, four numerical features, and three species classes. In this notebook's inspection, no feature or species values are missing.

## Methodology
1. Import the required libraries.
2. Load the Iris dataset and create a pandas DataFrame.
3. Inspect data types, missing values, summary statistics, and class counts.
4. Perform EDA using species means, a count plot, a pairplot, and feature-wise boxplots.
5. Split the data into training and test sets using an 80/20 split with stratification.
6. Train Logistic Regression (with feature scaling) and Decision Tree classifiers.
7. Compare both models on the same test set.

## Results
On the notebook's current train/test split (random state 42):

| Model | Test accuracy | Correct predictions |
|---|---:|---:|
| Logistic Regression | 93.33% | 28 / 30 |
| Decision Tree | 93.33% | 28 / 30 |

Both models have the same measured accuracy on this split. The confusion matrices show that both classified all 10 Setosa samples correctly and each misclassified one Versicolor and one Virginica sample.

**Note:** These are results for this particular split, not a guarantee of performance on every dataset. Results can vary with different splits or data.

## How to Run
1. Install Python and Jupyter Notebook, or use an existing Jupyter environment.
2. Install the libraries listed in `requirements.txt`.
3. Open `iris_flower_classification.ipynb`.
4. Run the cells from top to bottom.

## Files
- `iris_flower_classification.ipynb` — notebook containing the analysis, visualizations, models, and evaluation.
- `README.md` — project description and results.
- `requirements.txt` — Python library dependencies.

## Learning Outcomes
This project demonstrates basic data inspection, EDA, data splitting, classification model training, and evaluation using common machine-learning metrics.
