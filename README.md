# ATP Match Outcome Prediction

Machine learning pipeline to predict the outcomes of professional ATP tennis matches using historical tour data. Built for the Artificial Intelligence course at Ca' Foscari University of Venice.

## Overview

The project tackles match prediction as a binary classification problem, comparing baseline models against gradient-boosted decision trees. 

* **Data Preprocessing & Feature Engineering:** Cleaning historical match logs, handling missing stats, and extracting player metrics (ranking differentials, surface performance, recent form, and head-to-head records).
* **Model Training & Tuning:** Benchmarking standard classifiers from `Scikit-learn` against `XGBoost` and `LightGBM`, using chronological splits to prevent data leakage from future matches.
* **Evaluation:** Assessed via accuracy, log-loss, and ROC-AUC, along with feature importance analysis.

For the full methodology, mathematical formulation, and experimental results, see the **[Project Report (PDF)]**.

##
The raw match data is not tracked in this repository due to file size. To re-run the notebook from scratch, download the historical ATP match xlsx from [here]([./report.pdf](https://drive.google.com/drive/folders/14ytRIAsi-rZANoE9lV3VlTZeJwCllvgb?usp=sharing)) and place them in the root directory. All pre-computed outputs and plots are already saved directly in the notebook.

## Tech Stack

* **Language:** Python 3 (Jupyter Notebook)
* **Libraries:** Scikit-learn, XGBoost, LightGBM, Pandas, NumPy, Matplotlib / Seaborn

## Running the Notebook

1. Clone the repository and install the required packages:
   ```bash
   git clone [https://github.com/tokkkkkkk/tennis_prediction.git](https://github.com/tokkkkkkk/tennis_prediction.git)
   cd tennis_prediction
   pip install scikit-learn xgboost lightgbm pandas numpy matplotlib seaborn jupyter
