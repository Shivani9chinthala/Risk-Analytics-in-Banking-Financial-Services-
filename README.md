# Risk-Analytics-in-Banking-Financial-Services-
# Risk Analytics in Banking & Financial Services 🏦📊

This project focuses on **risk analytics** in the banking and financial services sector. It implements a **clean, modular, and reproducible workflow** in Python and scikit-learn to assess and manage financial risk using historical customer and transaction data.

---

## 📌 Project Objective

The goal is to **analyze, model, and predict financial risk** to help banks and financial institutions:

- Identify high-risk clients and transactions ⚠️  
- Improve decision-making for credit approvals 💳  
- Enhance portfolio monitoring and regulatory compliance 📈  

---

## 📂 Dataset

- **Source:** Banking and financial services datasets  
- **Size:** 300,000+ rows, 120+ features  
- **Features:** Customer demographics, transaction history, credit history, account balances, income, employment info, and other risk-related indicators  
- **Target Column:** Risk flag / default indicator (binary)  

---

## 🛠 Project Workflow

### 1️⃣ Data Loading & Cleaning
- Load CSV data into pandas DataFrame  
- Standardize column names (lowercase, underscores)  
- Remove redundant or ID-like columns  
- Handle missing values  

### 2️⃣ Feature Engineering
- Derived features to enhance predictive performance:
  - `days_employed_abs` – absolute value of days employed  
  - `income_per_person` – household income per family member  
- Convert categorical variables to string type for preprocessing  

### 3️⃣ Preprocessing Pipeline
- **Numeric Features:** Median imputation + StandardScaler  
- **Categorical Features:** Impute missing values + OneHotEncoder  
- Combined using `ColumnTransformer`  

### 4️⃣ Model Training & Evaluation
- Models considered:
  - Logistic Regression ⚙️  
  - Random Forest Classifier 🌲  
- Train/test split with stratification  
- Stratified K-Fold Cross-Validation  
- Hyperparameter tuning for Random Forest using `GridSearchCV`  
- Metrics calculated:
  - **Accuracy:** 0.70  
  - **Precision:** 0.97 (class 0), 0.18 (class 1)  
  - **Recall:** 0.70 (class 0), 0.72 (class 1)  
  - **F1-score:** 0.81 (class 0), 0.28 (class 1)  
  - **Support:** 18354 (class 0), 1646 (class 1)  
  - **Macro Avg:** 0.57 / 0.71 / 0.55  
  - **Weighted Avg:** 0.90 / 0.70 / 0.77  

- Visualizations:
  - Confusion Matrix 🧮  
  - ROC Curve 📈  

**Interpretation:**  
- High precision for non-risky clients (class 0) ✅  
- Moderate recall for risky clients (class 1) ⚠️  
- Overall model accuracy: 70%  

### 5️⃣ Model Saving
- Best-performing model saved using `joblib` for future inference 💾  

---

## ⚡ How to Use

1. Clone the repository:
```bash
git clone <your-repo-url>
cd risk-analytics-banking

#2Install dependencies:
pip install -r requirements.txt


##Run the notebook risk_analytics_notebook.ipynb:

*Execute sequentially: Data Loading → Preprocessing → Feature Engineering → Training & Evaluation

*Trained model saved as risk_model.joblib

🔗 References

Kaggle: [Risk Analytics in Banking & Financial Services
](https://www.kaggle.com?utm_source=chatgpt.com)
Scikit-learn Documentationhttps://scikit-learn.org?utm_source=chatgpt.com

👤 Author

Refactored and documented by [shivani chinthala]

Contact: [chinthala.shivani0@gmail.com / (https://github.com/Shivani9chinthala)]
