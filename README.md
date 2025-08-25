# Customer Churn Prediction

![Last Updated](https://img.shields.io/badge/last%20updated-2025-08-25-blue) ![Made with Jupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange)

## 📌 Project Overview
This project predicts **customer churn** using machine learning models trained on customer attributes and service usage signals to identify at‑risk customers and support retention strategies.

## 📊 Dataset
- Files detected: /content/drive/MyDrive/data mining project/WA_Fn-UseC_-Telco-Customer-Churn.csv, appendix_missing_value_report_raw.csv, missing_value_report_before.csv, test_processed.csv, train_processed.csv
- Target variable (guessed): `Churn`

## 🧹 Workflow
1. **Data Preprocessing**: Missing values handling, encoding categorical features, scaling/normalization as needed.
2. **EDA**: Class balance, feature relationships, correlation heatmaps and key visualizations.
3. **Modeling**: Train/validate multiple classifiers with cross‑validation and hyper‑parameter tuning.
4. **Evaluation**: Track Accuracy/Precision/Recall/F1/ROC‑AUC; examine confusion matrices and top features.
5. **Interpretation**: Feature importances/SHAP (if available) to guide retention strategies.

## 🤖 Models Detected
- scikit-learn (Logistic Regression)
- scikit-learn (Random Forest)

## ✅ Best Metrics (auto‑parsed)
- **Accuracy**: 1.0000
- **F1-score**: 1.0000
- **Precision**: 1.0000
- **Recall**: 1.0000

## 🛠️ Tech Stack
- Python, Jupyter Notebook
- Libraries (auto‑detected imports): collections, google, imblearn, matplotlib, numpy, os, pandas, seaborn, sklearn

## 🚀 How to Run
```bash
# 1) Create environment (optional)
python -m venv .venv && source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# 2) Install dependencies
pip install -r requirements.txt

# 3) Launch Jupyter
jupyter notebook customerChurn.ipynb
```

## 📈 Reproducibility Tips
- Set a random seed for numpy/ sklearn.
- Use train/validation/test splits; report test results only once.
- Keep raw data immutable; write processed artifacts to a `data/processed` folder.

## 🧭 Project Structure (suggested)
```
.
├─ customerChurn.ipynb
├─ data/
│  ├─ raw/
│  └─ processed/
├─ notebooks/
├─ src/
│  ├─ data/
│  ├─ features/
│  ├─ models/
│  └─ visualization/
├─ README.md
└─ requirements.txt
``
