# Install and Run

## Requirements
Python 3.9+

## Installation

1. Clone the repository:
```bash
git clone https://github.com/mariacpereira/MasterThesis_MariaPereira_2026.git
cd MasterThesis_MariaPereira_2026
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Data
Download the World Bank Sovereign ESG Data Portal dataset from:
https://esgdata.worldbank.org/

Place the raw files in the `raw_data/` folder before running the notebooks.

## Running the Notebooks

Run notebooks sequentially in the following order:

| Step | Notebook | Description |
|------|----------|-------------|
| 1 | `01_governance_EU27.ipynb` | Data collection and exploration |
| 2 | `02_data_understanding_EDA.ipynb` | Exploratory Data Analysis |
| 3 | `03_data_preprocessing.ipynb` | Preprocessing and imputation |
| 4 | `04_baseline_panel_regression.ipynb` | Fixed Effects baseline |
| 5 | `05_forecast_XGB.ipynb` | XGBoost forecasting |
| 6 | `06_forecast_RF.ipynb` | Random Forest forecasting |
| 7 | `07_hyperparameters_optimizing.ipynb` | Hyperparameter tuning (Optuna) |
| 8 | `08_model_selection.ipynb` | Model selection |
| 9 | `09_clustering.ipynb` | Fuzzy C-Means clustering |
| 10 | `10_explainability_shap.ipynb` | SHAP explainability |

## Notes
- Notebook `07` includes ANN and LSTM evaluation. Both were excluded from the final pipeline due to inferior performance. See `08_model_selection.ipynb` for the full comparison.
- Hyperparameter tuning (notebook `07`) uses `seed=42` for reproducibility, but results may vary slightly depending on system configuration.
