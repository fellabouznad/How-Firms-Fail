# How-Firms-Fail
All the code for the MPhil Thesis of Fella Bouznad. The notebooks are ordered so that a new user can follow the empirical data construction first, the failure-trajectory analysis second, and the self-contained simulation study third.

## Repository structure

```text
.
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_failure_trajectories.ipynb
│   └── 03_simulation.ipynb
├── data/
│   ├── raw/
│   └── processed/
├── results/
├── requirements.txt
└── .gitignore
```

## Notebook order

1. **`01_data_cleaning.ipynb`** merges the Annual Report, REACH, and BKR files, constructs the analysis variables, and writes `data/processed/merged_df.xlsx` and `data/processed/cleaned_df.xlsx`.
2. **`02_failure_trajectories.ipynb`** uses the merged panel to construct event-time data, matching diagnostics, matched failure trajectories, robustness checks, figures, and the RQ1 workbook.
3. **`03_simulation.ipynb`** is self-contained and evaluates the forecasting and prediction methods across four simulated DGPs and Monte Carlo replications.
