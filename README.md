# 🛡️ Suspicious Transaction Detection (AML)

This project focuses on detecting suspicious (money laundering) transactions using machine learning techniques on a large synthetic Anti-Money Laundering (AML) dataset. It applies various models and data preprocessing steps to identify fraudulent activity with high precision and recall.

---

## 📌 Overview

Financial institutions are required to monitor and report suspicious transactions under AML regulations. This project simulates such detection using a synthetic dataset with over 9.5 million transactions. We trained models like **Random Forest** and **XGBoost**, achieving **100% precision/recall** and **1.0 ROC-AUC** on a 100K sample for proof-of-concept.

---

## 📂 Dataset

> The original dataset is too large to upload directly to GitHub. Please download it from Kaggle:

🔗 **Dataset:**  
[Synthetic Transaction Monitoring Dataset – AML (SAML-D) – Kaggle](https://www.kaggle.com/datasets/berkanoztas/synthetic-transaction-monitoring-dataset-aml)

After downloading, place `SAML-D.csv` in your working directory or modify the notebook’s file path.

---

## 🧠 Objectives

- Detect suspicious transactions from anonymized financial data.
- Handle extreme class imbalance (0.10% fraud cases).
- Visualize transaction trends between normal and laundering activities.
- Use metrics like ROC-AUC, precision, recall, F1-score for evaluation.

---

## 🔧 Technologies Used

| Category          | Tools / Libraries                         |
|-------------------|--------------------------------------------|
| Language          | Python                                     |
| Data Processing   | Pandas, NumPy                              |
| Visualization     | Matplotlib, Seaborn                        |
| Machine Learning  | Scikit-learn, XGBoost                      |
| Evaluation        | ROC-AUC, Precision, Recall, F1-score       |

---

## ⚙️ Preprocessing Steps

- Loaded 9.5M records, sampled 100K for fast experimentation.
- Addressed class imbalance with **upsampling** (`fraud` class was 0.10%).
- Applied **log transformation** to reduce skewness (24.4 → –1.0).
- Split into 80% training and 20% testing sets.

---

## 📈 Model Performance (Random Forest & XGBoost)

| Metric          | Score       |
|----------------|-------------|
| Precision       | 100%        |
| Recall          | 100%        |
| F1-score        | 100%        |
| ROC-AUC         | 1.00        |
| TPR             | 90%         |
| FPR             | 0.00%       |

---

## 📊 Visualizations

- Distribution plots before and after log transformation
- Alert-level comparison between normal vs laundering transactions
- Feature importance charts

---

## 🔁 Future Improvements

- Use full 9.5M records for large-scale training
- Integrate SHAP for interpretability
- Deploy as a dashboard for real-time scoring

---

## 🧑‍💻 Author

**Rachakonda Shrutik Sai**  
📫 shrutiksai14@gmail.com  

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---
