# Task 3: Heart Disease Prediction

## 📌 Objective
Build a classification model to **predict whether a person is at risk of heart disease** based on clinical attributes, and evaluate performance using accuracy, ROC curve (AUC), and confusion matrix.

---

## 📊 Dataset Used
- **Source:** UCI Heart Disease Dataset (Kaggle mirror)
- **Typical Filename:** `heart.csv`
- **Target:** `target` (1 = disease, 0 = no disease)
- **Common Features (columns may vary slightly):**
  - `age`, `sex`, `cp` (chest pain type), `trestbps` (resting blood pressure),
  - `chol` (cholesterol), `fbs` (fasting blood sugar), `restecg`,
  - `thalach` (max heart rate), `exang` (exercise-induced angina),
  - `oldpeak`, `slope`, `ca`, `thal`, etc.

---

## 🛠 Methods & Models
1. **Cleaning**
   - Replace inf values, handle missing values (drop or impute).
2. **EDA**
   - Histograms of numeric features.
   - Correlation heatmap to spot relationships.
3. **Modeling**
   - **Logistic Regression** (with standardization) *or*
   - **Decision Tree Classifier** (depth-limited).
4. **Evaluation**
   - **Accuracy**, **ROC-AUC**, **Confusion Matrix**.
5. **Feature Importance**
   - Logistic Regression coefficients (scaled) or Decision Tree `feature_importances_`.

---

## 📈 Key Results & Insights (typical)
- Both models can achieve strong baseline accuracy on this dataset.
- Features like **cp, thalach, oldpeak, ca, thal** often rank highly in importance.
- ROC curve helps visualize the **trade-off between sensitivity and specificity**.

> ⚕️ **Disclaimer:** This project is for **educational purposes only** and is **not** a medical device or diagnostic tool.

---

## 📦 Requirements
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
