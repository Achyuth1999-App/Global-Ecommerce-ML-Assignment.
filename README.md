# 🛒 Global E-Commerce Purchase Amount Prediction
## Supervised Learning — 7 Research Questions

**Dataset:** [Global E-Commerce Dataset (1M Records)](https://www.kaggle.com/datasets/akrambelha/global-e-commerce-dataset-1m-records)  
**Target Variable:** `Purchase_Amount` (USD) | **Task:** Regression

---

## 📓 Notebooks

| Notebook | Research Question |
|----------|-------------------|
| `RQ01_baseline_models.ipynb` | Can we predict purchase amount from demographics & browsing behaviour using baseline models? |
| `RQ02_category_analysis.ipynb` | Which product categories drive the highest purchase amounts? |
| `RQ03_payment_method.ipynb` | How does payment method correlate with purchase amounts? |
| `RQ04_age_gender.ipynb` | Does customer age and gender significantly influence spending behaviour? |
| `RQ05_items_vs_spend.ipynb` | How does the number of items relate to total spending (linear vs non-linear)? |
| `RQ06_model_comparison.ipynb` | Which ML model best predicts purchase amounts (with cross-validation)? |
| `RQ07_feature_importance.ipynb` | What are the most important features? (impurity + permutation + ablation) |

---

## ▶️ How to Run

```bash
# 1. Clone this repo
git clone <your-repo-url>
cd global-ecommerce-prediction

# 2. Install dependencies
pip install -r requirements.txt

# 3. (Optional) Download the dataset from Kaggle and place in this folder:
#    global_ecommerce.csv
#    Without the CSV, all notebooks auto-simulate a representative dataset.

# 4. Run any notebook
jupyter notebook RQ01_baseline_models.ipynb
```

## 📊 Outputs

Each notebook saves to `./outputs/`:
- `RQ0X_table_*.csv` — metric/statistics tables
- `RQ0X_fig_*.pdf` — publication-quality figures

## 🛠 Models Used
Linear Regression · Ridge Regression · Decision Tree · KNN · Random Forest · Gradient Boosting

## 📦 Requirements
See `requirements.txt`
