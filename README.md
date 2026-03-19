# 🏦 Credit Risk Analytics Dashboard & Machine Learning Model

## 📌 Project Overview
This project focuses on **credit risk analysis in the banking and financial services domain**.  
It combines **Excel, Python, Machine Learning, and Power BI** to analyze customer data, predict loan defaults, and build interactive dashboards for decision-making.

The project demonstrates an **end-to-end data analytics workflow** from data cleaning to model building and visualization.

---

## 🎯 Objectives
- Analyze customer data to identify **loan default patterns**  
- Build a **machine learning model** to predict credit risk  
- Create **interactive dashboards** for business insights  
- Segment customers based on financial and demographic factors  
- Support **data-driven credit decision making**  

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
- Cleaned raw dataset using **Microsoft Excel**  
- Handled missing values and inconsistent data  
- Created derived analytical columns:
  - Age (from DAYS_BIRTH)  
  - Age Group  
  - Income Band  
  - Credit-Income Ratio  
  - Ratio Band  
- Structured dataset for further analysis  

---

### 🔹 2. Data Analysis & Visualization (Power BI)
- Imported cleaned dataset into **Power BI**  
- Created DAX measures:
  - Total Customers  
  - Total Defaults  
  - Default Rate (%)  

- Built an **interactive dashboard** with:
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
- Improved dataset quality for modeling  

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
![Credit Risk Dashboard](./Screenshot%202026-03-15%20161531.png)
---

## 📊 Key Insights
- Customers with **high credit-income ratio** show higher default risk  
- **Low income groups** have higher default probability  
- Certain **contract types** are riskier  
- Demographic factors like **age and gender** influence risk patterns  

---

## 🛠️ Tech Stack
- Microsoft Excel  
- Python  
- Pandas / NumPy  
- Scikit-learn  
- Power BI  
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
