# Car Price Prediction with Machine Learning

**Oasis Infobyte — Data Science Internship | Task 3**  
**Project author:** Sumit Kumar

## Overview
This project develops and compares regression models to estimate used-car selling prices using a CarDekho-style dataset. It includes data quality checks, feature engineering, exploratory data analysis, preprocessing, model evaluation, residual analysis, and permutation-based feature importance.

## Objectives
- Clean and inspect a used-car dataset.
- Explore price patterns by car age, fuel type, and kilometres driven.
- Engineer a `Car_Age` feature from the manufacture year.
- Compare Linear Regression, Random Forest Regressor, and Gradient Boosting Regressor.
- Evaluate models with MAE, RMSE, and R².
- Identify influential features using permutation importance.

## Dataset
The notebook looks for a CSV in `dataset/` named `CarDekho_Dataset.csv` or `car_data.csv`. If absent, it attempts to download a public copy from the linked GitHub dataset source.

Dataset source page: https://github.com/pujarisurakshashankar/car-market-trend-analysis/blob/main/data/CarDekho_Dataset.csv

Expected columns include `Car_Name`, `Year`, `Selling_Price`, `Present_Price`, `Kms_Driven`, `Fuel_Type`, `Seller_Type`, `Transmission`, and `Owner`. Exact columns can vary by dataset version. The notebook checks required fields and uses the columns actually present.

**Dataset note:** Check the dataset source's license/terms before redistributing the CSV. The CSV is not bundled with this project.

## Project structure
```text
DataScience-Task3-CarPricePrediction/
├── car_price_prediction.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── dataset/
    └── README.md
```

## Run locally
1. Download/extract this project folder.
2. Install Python 3 and Jupyter Notebook/JupyterLab.
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Open `car_price_prediction.ipynb`.
5. Run all cells from top to bottom. If automatic download fails, download the CSV from the source page above and place it in `dataset/CarDekho_Dataset.csv`.

## Evaluation
The notebook calculates test-set MAE, RMSE, and R² for every model and selects the model with the lowest RMSE. Scores are generated from the actual run; no metric is hard-coded into the documentation.

## Limitations
The dataset may be small or dated, prices depend on collection context and units, and some useful factors (location, condition, variant, market demand) may be missing. Results should not be interpreted as guaranteed current-market valuations.

## Libraries
Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn, Jupyter.
