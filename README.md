# Credit Card Fraud Detection with Machine Learning


## 📌 Project Overview
This project focuses on building a machine learning pipeline to detect fraudulent credit card transactions using real-world, anonymized financial data. The goal is to develop and evaluate models that can distinguish between legitimate and fraudulent transactions, despite the highly imbalanced nature of the dataset.

---

## 📊 Dataset
- **Source**: [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Size**: 284,807 transactions
- **Features**: 30 total features (including `Time`, `Amount`, and anonymized `V1–V28`)
- **Target Variable**: `Class` (0 = Non-fraud, 1 = Fraud)
- **Imbalance**: Fraudulent transactions represent only ~0.17% of the dataset

---

## 🎯 Objectives
- Preprocess and clean the dataset
- Address class imbalance with techniques like SMOTE and undersampling
- Train and evaluate multiple machine learning models
- Optimize for **recall**, as catching fraud is more important than false positives
- Compare model performance using appropriate metrics

---

## 🧠 Machine Learning Models Used
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier
- Gradient Boosting
- Support Vector Machines (SVM)

---

## 📈 Performance Metrics
Given the extreme imbalance, the following metrics were used for evaluation:
- **Precision**
- **Recall**
- **F1 Score**
- **ROC AUC**
- **Confusion Matrix**

> The XGBoost model achieved the best balance between precision and recall with an AUC of 0.985 and recall of 0.93.

---

## 🧪 Preprocessing Steps
- Feature scaling using `StandardScaler`
- Train-test split (stratified)
- Handling imbalance:
  - Random Undersampling
  - SMOTE (Synthetic Minority Oversampling Technique)

---

## 📊 Visualizations
- Fraud vs. Non-Fraud class distribution
- Correlation heatmap of PCA features
- ROC Curves
- Precision-Recall Curves
- Confusion Matrix for each model

---

## 📁 Folder Structure
credit-card-fraud-detection/
├── data/
│ └── creditcard.csv
├── notebooks/
│ └── fraud_detection_analysis.ipynb
├── models/
│ └── saved_model.pkl
├── outputs/
│ ├── visuals/
│ └── metrics/
├── README.md


---

## 🧠 Key Learnings
- Fraud detection problems require careful **handling of class imbalance**
- High accuracy is misleading—**recall and precision** are better indicators
- Ensemble models (like Random Forest and XGBoost) handle imbalanced data well with proper tuning

---

## 🔮 Future Enhancements
- Deploy model as a REST API using FastAPI or Flask
- Build a real-time dashboard using Streamlit or Tableau
- Integrate transaction metadata (e.g., device, location) to enhance detection

---

## 👤 Author
**Pragathi Porawakara Arachchige**  
[GitHub](https://github.com/PragathiM007)  
*Bellevue University – DSC680 Applied Data Science*

---

## 📜 License
This project is licensed under the **PAPM License**.
