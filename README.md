# 🫀 Heart Disease Prediction

An end-to-end Machine Learning project that predicts the presence of heart disease using clinical features. Built following the framework from **Aurélien Géron's "Hands-On Machine Learning" Chapter 2**.

## 📊 Results

| Model | Accuracy | Recall (Disease) | F1 Score |
|-------|----------|-----------------|----------|
| Logistic Regression ✅ | 82% | 85% | 84% |
| SVM | 77% | 82% | 79% |
| Random Forest | 75% | 79% | 78% |

> **Logistic Regression** was selected as the final model for its superior recall — critical in healthcare where missing a diagnosis is dangerous.

## 📁 Project Structure
```
Heart_Disease_prediction/
│
├── data/
│   └── heart.csv
├── notebooks/
│   └── heart_disease.ipynb
├── images/
│   └── confusion_matrix.png
│   └── feature_importance.png
└── README.md
```

## 🔍 Key Findings

- **Chest pain type (cp)** was the strongest predictor of heart disease
- **Age and cholesterol** — commonly assumed risk factors — were surprisingly weak predictors
- Dataset had **723 duplicate rows** — catching and removing them was critical to avoid a false 100% accuracy
- Final model catches **85% of actual heart disease patients** (recall)

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.12-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange)
![Pandas](https://img.shields.io/badge/Pandas-Data-green)
![Seaborn](https://img.shields.io/badge/Seaborn-Viz-lightblue)

## ⚙️ Methodology

1. **EDA** — Correlation heatmap, age distribution, target balance
2. **Data Cleaning** — Removed 723 duplicate rows from 1025 total
3. **Model Training** — Logistic Regression, Random Forest, SVM
4. **Hyperparameter Tuning** — GridSearchCV optimizing for Recall
5. **Evaluation** — Confusion matrix, classification report, feature importance

## 🚀 How to Run

```bash
git clone https://github.com/SahilDogra23/Heart-Disease-Prediction.git
cd Heart-Disease-Prediction
pip install -r requirements.txt
jupyter notebook notebooks/heart_disease.ipynb
```

## 📚 Reference

- Géron, A. (2019). *Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow* — Chapter 2
- Dataset: [Kaggle Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

## 👤 Author

**Sahil Dogra**
[![GitHub](https://img.shields.io/badge/GitHub-SahilDogra23-black)](https://github.com/SahilDogra23)