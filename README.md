# 🏠 House Price Prediction | AutoML + LightGBM

An end-to-end machine learning project for predicting house prices using Automated Machine Learning techniques. This project leverages **PyCaret** to streamline preprocessing, model comparison, and evaluation, with **LightGBM** emerging as the best-performing model.

---

## 📌 Project Overview

Accurate house price prediction is essential for real estate analytics, investment decisions, and market understanding. This project uses the **King County housing dataset** to build and evaluate multiple regression models.

✔ Dataset size: 21,613 rows
✔ Features: 20+ (structural, location, quality)
✔ Target: `price` (regression)

---

## 🎯 Objective

Build a high-performance regression model to accurately predict house prices using property characteristics such as:

* Square footage (`sqft_living`, `sqft_lot`)
* Location (`zipcode`, `lat`, `long`)
* House quality (`grade`, `condition`)
* Additional attributes (bedrooms, bathrooms, etc.)

---

## ⚙️ Tech Stack

* Python
* Pandas / NumPy
* Scikit-learn
* LightGBM
* PyCaret (AutoML)
* Matplotlib / Seaborn

---

## 🔄 Workflow

1. Data Loading & Exploration
2. Data Preprocessing (handled by PyCaret)
3. Feature Engineering (basic)
4. Model Training & Comparison
5. Model Evaluation (Cross-validation)
6. Best Model Selection

---

## 📊 Model Performance

| Model        | R2 Score | RMSE   | MAE    |
| ------------ | -------- | ------ | ------ |
| LightGBM     | 0.8707   | 77,456 | 52,657 |
| Extra Trees  | 0.8552   | 81,977 | 55,059 |
| RandomForest | 0.8500   | 83,400 | 55,928 |
| Linear Reg.  | 0.8026   | 95,741 | 68,235 |

🏆 **Best Model: LightGBM**

---

## 📈 Key Insights

* Tree-based ensemble models significantly outperform linear models
* Location features (latitude, longitude, zipcode) are highly predictive
* Non-linear relationships dominate house pricing
* AutoML allows rapid experimentation and model selection

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/your-username/house-price-prediction-automl-pycaret.git
cd house-price-prediction-automl-pycaret
```

### 2. Create environment

```bash
conda create -n pycaret_env python=3.10
conda activate pycaret_env
```

### 3. Install dependencies

```bash
pip install pycaret pandas numpy scikit-learn seaborn matplotlib
```

### 4. Run notebook

```bash
jupyter notebook
```

---

## 📂 Project Structure

```
├── data/
├── notebooks/
│   └── house_price_prediction.ipynb
├── models/
├── README.md
└── requirements.txt
