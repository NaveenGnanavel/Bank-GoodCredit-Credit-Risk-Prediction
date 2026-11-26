
# Bank GoodCredit – Credit Risk Prediction

## Project Overview

Bank GoodCredit – Credit Risk Prediction is a machine learning project designed to assess customer creditworthiness and identify potential credit defaulters. The project analyzes customer account information, credit enquiry history, and demographic data to develop predictive models that support effective credit risk assessment and informed lending decisions.

## Project Objectives

- Analyze customer financial and credit-related information.
- Identify important factors influencing credit risk.
- Develop machine learning models to predict potential defaulters.
- Compare model performance using classification evaluation metrics.
- Identify the best-performing model for credit risk assessment.

## Dataset Description

The project uses three datasets extracted from a MySQL database.

| Dataset | Description |
|---|---|
| Cust_Account | Contains customer account details, credit limits, outstanding balances, overdue amounts, and payment history. |
| Cust_Enquiry | Contains customer credit enquiry details, enquiry purposes, dates, and enquiry amounts. |
| Cust_Demographics | Contains customer-related demographic features and the target variable. |

### Target Variable

**Bad_label**

- `0` – Good Credit (Non-Defaulter)
- `1` – Bad Credit (Defaulter / 30+ DPD)

## Project Workflow

1. Data Collection using MySQL.
2. Data Understanding and Exploration.
3. Data Cleaning and Preprocessing.
4. Exploratory Data Analysis (EDA).
5. Feature Engineering.
6. Feature Selection.
7. Model Development.
8. Model Evaluation and Comparison.
9. Final Model Selection.
10. Credit Risk Prediction.

## Machine Learning Algorithms

The following classification algorithms were implemented:

- **Logistic Regression:** Baseline classification model for predicting customer credit risk.
- **Random Forest Classifier:** Ensemble learning algorithm that combines multiple decision trees.
- **Extra Trees Classifier:** Tree-based ensemble algorithm that uses randomized decision splits.

## Evaluation Metrics

Model performance is evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Gini Score

**Client Benchmark:** Gini Score – 37.9

The models are compared against the client benchmark to assess their predictive performance.

## Technologies and Libraries

### Programming and Development
- Python
- Jupyter Notebook
- MySQL

### Data Analysis
- Pandas
- NumPy

### Data Visualization
- Matplotlib
- Seaborn

### Machine Learning
- Scikit-learn
- SciPy
- Joblib

### Database Connectivity
- MySQL Connector

## Project Structure

```text
Bank-GoodCredit-Credit-Risk-Prediction/
│
├── Bank_GoodCredit_Credit_Risk_Prediction.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Bank-GoodCredit-Credit-Risk-Prediction.git
```

### 2. Navigate to the Project Directory

```bash
cd Bank-GoodCredit-Credit-Risk-Prediction
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the project notebook and execute the cells in sequence.

**Note:** Database access is required to retrieve the original project data. Configure your database credentials securely using environment variables. Do not publish passwords or confidential customer information.

## Project Outcome

The project provides a machine learning-based approach to customer credit risk prediction. By analyzing financial and demographic information, the developed models help identify potential credit defaulters and support data-driven lending decisions.

## Future Enhancements

- Improve predictive performance through hyperparameter tuning.
- Implement advanced ensemble learning techniques.
- Develop an interactive credit risk prediction dashboard.
- Deploy the selected model as a web-based application.
- Monitor model performance using new customer data.

## Author

**Naveen Gnanavel**

GitHub: https://github.com/Naveen0625

LinkedIn: https://www.linkedin.com/in/naveen-gnanavel-a570a1301/

---

**Disclaimer:** This project is developed for machine learning and educational purposes. Model predictions should be validated and reviewed before being used in real-world lending decisions.
