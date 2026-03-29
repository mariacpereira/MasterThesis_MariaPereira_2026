# Boosting ESG Governance Analysis
### Explaining Typologies and Transitions in the European Union

**Author:** Maria Cristino Pereira  
**Degree:** MSc Data Science and Advanced Analytics — Business Analytics  
**Institution:** NOVA Information Management School, Universidade Nova de Lisboa  
**Supervisor:** Prof. Doutora Fátima Trindade Neves  
**Year:** 2026

---

## Research Question
What factors explain the typologies and temporal variations of ESG governance indicators across EU member states?

## Objectives
1. Forecast governance indicators to analyse their trajectories over time (2000–2030)
2. Identify governance typologies of EU-27 countries via Fuzzy C-Means clustering
3. Explain typology transitions using SHAP-based explainability

---

## Data
World Bank Sovereign ESG Data Portal — 17 governance indicators, EU-27 member states, 2000–2023.  
Download from: https://esgdata.worldbank.org/

> Data files are not included in this repository. Please download directly from the World Bank portal and place in a `/data` folder.

---

## Notebooks

| Notebook | Description |
|----------|-------------|
| `01_governance_EU27.ipynb` | Data collection and governance indicator exploration |
| `02_data_understanding_EDA.ipynb` | Exploratory Data Analysis |
| `03_data_preprocessing.ipynb` | Missing values, outliers, scaling |
| `04_baseline_panel_regression.ipynb` | Fixed Effects Panel Regression baseline |
| `05_forecast_XGB.ipynb` | Forecasting with XGBoost |
| `06_forecast_RF.ipynb` | Forecasting with Random Forest |
| `07_hyperparameters_optimizing.ipynb` | Hyperparameter tuning with Optuna |
| `08_model_selection.ipynb` | Model comparison and selection |
| `09_clustering.ipynb` | Fuzzy C-Means clustering and transition analysis |
| `10_explainability_shap.ipynb` | SHAP explainability |

Run notebooks sequentially: `01 → 02 → ... → 10`

---

## How to Install and Run
See [Install_and_Run.md](Install_and_Run.md)

---

## Repository Structure
```
MasterThesis_MariaPereira_2026/
├── README.md
├── Install_and_Run.md
├── requirements.txt
├── notebooks/
│   ├── 01_governance_EU27.ipynb
│   ├── 02_data_understanding_EDA.ipynb
│   └── ...
└── data/          ← download from World Bank (not included)
```
