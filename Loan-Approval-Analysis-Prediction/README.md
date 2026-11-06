# Loan Approval Analysis & Prediction

**Tools:** Power BI | Power Query | Python | Pandas | Scikit-learn

## 1. Project Overview

The objective of this project was to analyze banking and loan-related data to identify patterns associated with loan approval decisions and customer activities.

The analysis focused on customer demographics, loan characteristics, interest rates, transaction anomalies and customer feedback. It also involved experimenting with a machine learning model to classify loan status.

The project demonstrates how data analytics and machine learning techniques can support data-driven decision-making in the financial sector.

## 2. Tools and Technologies

- **Power BI:** Dashboard development and data visualization.
- **Power Query:** Data cleaning and transformation.
- **Python:** Data exploration and predictive modelling.
- **Pandas:** Data manipulation and analysis.
- **Scikit-learn:** Random Forest classification and model evaluation.
- **Jupyter Notebook:** Python development environment.

## 3. Dataset Overview

The project involved banking and loan-related data covering:

- Customer and account information.
- Transaction records.
- Loan applications and loan characteristics.
- Credit card information.
- Customer feedback.
- Transaction anomalies.

For the machine learning experiment, a dataset containing 5,000 records was used.

The modelling exercise focused on the following variables:

- Age
- City
- Loan Amount
- Loan Type
- Interest Rate
- Loan Term
- Loan Status

The target variable was **Loan Status**, consisting of three categories: Approved, Closed and Rejected.

Personal identifiers and contact information were excluded from the modelling dataset.

Raw source data containing personal information is not included in this repository.

## 4. Methodology

The project involved the following activities:

**Data Preparation**

- Reviewed data types, missing values and duplicate records.
- Cleaned and transformed relevant data using Power Query.
- Selected relevant variables for the machine learning experiment.
- Applied One-Hot Encoding to categorical predictors.

**Data Analysis**

- Examined loan approval patterns across customer demographics and loan categories.
- Analyzed interest rate trends and monthly loan activity.
- Investigated customer feedback and transaction anomalies.

**Predictive Modelling**

- Used Python, Pandas and Scikit-learn.
- Developed a Random Forest classification model.
- Split the dataset into 80% training data and 20% testing data.
- Generated predictions for the three loan-status categories.
- Compared model performance against a baseline classifier.

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

## 6. Model Performance and Evaluation

A Random Forest classifier was developed to predict loan status across three categories: Approved, Closed and Rejected.

The model was evaluated using accuracy, a classification report and a confusion matrix.

**Model Performance Comparison**

| Evaluation Metric | Random Forest | Baseline Model |
|---|---:|---:|
| Accuracy | 31.20% | 34.20% |

The classification report for the Random Forest model produced the following results:

| Class | Precision | Recall | F1-score |
|---|---:|---:|---:|
| Approved | 0.34 | 0.39 | 0.36 |
| Closed | 0.31 | 0.33 | 0.32 |
| Rejected | 0.26 | 0.22 | 0.24 |
| Macro Average | 0.31 | 0.31 | 0.31 |
| Weighted Average | 0.31 | 0.31 | 0.31 |

**Confusion Matrix**

| Actual / Predicted | Approved | Closed | Rejected |
|---|---:|---:|---:|
| Approved | 132 | 111 | 99 |
| Closed | 121 | 108 | 103 |
| Rejected | 130 | 124 | 72 |

**Model Interpretation**

The Random Forest classifier achieved an accuracy of 31.20%, compared with 34.20% from the baseline model.

This indicates that the Random Forest model did not outperform the baseline classifier. The selected features may not contain sufficient predictive information to reliably distinguish between the three loan-status categories.

The experiment highlights the importance of comparing machine learning models against simple baseline approaches rather than relying on accuracy alone.

Further investigation, feature engineering and experimentation with alternative algorithms would be necessary before considering the model suitable for practical loan assessment.

## 7. Recommendations

1. Improve customer experience by investigating the relatively low proportion of positive feedback.
2. Strengthen transaction monitoring to identify unusual transaction patterns.
3. Further investigate demographic and loan product patterns to support lending decisions.
4. Explore additional features and alternative classification algorithms to improve predictive performance.
5. Evaluate models against appropriate baseline approaches before considering practical deployment.

## 8. Project Files

The project repository contains the following supporting materials:

- **Power BI Dashboard:** Interactive dashboard file (`.pbix`).
- **Python Notebook:** Jupyter Notebook (`.ipynb`) containing the machine learning workflow.
- **HTML Notebook:** Browser-readable version of the Python notebook.
- **Dashboard Screenshots:** Images showing the Power BI dashboard pages.

*Note: Raw datasets are excluded where sharing is restricted or where they contain confidential or personally identifiable information.*
