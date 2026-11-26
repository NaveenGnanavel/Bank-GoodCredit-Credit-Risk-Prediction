
# Bank GoodCredit – Credit Risk Prediction

## Project Overview

Bank GoodCredit – Credit Risk Prediction is a machine learning project developed to assess customer creditworthiness and identify potential credit defaulters. The project uses customer account information, credit enquiry history, and demographic data to build predictive classification models.

The trained model helps identify customers with a higher risk of default and supports data-driven credit risk assessment.

## Project Objectives

- Analyze customer financial and credit-related information.
- Identify important factors influencing credit risk.
- Develop machine learning models to predict potential defaulters.
- Compare multiple classification algorithms.
- Select the best-performing model based on evaluation metrics.
- Save the trained model for future predictions.

## Dataset Description

The project uses three datasets extracted from a MySQL database.

| Dataset | Description |
|---|---|
| Cust_Account | Customer account details, credit limits, outstanding balances, overdue amounts, and payment history. |
| Cust_Enquiry | Customer credit enquiry details, enquiry purposes, dates, and amounts. |
| Cust_Demographics | Customer demographic features and target variable. |

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
10. Model Saving and Prediction.

## Machine Learning Models

The following classification algorithms were implemented:

- **Logistic Regression:** Baseline model for credit risk classification.
- **Random Forest Classifier:** Ensemble model that combines multiple decision trees.
- **Extra Trees Classifier:** Randomized tree-based ensemble learning algorithm.

## Model Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Gini Score

**Client Benchmark:** Gini Score – 37.9

The models are compared using these metrics to identify the most suitable model for credit risk prediction.

## Technologies and Libraries

**Programming:** Python

**Development Environment:** Jupyter Notebook

**Database:** MySQL

**Data Analysis:** Pandas, NumPy

**Data Visualization:** Matplotlib, Seaborn

**Machine Learning:** Scikit-learn, SciPy

**Model Serialization:** Joblib

## Project Structure

```text
Bank-GoodCredit-Credit-Risk-Prediction/
│
├── Bank_GoodCredit_Credit_Risk_Prediction.ipynb
│
├── models/
│   ├── bank_goodcredit_model.pkl
│   └── bank_goodcredit_features.pkl
│
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

### 3. Install Required Libraries

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the project notebook and execute the cells in sequence.

## Loading the Trained Model

The trained machine learning model is saved as a PKL file using Joblib.

```python
import joblib

# Load the trained model
loaded_model = joblib.load(
    "models/bank_goodcredit_model.pkl"
)

# Load selected feature names
feature_names = joblib.load(
    "models/bank_goodcredit_features.pkl"
)

print("Model loaded successfully!")
```

The loaded model can be used to predict customer credit risk when provided with input data containing the required features in the correct format.

**Note:** Use the same preprocessing pipeline and feature order used during model training. Only load PKL files from trusted sources.

## Project Outcome

Developed a machine learning-based credit risk prediction solution using customer financial and demographic information. The project compares multiple classification algorithms and saves the selected trained model for future use.

The solution aims to support financial institutions in identifying potential credit defaulters, assessing customer creditworthiness, and making informed lending decisions.

## Future Enhancements

- Hyperparameter tuning for improved model performance.
- Integration of advanced machine learning algorithms.
- Development of an interactive credit risk dashboard.
- Deployment of the trained model as a web application.
- Continuous monitoring of model performance.

## Author

**Naveen Gnanavel**

GitHub: https://github.com/Naveen0625

LinkedIn: https://www.linkedin.com/in/naveen-gnanavel-a570a1301/

---

**Disclaimer:** This project is developed for machine learning and educational purposes. Predictions should be validated before being used in real-world lending decisions.
