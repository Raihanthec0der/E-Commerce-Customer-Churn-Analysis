# E-Commerce Customer Churn Analysis

An end-to-end data science project that analyzes e-commerce customer behavior to identify patterns associated with customer churn and evaluate machine learning models for churn-risk prediction.

## Project Overview

Customer churn is an important business problem for e-commerce companies. This project explores customer demographics, engagement, purchasing behavior, service interactions, and other customer-level attributes to answer:

> What customer behaviors and characteristics are associated with churn?

The project combines Exploratory Data Analysis (EDA), data quality checks, visualization, machine learning, model evaluation, and churn-risk segmentation.

## Key Objectives

- Understand the overall customer churn rate
- Identify customer behaviors associated with churn
- Analyze customer engagement and purchasing patterns
- Investigate customer friction such as cart abandonment, returns, and service interactions
- Compare churn across selected categorical variables
- Build Logistic Regression and Random Forest churn models
- Evaluate models using accuracy, precision, recall, F1, and ROC-AUC
- Segment customers into low-, medium-, and high-risk groups
- Translate analytical findings into practical retention strategies

Dataset Source

Kaggle — Ecommerce Customer Behavior Dataset(www.kaggle.com/datasets/dhairyajeetsingh/ecommerce-customer-behavior-dataset)

Dataset Author: Dhairyajeet Singh
Records: 50,000 customers
Features: 25
Target: Churned
Coverage: Multiple countries including USA, UK, Germany, Canada, India, Japan, and France
Data Type: Numerical + categorical customer behavior data
License: Open Database / Database Contents

## Project Structure

```text
E-Commerce-Customer-Churn-Analysis/
│
├── Data/
│   └── ecommerce_customer_churn_dataset.csv
│
├── Notebooks/
│   └── E-Commerce_Customer_Churn_Analysis_Professional.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Analysis Workflow

### 1. Data Loading
Loads the dataset and checks dimensions, columns, data types, and summary statistics.

### 2. Data Quality Assessment
Checks duplicates, missing values, missing-value percentages, and unusual age values.

For modeling, numerical missing values are imputed with the median and categorical missing values with the most frequent category. Preprocessing is kept inside the ML pipeline to reduce data leakage.

### 3. Exploratory Data Analysis
The analysis covers:

- Churn distribution
- Numerical features vs. churn
- Correlation with churn
- Customer engagement
- Purchase behavior
- Cart abandonment
- Purchase recency
- Customer service interactions
- Gender
- Country
- Signup quarter
- Feature-to-feature correlations

### 4. Machine Learning

#### Logistic Regression
Used as an interpretable baseline model.

#### Random Forest
Used to capture nonlinear relationships and feature interactions.

### 5. Model Evaluation

Models are evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Confusion Matrix
- ROC Curve
- Precision-Recall Curve
- 5-fold Cross-Validation

### 6. Churn Risk Segmentation

Model probabilities are converted into:

- Low Risk
- Medium Risk
- High Risk

These groups are then compared to understand customer behavior across risk levels.

## Business Insights Framework

The project focuses on:

1. Churn level
2. Customer engagement
3. Purchase behavior
4. Customer friction
5. High-risk customer characteristics

## Business Recommendations

Potential actions include:

- Prioritize high-risk customers for retention campaigns
- Monitor declining engagement as an early-warning signal
- Investigate cart abandonment and service-related friction
- Use purchase recency and frequency for targeted re-engagement
- Personalize retention offers instead of discounting every customer
- Monitor model performance over time

These recommendations should be validated through business experiments before being treated as causal conclusions.

## Professional Data Science Practices

This project demonstrates:

- Data quality assessment
- Documented cleaning assumptions
- Pipeline-based preprocessing
- Train/test splitting with stratification
- Model comparison
- Cross-validation
- Multiple evaluation metrics
- Risk segmentation
- Separation of EDA findings from predictive results
- Cautious interpretation of correlations and feature importance

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/E-Commerce-Customer-Churn-Analysis.git
cd E-Commerce-Customer-Churn-Analysis
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Start Jupyter:

```bash
jupyter notebook
```

Open:

```text
Notebooks/E-Commerce_Customer_Churn_Analysis_Professional.ipynb
```

Dataset location:

```text
Data/ecommerce_customer_churn_dataset.csv
```

## Limitations

- The analysis is observational and does not establish causation.
- Dataset-specific patterns may not generalize to every e-commerce business.
- The age validation rule is an explicit project assumption.
- Model performance depends on available features and data quality.
- Production deployment would require additional validation, monitoring, and appropriate threshold selection.

## Future Improvements

- Hyperparameter optimization
- Advanced feature engineering
- Gradient-boosting models
- SHAP-based explainability
- Customer lifetime value analysis
- Retention campaign simulation
- Cost-sensitive threshold optimization
- Dashboard or API deployment
- Automated model monitoring

## Author

**Abdullah Al Raihan**

Data Science / Data Analysis Portfolio Project

> Learning by building real-world data projects.
