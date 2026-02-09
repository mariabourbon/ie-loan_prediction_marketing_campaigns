# Loan Prediction Based on Marketing Campaigns

## Project Overview
This project applies machine learning techniques to predict whether a bank client will subscribe to a term deposit following a marketing campaign. Using data from a Portuguese bank, the analysis combines exploratory data analysis (EDA), supervised learning models, and business interpretation to support data-driven marketing decisions.

## Dataset
- Source: Bank Marketing Dataset (Portuguese bank)
- Observations: 11,162 client contacts
- Target Variable: `deposit` (1 = subscribed, 0 = not subscribed)
- Features include demographic, financial, and campaign-related variables

The dataset is available in the `data/` folder.

## Methodology
1. **Data Preparation**
   - Data validation (no missing values or duplicates)
   - One-Hot Encoding for categorical variables
   - Feature scaling using StandardScaler
   - Train-test split (70% / 30%)

2. **Exploratory Data Analysis**
   - Analysis of age, balance, call duration, campaign frequency
   - Identification of behavioral patterns influencing subscriptions

3. **Modeling**
   - Logistic Regression
   - Decision Tree
   - Bagging Classifier (Best performing model)

4. **Evaluation Metrics**
   - Accuracy
   - Precision, Recall, F1-Score
   - ROC-AUC
   - Confusion Matrix

## Key Results
- **Best Model:** Bagging Classifier  
- **Accuracy:** ~84%  
- **ROC-AUC:** ~0.91  

### Most Important Features
- Call duration
- Previous successful contact (`poutcome`)
- Number of previous interactions
- Account balance
- Contact type

## Business Insights
- Client engagement quality matters more than demographics
- Longer, meaningful calls significantly improve conversion rates
- Prior successful interactions strongly predict future subscriptions
- Predictive modeling can optimize campaign targeting and resource allocation

## Files in This Repository
- `notebooks/` – Jupyter notebook with full analysis and modeling
- `data/` – Dataset used for the project
- `reports/` – Executive summary and technical annex
- `README.md` – Project documentation

## Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

## Author
Group 7 – Machine Learning II  
Master’s Program (Concentration in FinTech)
