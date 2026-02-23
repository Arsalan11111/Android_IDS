# Cybersecurity ML (Notebook)

`Cybersecurity_ML.ipynb` is a Jupyter/Colab notebook for **malware classification** using **app/permission-style features** (label: `Malicious`).

## Files / Data
- Notebook: `Copy_of_Cybersecurity_ML.ipynb`
- Expects:
  - `/content/train.csv` (includes `Malicious`)
  - `/content/test.csv`

## What it does
- Loads `train.csv` / `test.csv`
- Basic EDA (class balance, plots)
- Train/test split
- Trains and evaluates models such as:
  - **LightGBM (LGBMClassifier)**
  - **Random Forest** (+ **GridSearchCV** / cross-validation)
  - **SVM (SVC)**
  - (also includes **LDA** exploration)
- Metrics: **confusion matrix**, **precision/recall**, **classification report**, **accuracy**
- Generates predictions for the test set

## Setup
```bash
pip install pandas numpy matplotlib seaborn scikit-learn lightgbm
