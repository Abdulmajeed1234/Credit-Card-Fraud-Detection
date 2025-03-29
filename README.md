# 🚀 Credit Card Fraud Detection

## 📌 Project Overview
This project aims to develop a robust **classification model** to detect fraudulent credit card transactions efficiently. The dataset used for this project contains transactions made by European cardholders in **September 2013**, spanning **two days** of transactions. With **492 fraud cases out of 284,807 transactions**, the dataset is highly imbalanced, making fraud detection a challenging task.

## 📂 Dataset Details
- **Total Transactions:** 284,807
- **Fraudulent Transactions:** 492 (0.172% of total data)
- **Features:**
  - `V1` to `V28`: Principal components from PCA transformation
  - `Time`: Seconds elapsed since the first transaction
  - `Amount`: Transaction amount
  - `Class`: Target variable (0 = Non-fraud, 1 = Fraud)

## ⚙️ Methodology
### 1️⃣ Data Preprocessing
- Handled class imbalance using **oversampling, undersampling, and SMOTE** techniques.
- Standardized `Amount` and `Time` features to enhance model performance.

### 2️⃣ Feature Engineering
- Created new meaningful features such as:
  - **Transaction Frequency**: Number of transactions per customer
  - **Location Mismatch**: Identifying transactions from unusual locations
  - **Spending Patterns**: Detecting deviations in transaction behavior

### 3️⃣ Model Training
- Implemented and compared multiple machine learning models:
  - **RandomForestClassifier** (Final Model)
  - Logistic Regression
  - XGBoost
  - Decision Tree
- Evaluated models based on **Precision, Recall, F1-Score, Accuracy, and ROC-AUC Score**.

## 📊 Model Performance
**Final Model: RandomForestClassifier (random_state=42)**
- **Accuracy:** 🎯 100%
- **F1 Score:** 💯 1.00
- **Precision & Recall:** 🚀 1.00
- **ROC-AUC Score:** 📈 1.00

### 🔍 Confusion Matrix
![Confusion Matrix]![image](https://github.com/user-attachments/assets/a449f710-60d0-48ab-9765-9c11f9ead33b)

)

### 📈 Feature Importance
![Feature Importance]![image](https://github.com/user-attachments/assets/c5e38065-4bf5-477c-8c95-9ff170845063)

)

### ⚠️ Class Distribution
![Class Distribution]![image](https://github.com/user-attachments/assets/554d56df-f91a-4701-bb93-6bfc35006420)


## 🔥 Key Insights
- **Imbalanced dataset:** The original dataset was highly skewed, requiring proper resampling techniques.
- **Feature Importance:** Features like `V14`, `V10`, and `V4` played a significant role in fraud detection.
- **Performance Optimization:** Hyperparameter tuning and class balancing improved model accuracy drastically.

## 📌 How to Use
1. Clone this repository:
   ```bash
   [https://github.com/Abdulmajeed1234/Credit-Card-Fraud-Detection.git]
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the fraud detection script:
   ```bash
   python fraud_detection.py
   ```

## 📜 License
This project is open-source and available under the **MIT License**.

---
💡 *Feel free to contribute or suggest improvements!* 🚀

