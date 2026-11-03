# Loan Approval Analysis & Prediction

**Tools:** Power BI | Power Query | Python | Pandas | Scikit-learn

## 1. Project Overview

The objective of this project was to analyze historical banking and loan-related data to identify patterns associated with loan approval decisions.

The analysis focused on customer demographics, loan characteristics, interest rates, transaction anomalies and customer feedback. It also involved developing a machine learning model to classify loan status.

The project demonstrates how data analytics and machine learning can support informed decision-making in the financial sector.

## 2. Tools and Technologies

- **Power BI:** Dashboard development and data visualization.
- **Power Query:** Data cleaning and transformation.
- **Python:** Predictive modelling.
- **Pandas:** Data exploration and manipulation.
- **Scikit-learn:** Random Forest classification and model evaluation.

## 3. Dataset Overview

The project involved historical banking and loan-related datasets covering:

- Customer and account information.
- Transaction records.
- Loan applications and loan characteristics.
- Credit card information.
- Customer feedback.
- Transaction anomalies.

For the machine learning exercise, a separate loan training dataset (`ML_Loan_Training.csv`) containing 5,000 records was used.

The dataset included variables such as age, city, loan amount, loan type, interest rate, loan term, approval/rejection date, loan status and anomaly.

The target variable was **Loan Status**, consisting of three categories: Approved, Closed and Rejected.

## 4. Methodology

The project involved the following activities:

**Data Preparation**
- Reviewed data types, missing values and duplicate records.
- Cleaned and transformed relevant data using Power Query.
- Used LabelEncoder to convert categorical variables into numerical formats for machine learning.

**Data Analysis**
- Examined loan approval patterns across customer demographics and loan categories.
- Analyzed interest rate trends and monthly loan activity.
- Investigated customer feedback and transaction anomalies.

**Predictive Modelling**
- Used Python, Pandas and Scikit-learn.
- Developed a Random Forest Classification model.
- Split the machine learning dataset into 80% training data and 20% testing data.
- Generated predictions for the three loan-status categories.

## 5. Dashboard Insights and Key Findings

An interactive Power BI dashboard was developed to present the analysis through charts, KPIs, filters and navigation buttons.

The dashboard examined loan approval rates, monthly loan activity, customer feedback and transaction anomalies.

**Key findings included:**

- **Customer Demographics:** Adults aged 31–55 recorded higher loan approval rates and represented the largest customer demographic.
- **Loan Terms:** Adults recorded loan terms averaging up to five years, compared with predominantly four-year terms among older and younger adult groups.
- **Interest Rates:** Average interest rates were 5.50% in 2020, 5.48% in 2021 and 5.53% in 2022.
- **Customer Feedback:** Suggestions and complaints recorded relatively similar proportions, with positive feedback comparatively low.
- **Transaction Anomalies:** Anomalous transactions represented less than 6% of the records. Approved anomalous transactions numbered 32 in 2020 and 38 in both 2021 and 2022.
- **Loan Type:** Mortgage loans recorded the highest approval rates.
- **Loan Value:** Total loan value reached 43.43M in 2022, while approved loan value peaked at 14.77M in 2021.
- **Monthly Activity:** August recorded the highest loan collection activity, with May to August showing notable activity across age groups.

## 6. Model Performance and Recommendations

The Random Forest model was evaluated using accuracy, a confusion matrix and a classification report.

**Model Evaluation Results**

| Evaluation Metric | Result |
|---|---:|
| Accuracy | 31.8% |
| Macro Precision | 32% |
| Macro Recall | 32% |
| Macro F1-score | 31% |
| Weighted F1-score | 32% |

**Confusion Matrix**

| Actual / Predicted | Approved | Closed | Rejected |
|---|---:|---:|---:|
| Approved | 133 | 142 | 96 |
| Closed | 119 | 104 | 88 |
| Rejected | 132 | 105 | 81 |

The model achieved an accuracy of 31.8%, indicating limited classification performance across the three loan-status categories. Further development would be necessary before considering its use in practical loan assessment.

**Recommendations**

1. Improve customer experience by investigating the relatively low proportion of positive feedback.
2. Strengthen transaction monitoring to identify unusual transaction patterns.
3. Further investigate demographic and loan product patterns to support lending decisions.
4. Improve predictive performance through feature engineering and experimentation with alternative classification algorithms.

## 7. Project Files

The project repository contains the following supporting materials:

- **Power BI Dashboard:** Interactive dashboard file (`.pbix`).
- **Python Notebook:** Jupyter Notebook (`.ipynb`) containing the machine learning process.
- **Dashboard Screenshots:** Images showing the two dashboard pages.

*Note: Raw datasets are excluded where sharing is restricted or where they contain confidential or personally identifiable information.*
