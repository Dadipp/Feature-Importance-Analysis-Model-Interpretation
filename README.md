# 🔍 Feature Importance Analysis & Model Interpretation

## 🧠 Overview

Project ini berfokus pada **analisis pentingnya fitur (feature importance)** dan **interpretasi model klasifikasi** dalam konteks prediksi target variabel (misalnya churn, kelayakan kredit, atau lainnya). Tujuannya adalah memahami **faktor-faktor utama** yang memengaruhi hasil prediksi model machine learning dan menyajikan interpretasi yang dapat digunakan dalam pengambilan keputusan bisnis.

## 🧾 Tujuan Utama

- Mengidentifikasi fitur paling berpengaruh dalam model klasifikasi.
- Menggunakan berbagai pendekatan interpretabilitas model, baik berbasis model maupun agnostik model.
- Memberikan insight actionable berdasarkan hasil analisis.

## 🔧 Proses dan Metodologi

1. **Data Preparation**
   - Preprocessing data: imputasi, encoding, scaling
   - Train-test split
   - Handling imbalance data (opsional: SMOTE)

2. **Model Training**
   - Model utama: 
     - `Logistic Regression`
     - `Random Forest`
     - `XGBoost`
   - Evaluasi performa dengan:
     - Accuracy, Precision, Recall, F1-Score
     - Confusion Matrix

3. **Feature Importance Analysis**
   - Coefficients dari Logistic Regression
   - `feature_importances_` dari Random Forest dan XGBoost
   - Plot visual ranking fitur

4. **Model Interpretation**
   - **SHAP (SHapley Additive Explanations)** untuk interpretasi model kompleks seperti XGBoost
   - **Partial Dependence Plots (PDP)** untuk melihat efek fitur terhadap prediksi
   - **Permutation Importance** sebagai pendekatan agnostik model

## 📊 Insight Utama

- Fitur tertentu seperti `LIMIT_BAL`, `PAY_0`, atau `AGE` (tergantung data) memberikan kontribusi terbesar terhadap prediksi model.
- SHAP values membantu mengungkap **arah dan besar pengaruh fitur individual** terhadap prediksi model.
- Visualisasi membantu tim non-teknis memahami **mengapa** suatu prediksi dibuat.

## 🧰 Tools & Libraries

- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`
- `xgboost`
- `shap`
- `eli5`, `pdpbox`
