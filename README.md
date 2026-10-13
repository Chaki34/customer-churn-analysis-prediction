# Customer Churn Analysis & Prediction

<p align="center">
  <img src="https://img.shields.io/badge/Python-Data%20Analytics-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python Data Analytics"/>
  <img src="https://img.shields.io/badge/Google-Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" alt="Google Colab"/>
  <img src="https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy"/>
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas"/>
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-11557C?style=for-the-badge" alt="Matplotlib"/>
</p>

<p align="center">
  <b>Turning Customer Data into Actionable Business Insights</b>
  <br/>
  Exploratory Data Analysis · Data Mining · Customer Segmentation · Risk Scoring
</p>

<p align="center">
  <a href="https://github.com/Chaki34/customer-churn-analysis-prediction">
    <img src="https://img.shields.io/badge/GitHub-View%20Repository-181717?style=flat-square&logo=github" alt="View GitHub Repository"/>
  </a>
  <a href="https://www.kaggle.com/datasets/blastchar/telco-customer-churn">
    <img src="https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=flat-square&logo=kaggle&logoColor=white" alt="Kaggle Dataset"/>
  </a>
  <a href="https://colab.research.google.com/">
    <img src="https://img.shields.io/badge/Open%20Environment-Google%20Colab-F9AB00?style=flat-square&logo=googlecolab&logoColor=white" alt="Google Colab"/>
  </a>
</p>

---

## Overview

Customer churn occurs when customers stop using a company's products or services. Understanding why customers leave helps businesses improve customer satisfaction, strengthen retention strategies, and make better decisions.

This project analyzes the **IBM Telco Customer Churn dataset** using Python. It explores customer characteristics, identifies churn-related patterns, compares customer groups, and develops a simple rule-based customer risk score.

The project transforms raw customer data into meaningful visualizations and business recommendations using **NumPy, Pandas, and Matplotlib**.

**Current scope:** Data analytics and data mining. No machine learning model is trained in this version.

## Project at a Glance

| Component       | Description                                     |
| --------------- | ----------------------------------------------- |
| Domain          | Data Analytics and Data Mining                  |
| Language        | Python                                          |
| Environment     | Google Colab                                    |
| Data processing | Pandas and NumPy                                |
| Visualization   | Matplotlib                                      |
| Dataset         | IBM Telco Customer Churn                        |
| Risk assessment | Rule-based customer risk score                  |
| Final output    | Findings dashboard and business recommendations |

## Visual Preview

### Customer Churn Findings Dashboard

The final dashboard consolidates important metrics, churn patterns, risk-score analysis, and possible business solutions into a single visual report.

<p align="center">
  <img src="customer_churn_findings_dashboard.png" alt="Customer Churn Findings Dashboard" width="100%"/>
</p>

> **To display the dashboard:** Run the final dashboard cell in Google Colab, download `customer_churn_findings_dashboard.png`, and upload the image to the root of this GitHub repository. If the image has not been uploaded yet, this preview will remain unavailable.

## Objectives

* Understand the dataset's structure, features, and quality.
* Identify missing values, duplicates, and inconsistent data types.
* Measure the overall customer churn rate.
* Investigate churn patterns across contract types, tenure, internet services, and technical support.
* Explore statistical relationships between numerical variables.
* Segment customers using relevant characteristics.
* Create a rule-based risk score for exploratory analysis.
* Visualize findings in a consolidated Matplotlib dashboard.
* Recommend practical strategies for customer retention.

## Dataset

**IBM Telco Customer Churn**

