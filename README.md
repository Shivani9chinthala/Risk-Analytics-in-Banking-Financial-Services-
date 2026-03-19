# 🏦 Credit Risk Analytics Dashboard & Machine Learning Model

## 📌 Project Overview
This project focuses on **credit risk analysis in the banking and financial services domain**.  
It combines **data analysis, machine learning, and business intelligence** to identify high-risk customers and support data-driven decision-making.

The project includes:
- 📊 Power BI Dashboard for business insights  
- 🤖 Machine Learning model for risk prediction  
- 🐍 Python-based data preprocessing and analysis  

---

## 🎯 Objectives
- Analyze customer data to identify **loan default patterns**  
- Build a **machine learning model** to predict credit risk  
- Create **interactive dashboards** for business users  
- Segment customers based on financial and demographic factors  
- Support **better credit approval decisions**  

---

## 📂 Dataset
- Source: Banking & Financial Services dataset  
- Size: 300,000+ records, 100+ features  
- Features include:
  - Customer demographics  
  - Income and employment details  
  - Credit and loan information  
  - Financial behavior indicators  
- Target Variable:
  - `TARGET` (0 = No Default, 1 = Default)

---

## ⚙️ End-to-End Workflow

### 🔹 1. Data Cleaning & Preparation (Excel)
- Cleaned raw dataset in Excel  
- Handled missing values and inconsistencies  
- Created derived columns:
  - Age (from DAYS_BIRTH)  
  - Age Group  
  - Income Band  
  - Credit-Income Ratio  
  - Ratio Band  

---

### 🔹 2. Data Analysis & Visualization (Power BI)
- Imported cleaned dataset into Power BI  
- Created measures using DAX:
  - Total Customers  
  - Total Defaults  
  - Default Rate (%)  

- Built interactive dashboard with:
  - KPI Cards  
  - Slicers (Gender, Age Group, Income Band, Contract Type)  
  - Charts:
    - Default Rate by Age Group  
    - Default Rate by Income Band  
    - Default Rate by Contract Type  
    - Default Rate by Gender  
    - Default Rate by Credit-Income Ratio  

📊 Key KPIs:
- Total Customers: 308K  
- Total Defaults: 25K  
- Default Rate: ~8%  

---

### 🔹 3. Feature Engineering (Python)
- Created new features:
  - `days_employed_abs`  
  - `income_per_person`  
- Converted categorical variables for preprocessing  
- Improved data quality for modeling  

---

### 🔹 4. Preprocessing Pipeline
- Numeric Features:
  - Missing value imputation (Median)  
  - Standardization (StandardScaler)  

- Categorical Features:
  - Missing value handling  
  - OneHot Encoding  

- Combined using **ColumnTransformer**

---

### 🔹 5. Machine Learning Model
- Models used:
  - Logistic Regression  
  - Random Forest Classifier  

- Applied:
  - Train-Test Split  
  - Stratified K-Fold Cross Validation  
  - Hyperparameter tuning using GridSearchCV  

---

### 🔹 6. Model Evaluation

📊 Performance Metrics:

- Accuracy: 70%  
- Precision:
  - Class 0: 0.97  
  - Class 1: 0.18  
- Recall:
  - Class 0: 0.70  
  - Class 1: 0.72  
- F1 Score:
  - Class 0: 0.81  
  - Class 1: 0.28  

📈 Visualizations:
- Confusion Matrix  
- ROC Curve  

👉 Insights:
- High precision for low-risk customers  
- Moderate recall for high-risk customers  
- Model effectively identifies risky clients  

---

### 🔹 7. Model Saving
- Saved trained model using **joblib**
- File: `risk_model.joblib`

---

## 📊 Dashboard Preview
(Add your Power BI dashboard screenshot here)

---

## 📊 Key Insights
- Customers with **high credit-income ratio** show higher default risk  
- **Low income groups** have higher default probability  
- Certain **contract types** are riskier  
- Demographic factors like **age and gender** influence risk patterns  

---

## 🛠️ Tech Stack
- Python  
- Pandas / NumPy  
- Scikit-learn  
- Power BI  
- Excel  
- DAX  
- Matplotlib / Seaborn  

---

## 🚀 How to Run

```bash
git clone https://github.com/Shivani9chinthala/Risk-Analytics-in-Banking-Financial-Services-
cd Risk-Analytics-in-Banking-Financial-Services-
```

Install dependencies:
```bash
pip install -r requirements.txt
```

Run notebook:
```bash
jupyter notebook
```

---

## 💡 Business Impact
- Helps banks identify **high-risk customers**  
- Improves **loan approval decisions**  
- Supports **risk management strategies**  
- Enables **data-driven financial insights**  

---

## 🔗 Project Link
- GitHub Repository:  
https://github.com/Shivani9chinthala/Risk-Analytics-in-Banking-Financial-Services-

---

## 👤 Author
**Shivani Chinthala**  
📧 chinthala.shivani0@gmail.com  
🔗 https://github.com/Shivani9chinthala


