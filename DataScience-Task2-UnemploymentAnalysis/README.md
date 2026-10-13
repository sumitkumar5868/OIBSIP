# Unemployment Analysis with Python

**Internship:** Oasis Infobyte — Data Science  
**Task:** Task 2 — Unemployment Analysis with Python

## Project overview
This project performs exploratory data analysis (EDA) on a commonly used secondary dataset of monthly unemployment estimates for Indian states/territories in 2020. It examines regional differences, monthly patterns, employment and labour-participation estimates, correlations, and a carefully defined comparison around the COVID-19 period.

This is a descriptive analysis, not a prediction model. An accuracy score is therefore not applicable.

## Dataset
- **File:** `Unemployment_Rate_upto_11_2020.csv`
- **Publisher page:** [Unemployment in India — Kaggle](https://www.kaggle.com/datasets/gokulrajkmv/unemployment-in-india)
- The selected file is commonly attributed to CMIE by the dataset publisher.
- The notebook's executed analysis covers 267 state-month observations, 27 states/territories, and 31 January–31 October 2020.
- The file name suggests November, but the inspected dates end in October 2020.
- The dataset is not bundled in this project. Download it yourself and place it at `dataset/Unemployment_Rate_upto_11_2020.csv`. Check the dataset's licence/terms before redistributing it.

See `dataset/README.md` for detailed setup.

## Analyses included
- Data loading, shape, column types, nulls, duplicates, and summary statistics
- Data cleaning and date conversion
- State-wise and geographic-region comparisons
- Monthly unemployment trends and a fixed-cohort comparison
- Top 10 states/territories by observed-period average unemployment rate
- Time-series charts for Maharashtra, Tamil Nadu, and Uttar Pradesh
- Correlation heatmap for unemployment, estimated employment, and labour participation
- A defined baseline vs. COVID-period comparison, with March treated separately
- Key findings, project limitations, and review-practice questions

## Key findings from the notebook's executed outputs
- Mean unemployment across the 267 observed state-month records: **12.24%**; median: **9.65%**.
- Haryana (**27.48%**) and Tripura (**25.06%**) have the highest observed-month state means in this dataset; Meghalaya (**3.87%**) and Assam (**4.86%**) have the lowest.
- For the fixed 25-state cohort, the Jan–Feb 2020 baseline mean is **8.76%** and the Apr–Oct 2020 mean is **13.43%**: a difference of **4.67 percentage points** (about **53.26% relative**).
- The observed all-state mean rises in April and May 2020 and declines in later months.

These are descriptive results for this incomplete secondary dataset, not official population-weighted national unemployment estimates. They do not prove that COVID-19 alone caused the observed changes.

## Tools
Python, Jupyter Notebook/JupyterLab, Pandas, NumPy, Matplotlib, Seaborn.

## Run the project
1. Download the CSV and save it to the `dataset/` folder using the exact filename above.
2. Install dependencies:
   ```bash
   python -m pip install -r requirements.txt
   ```
3. Open `unemployment_analysis.ipynb` in JupyterLab/Notebook.
4. Restart the kernel and run all cells from top to bottom.

The notebook searches for the dataset in the project folder or in the repository-root layout.

## Repository structure
```text
OIBSIP/
└── DataScience-Task2-UnemploymentAnalysis/
    ├── unemployment_analysis.ipynb
    ├── README.md
    ├── requirements.txt
    ├── .gitignore
    └── dataset/
        └── README.md
```

## Limitations
- Data covers January–October 2020 and omits some state-month records.
- There is no urban/rural column in this selected CSV.
- A simple average across states is not population- or labour-force-weighted.
- Correlation does not establish causation.
- The baseline has only January and February; the before/after comparison has no control group and cannot isolate a causal COVID-19 effect.
- The CSV's redistribution permission is unclear, so it is excluded from the repository.

## Internship note
Review the code and findings before submission so you can explain them in your own words. No GitHub commit or push is performed by this package.
