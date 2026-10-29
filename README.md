# ATP Match Outcome Prediction

Machine learning pipeline to predict the outcomes of professional ATP tennis matches using historical tour data. Built for the Artificial Intelligence course at Ca' Foscari University of Venice.

## Overview

The project tackles match prediction as a binary classification problem, comparing baseline models against gradient-boosted decision trees. 

* **Data Preprocessing & Feature Engineering:** Cleaning historical match logs, handling missing stats, and extracting player metrics (ranking differentials, surface performance, recent form, and head-to-head records).
* **Model Training & Tuning:** Benchmarking standard classifiers from `Scikit-learn` against `XGBoost` and `LightGBM`, using chronological splits to prevent data leakage from future matches.
* **Evaluation:** Assessed via accuracy, log-loss, and ROC-AUC, along with feature importance analysis.

For the full methodology, mathematical formulation, and experimental results, see the **[Project Report (PDF)](./report.pdf)**.

## Tech Stack

* **Language:** Python 3
* **Libraries:** Scikit-learn, XGBoost, LightGBM, Pandas, NumPy, Matplotlib / Seaborn

## Repository Structure

```text
├── data/               # Raw and processed ATP datasets
├── notebooks/          # EDA, feature engineering, and training notebooks
├── src/                # Preprocessing and model evaluation scripts
├── report.pdf          # 5-page formal research report
└── requirements.txt    # Python dependencies
