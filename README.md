# 🎓 Student Performance Classifier

This project uses the **"Students Performance in Exams"** dataset from Kaggle to predict whether a student will score **above 70 in math** based on demographic and academic features. The final model achieves **>95% accuracy** using advanced feature engineering and ensemble learning.

---

## 📦 Dataset

- **Source**: [Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
- **Columns**:
  - Gender, Race/Ethnicity
  - Parental Level of Education
  - Lunch, Test Preparation Course
  - Scores in Math, Reading, and Writing

---

## 📈 Problem Statement

> Predict whether a student will achieve a **high math score (>70)** using features like gender, parental education, test preparation, and other exam scores.

---

## 🧠 ML Techniques Used

- ✅ Feature Engineering:
  - Combined reading and writing scores (`rw_avg`)
  - Ordinal encoding of parental education
- ✅ One-Hot Encoding for categorical features
- ✅ Model Training:
  - Random Forest
  - Gradient Boosting
  - XGBoost (tuned)
- ✅ Final Model:
  - **VotingClassifier Ensemble**
- ✅ Hyperparameter tuning with `GridSearchCV`

---

## 🚀 Accuracy Achieved

| Model             | Accuracy   |
|------------------|------------|
| XGBoost (base)    | ~88%       |
| XGBoost (tuned)   | ~93–95%    |
| **Final Ensemble**| **>95% ✅** |

---

## 🧪 Prediction Pipeline

1. Preprocess new student data
2. Apply same feature engineering and encoding
3. Predict `high_math_score` (1 or 0)
4. Output prediction confidence (`predict_proba`)
5. Export results to `predicted_scores.csv`

---

