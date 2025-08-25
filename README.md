# Loan-Approval-Prediction

Predicting whether a loan application will be **approved or denied** using **Logistic Regression** in Python.  


## Overview
This project tackles a common real-world financial classification problem:  
**Will an individual’s loan application be approved based on demographic and financial attributes?**  

By applying logistic regression, I focus on identifying the factors most influencing loan approval decisions and evaluating the model’s predictive performance.

## Dataset
The dataset contains demographic, socio-economic, and financial details of loan applicants.  

**Columns**
- `age (int)` — Age of the individual  
- `gender (string)` — Gender of the individual (`Male`/`Female`)  
- `occupation (string)` — Applicant’s occupation  
- `education_level (string)` — Highest level of education attained (High School, Associate's, Bachelor’s, Master’s, Doctoral)  
- `marital_status (string)` — `Single` or `Married`  
- `income (int)` — Annual income (USD)  
- `credit_score (int)` — Credit score ranging between 300–850  
- `loan_status (string)` — Target variable: `Approved` or `Denied`
  
##  Objectives
- Preprocess categorical and numerical data for model training.  
- Train a Logistic Regression classifier to predict **loan_status**.  
- Evaluate performance using metrics such as Accuracy, Precision, Recall, F1-score, and ROC-AUC.  
- Identify key demographic & financial factors influencing loan approval.  
- Provide interpretable insights into how attributes such as income, credit score, and education level impact approval probability.
  
## Project Structure
---

## ⚙️ Methods
1. **Data Pre-processing**
   - Encode categorical variables (`gender`, `occupation`, `education_level`, `marital_status`)  
   - Scale numerical features (`age`, `income`, `credit_score`)  
   - Handle missing values if present  

2. **Modelling**
   - Logistic Regression (`scikit-learn`)  
   - Train/test split (Stratified)  

3. **Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC  
   - Visualisations: Confusion Matrix, ROC Curve  

4. **Interpretation**
   - Model coefficients → identify which factors drive approval likelihood  
   - Probability curves for income and credit score thresholds  

## Results 
-Accuracy: 1.0  ~ 100% 
-Precision: saved in report
- Recall: saved in report
-nROC-AUC: saved in report
- Confusion Matrix & ROC Curve: saved in reports/

## Technologies Used
- Python (pandas, numpy, scikit-learn, matplotlib)
- Jupyter Notebook

## Responsible AI
- Models should not be used in real-world lending decisions.
- Sensitive features (gender, marital_status, etc.) may lead to bias → test models with and without them.
- This project is intended for Research and educational purposes only.
  
##  Contributing
-Fork the repo
-Create a feature branch
-Commit your changes
-Open a pull request

## License

This project is licensed under the MIT License.

## References
- Hosmer & Lemeshow, Applied Logistic Regression
- scikit-learn documentation
- Fairness in Machine Learning resource
- Kaggle
