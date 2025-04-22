# 🧬 Breast Cancer Diagnosis using Machine Learning

## 📌 Project Overview
This project applies machine learning techniques for diagnosing and predicting breast cancer. It includes data preprocessing, model training, hyperparameter optimization, and model interpretability using SHAP analysis. The goal is to assist clinical decision-making with accurate and interpretable models.

---

## 📖 1. Introduction
- Breast cancer is the most common cancer among women.
- About **25%** of cases are aggressive and lead to higher mortality.
- In 2019, nearly **12,000 women in Italy** died from breast cancer.
- Screening programs and treatment advances have improved **5-year survival (87%)** and **10-year survival (80%)**.
- ML helps distinguish between **malignant** and **benign** tumors, improving early detection.

---

## 📊 2. Dataset & Preprocessing
- **Source**: Kaggle (Anonymized dataset, no PII)
- **Samples**: 569 rows
- **Features**: 31 numerical features, 1 categorical (Diagnosis)
- **Target**: `diagnosis` → M (malignant), B (benign)

### 🧹 Preprocessing:
- Dropped ID columns
- Verified no missing values
- Addressed class imbalance

### 📦 Libraries:
- `Pandas`, `NumPy`, `SciPy`, `Scikit-learn`

---

## 🧪 3. Methodology

### 🔍 Classifiers Used:
- Logistic Regression
- Decision Tree
- Gradient Boosting
- Random Forest
- LightGBM
- CatBoost

### ⚙️ Techniques:
- **Stratified K-Fold Cross Validation (K=10)**
- **F1 Score (Weighted)** as evaluation metric
- **Optuna** for hyperparameter optimization
- **SHAP** for interpretability

---

## 📈 4. Results

### 4.1 Baseline Performance

| Model                | Accuracy | Weighted F1 Score |
|---------------------|----------|-------------------|
| Logistic Regression | 94.72%   | 94.76%            |
| Random Forest       | 96.12%   | 96.14%            |
| Gradient Boosting   | 96.29%   | 96.33%            |
| Extra Trees         | 95.94%   | 95.97%            |
| XGBoost             | 96.12%   | 96.14%            |
| LightGBM            | 96.64%   | 96.71%            |
| CatBoost            | 97.00%   | 97.03%            |

### 4.2 Optimized Performance

| Model                | Accuracy | Weighted F1 Score |
|---------------------|----------|-------------------|
| Logistic Regression | 94.54%   | 94.59%            |
| Random Forest       | 91.19%   | 91.14%            |
| Gradient Boosting   | 93.67%   | 93.67%            |
| Extra Trees         | 94.54%   | 94.62%            |
| XGBoost             | 96.12%   | 96.14%            |
| LightGBM            | 96.65%   | 96.67%            |
| CatBoost            | 96.65%   | 96.70%            |

### 4.3 SHAP Analysis
- Used SHAP to explain predictions and feature contributions.
- Visualized impact of top features on model predictions.
- Compared prediction vs. base probability.

---

## 🔐 5. Ethical & Legal Considerations
- Dataset is anonymized and does not require consent.
- No personally identifiable information (PII) used.
- Complies with data ethics for medical AI research.

---

## 🧰 6. Tools & Libraries

| Type                  | Tools                           |
|-----------------------|----------------------------------|
| Data Handling         | `Pandas`, `NumPy`               |
| Modeling              | `Scikit-learn`, `CatBoost`, `LightGBM`, `XGBoost` |
| Optimization          | `Optuna`                        |
| Explainability        | `SHAP`                          |
| Scientific Computing  | `SciPy`                         |

---