Source: [Download or explore the dataset on Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

The commonly distributed dataset contains approximately **7,043 customer records and 21 original columns**. The exact number of records and columns should be confirmed from the dataset version loaded in the notebook.

### Important features

| Feature           | Description                              |
| ----------------- | ---------------------------------------- |
| `customerID`      | Unique customer identifier               |
| `gender`          | Customer gender                          |
| `SeniorCitizen`   | Senior-citizen indicator                 |
| `Partner`         | Whether the customer has a partner       |
| `Dependents`      | Whether the customer has dependents      |
| `tenure`          | Customer subscription duration in months |
| `InternetService` | Internet service category                |
| `TechSupport`     | Technical support subscription status    |
| `Contract`        | Customer contract type                   |
| `PaymentMethod`   | Customer payment method                  |
| `MonthlyCharges`  | Monthly service charges                  |
| `TotalCharges`    | Accumulated customer charges             |
| `Churn`           | Whether the customer left the service    |

The notebook can load the data directly from a public CSV source, avoiding a manual download:

```python
import pandas as pd

url = (
    "https://raw.githubusercontent.com/IBM/"
    "telco-customer-churn-on-icp4d/master/data/"
    "Telco-Customer-Churn.csv"
)

df = pd.read_csv(url)

print("Dataset shape:", df.shape)
display(df.head())
```

## Technology Stack

<p align="center">
  <img src="https://cdn.simpleicons.org/python/3776AB" width="58" alt="Python"/>
  &nbsp;&nbsp;
  <img src="https://cdn.simpleicons.org/numpy/013243" width="58" alt="NumPy"/>
  &nbsp;&nbsp;
  <img src="https://cdn.simpleicons.org/pandas/150458" width="58" alt="Pandas"/>
  &nbsp;&nbsp;
  <img src="https://cdn.simpleicons.org/googlecolab/F9AB00" width="58" alt="Google Colab"/>
</p>

* **Python:** Main programming language.
* **NumPy:** Numerical calculations, array operations, and statistical measures.
* **Pandas:** Data loading, cleaning, grouping, transformation, and analysis.
* **Matplotlib:** Statistical charts, comparisons, and the final dashboard.
* **Google Colab:** Cloud-based notebook environment for executing and documenting the project.

## Project Workflow

The notebook follows a structured analytics workflow.

```text
Data Collection
      |
      v
Data Understanding
      |
      v
Data Cleaning & Preprocessing
      |
      v
Exploratory Data Analysis
      |
      v
Statistical & Correlation Analysis
      |
      v
Customer Segmentation & Data Mining
      |
      v
Rule-Based Customer Risk Score
      |
      v
Visual Findings Dashboard
      |
      v
Business Recommendations
```

### 1. Data collection and understanding

* Load the customer dataset.
* Inspect rows, columns, data types, and sample records.
* Understand the meaning of relevant features.

### 2. Data cleaning and preprocessing

* Check for missing values and duplicate records.
* Correct inconsistent data types where necessary.
* Prepare the dataset for reliable analysis.
* Convert `TotalCharges` to a numeric data type if required.

### 3. Exploratory Data Analysis

Explore customer distributions and churn patterns using:

* Univariate analysis.
* Bivariate analysis.
* Multivariate analysis.
* Descriptive statistics.
* Numerical and categorical comparisons.

### 4. Statistical and correlation analysis

Calculate summary statistics and examine relationships between numerical features such as tenure, monthly charges, total charges, and churn status.

Correlation indicates association; it does not establish causation.

### 5. Data mining and customer segmentation

Group customers by selected characteristics and compare their observed churn rates to identify potentially important customer segments.

### 6. Customer risk scoring

Calculate a simple risk score using four selected conditions:

| Condition                                | Points |
| ---------------------------------------- | -----: |
| Month-to-month contract                  |     +1 |
| Tenure of 12 months or less              |     +1 |
| Monthly charges above the dataset median |     +1 |
| No technical support                     |     +1 |

The resulting score ranges from **0 to 4**. The analysis compares actual churn rates across score groups.

This is a rule-based analytical indicator, not a validated prediction of future customer behavior.

## Key Findings and Business Value

The notebook investigates the following questions:

* What percentage of customers have churned?
* Which contract types have higher observed churn rates?
* How does churn vary with customer tenure?
* How does technical support relate to churn?
* Do monthly charges differ between churned and retained customers?
* How do observed churn rates vary across risk-score groups?

Actual numerical findings should be taken from the executed notebook and dashboard, rather than assumed in advance.

## Business Recommendations

Based on the patterns identified in the analysis, businesses can consider:

1. **Customer retention:** Investigate customer groups with higher observed churn and develop targeted retention campaigns.
2. **Contract incentives:** Test suitable benefits for customers considering longer-term contracts.
3. **Early customer engagement:** Improve onboarding and support for customers with short tenure.
4. **Technical support:** Investigate unresolved issues and improve response times.
5. **Billing experience:** Review pricing concerns and billing clarity.
6. **Risk monitoring:** Track churn rates across rule-based risk groups over time and assess whether retention actions are effective.

These recommendations are hypotheses for business action. Their effectiveness should be measured using subsequent customer outcomes.

## How to Run the Project

### Option 1: Google Colab

1. Open [Google Colab](https://colab.research.google.com/).

2. Select **File → Open notebook → GitHub**.

3. Enter the repository URL:

   `https://github.com/Chaki34/customer-churn-analysis-prediction`

4. Select the project notebook, if it has been committed.

5. Run the notebook cells in order, beginning with data loading.

6. Review the analysis outputs and execute the final dashboard cell.

If the repository does not yet contain a notebook, create a new Colab notebook and save it to GitHub using **File → Save a copy in GitHub**.

### Option 2: Run locally

Clone the repository:

```bash
git clone https://github.com/Chaki34/customer-churn-analysis-prediction.git
cd customer-churn-analysis-prediction
```

Install the required libraries:

```bash
pip install numpy pandas matplotlib jupyter
```

Launch Jupyter:

```bash
jupyter notebook
```

Open the project notebook and execute the cells in order. A local Python environment and internet access are required for loading the online dataset.

## Repository Structure

The intended repository structure is:

```text
customer-churn-analysis-prediction/
│
├── customer_churn_analysis.ipynb
├── customer_churn_findings_dashboard.png
├── README.md
└── requirements.txt
```

The dashboard image should be added after it has been generated. Update the notebook filename in this README if your actual file uses a different name.

Example `requirements.txt`:

```text
numpy
pandas
matplotlib
```

## Learning Outcomes

This project provides practical experience in:

* Python-based data analysis.
* Data cleaning and preprocessing.
* NumPy numerical operations.
* Pandas filtering, grouping, and aggregation.
* Exploratory data analysis.
* Descriptive statistics and correlation.
* Customer segmentation and rule-based risk scoring.
* Matplotlib dashboard development.
* Communicating analytical findings and business recommendations.

## Future Improvements

Possible extensions include more detailed customer segmentation, additional visualizations, automated reporting, and a separate machine learning model if predictive churn modeling becomes a future objective.

## Author

**Debmalya Chaki**

B.Tech Computer Science and Engineering Student | Aspiring Data Scientist | Software Developer

* GitHub Profile: [@Chaki34](https://github.com/Chaki34)
* Project Repository: [Customer Churn Analysis & Prediction](https://github.com/Chaki34/customer-churn-analysis-prediction)

---

<p align="center">
  <b>Analyze Data. Discover Patterns. Make Better Decisions.</b>
</p>
