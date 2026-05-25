# 🛒 Global E-Commerce Purchase Amount Prediction

A supervised machine learning project predicting customer purchase amounts using the Global E-Commerce Dataset (1M Records).

## 📌 Project Overview
| Item | Detail |
|------|--------|
| **Dataset** | Global E-Commerce Dataset (1M Records) |
| **Source** | [Kaggle – akrambelha/global-e-commerce-dataset-1m-records](https://www.kaggle.com/datasets/akrambelha/global-e-commerce-dataset-1m-records) |
| **Rows** | 1,000,000 |
| **Columns** | 9 features + 1 target |
| **Target Variable** | `Purchase_Amount` (USD) |
| **Task Type** | Regression |

## ❓ Research Questions
1. Can purchase amount be predicted from demographics and browsing behaviour?
2. Which product categories drive the highest purchase amounts?
3. How do payment methods correlate with purchase amounts?
4. Does customer age and gender significantly influence spending behaviour?
5. How does the number of items purchased relate to total spending?
6. Which ML model (Linear Regression, Ridge, Random Forest, Gradient Boosting) best predicts purchase amounts?
7. What are the most important features for predicting purchase amounts?

## 📁 Repository Structure
```
├── global_ecommerce_analysis.ipynb   # Main Jupyter Notebook (executed)
├── README.md                          # This file
├── requirements.txt                   # Python dependencies
├── fig1_target_distribution.png
├── fig2_category_boxplot.png
├── fig3_payment_method.png
├── fig4_age_gender.png
├── fig5_items_vs_spend.png
├── fig6_correlation_heatmap.png
├── fig7_model_comparison.png
├── fig8_actual_vs_predicted.png
└── fig9_feature_importance.png
```

## ▶️ How to Run

### 1. Clone the repository
```bash
git clone <your-repo-url>
cd global-ecommerce-prediction
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Download the dataset
Download from [Kaggle](https://www.kaggle.com/datasets/akrambelha/global-e-commerce-dataset-1m-records) and place `global_ecommerce.csv` in the project folder.

### 4. Run the notebook
```bash
jupyter notebook global_ecommerce_analysis.ipynb
```
> **Note:** The notebook includes a built-in data simulation mode that runs without the CSV file, making all outputs reproducible immediately.

## 📊 Key Results

| Model | MAE | RMSE | R² |
|-------|-----|------|----|
| Linear Regression | 224.55 | 399.01 | 0.1439 |
| Ridge Regression | 224.55 | 399.01 | 0.1439 |
| Random Forest | 198.18 | 363.74 | 0.2885 |
| **Gradient Boosting** | **195.50** | **360.62** | **0.3007** |

**Best Model:** Gradient Boosting Regressor  
**Top Features:** Product Category (0.36), Number of Items (0.30), Browse Time (0.10)

## 📈 Figures Generated
- Fig 1 – Target variable distribution (raw & log-transformed)
- Fig 2 – Purchase amount by product category (boxplot)
- Fig 3 – Average spend by payment method
- Fig 4 – Spend by age group & gender
- Fig 5 – Items purchased vs total spending
- Fig 6 – Correlation heatmap
- Fig 7 – Model comparison (MAE, RMSE, R²)
- Fig 8 – Actual vs predicted (best model)
- Fig 9 – Feature importance (Random Forest)

## 🛠️ Technologies Used
Python 3.11, scikit-learn, pandas, numpy, matplotlib, seaborn, Jupyter Notebook
