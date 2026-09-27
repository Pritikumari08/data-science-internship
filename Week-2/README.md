# Week 2 – Exploratory Data Analysis (EDA) and Visualization Framework Design

## Project Title

### Customer Churn Analysis and Prediction

## Objective

The objective of this task is to design a comprehensive framework for Exploratory Data Analysis (EDA) and data visualization for a hypothetical customer churn analysis and prediction project.

This task focuses on planning the EDA process, identifying suitable analysis techniques, selecting appropriate visualization methods, and defining how results would be documented and communicated.

No real dataset is used in this task because the focus is on designing a reusable EDA and visualization framework.

---

## Project Context

The hypothetical project focuses on understanding customer churn and identifying patterns that may be associated with customers discontinuing a company's products or services.

EDA would be used to understand the structure and quality of customer-related data before applying machine learning techniques.

The planned analysis may consider variables such as:

- Customer tenure
- Contract type
- Monthly charges
- Total charges
- Payment method
- Service usage
- Customer demographics
- Customer support interactions
- Churn status

---

## What is Exploratory Data Analysis?

Exploratory Data Analysis (EDA) is the process of examining and understanding a dataset before performing advanced statistical analysis or machine learning.

EDA helps identify:

- Data structure
- Data types
- Missing values
- Duplicate records
- Outliers
- Distributions
- Relationships between variables
- Patterns and trends
- Potentially useful features

---

## EDA Process

The planned EDA process consists of the following stages:

1. Understand the dataset
2. Inspect data types and structure
3. Perform data-quality checks
4. Identify missing values
5. Detect and investigate outliers
6. Perform univariate analysis
7. Perform bivariate analysis
8. Perform multivariate analysis
9. Create appropriate visualizations
10. Document important observations
11. Prepare insights for future modeling

---

## Potential Data Types

The framework considers different types of data that may occur in a dataset.

| Data Type | Example |
|-----------|---------|
| Numerical | Age, Monthly Charges, Tenure |
| Categorical | Contract Type, Payment Method |
| Binary | Churn: Yes/No |
| Date/Time | Signup Date, Service Date |
| Text | Customer Feedback or Comments |

Understanding data types helps determine which EDA and visualization techniques should be applied.

---

## Data Quality Checks

Before performing analysis, the following checks are planned:

- Dataset shape
- Column names
- Data types
- Missing values
- Duplicate records
- Unique values
- Invalid values
- Inconsistent categories
- Extreme values
- Basic statistical summaries

These checks help establish the quality and reliability of the data before further analysis.

---

## Missing Data Handling

Missing data will be handled using the following framework:

### 1. Identify

Determine which columns contain missing values and measure their frequency.

### 2. Investigate

Understand why values may be missing and whether missingness follows a pattern.

### 3. Select an Approach

Depending on the situation, possible approaches may include:

- Removing records
- Removing unnecessary columns
- Mean or median imputation
- Mode imputation
- Appropriate categorical replacement

### 4. Document

The selected method and its reason should be recorded in the final EDA documentation.

---

## Outlier Detection and Handling

Outliers are unusual observations that may significantly differ from the majority of values.

Planned techniques include:

- Box plots
- Interquartile Range (IQR)
- Statistical summaries
- Distribution analysis

Outliers should be investigated before deciding whether they should be removed, transformed, capped, or retained.

---

# Univariate Analysis

Univariate analysis studies one variable at a time.

| Variable Type | Planned Technique | Visualization |
|---------------|------------------|---------------|
| Numerical | Distribution analysis | Histogram |
| Numerical | Spread analysis | Box Plot |
| Categorical | Frequency analysis | Bar Chart |
| Binary | Category distribution | Count Plot |

The objective is to understand the distribution, frequency, spread, and unusual values of individual variables.

---

# Bivariate Analysis

Bivariate analysis examines the relationship between two variables.

| Variables | Planned Technique | Visualization |
|-----------|------------------|---------------|
| Numerical + Numerical | Correlation/relationship | Scatter Plot |
| Categorical + Numerical | Group comparison | Box Plot |
| Categorical + Categorical | Frequency comparison | Bar Chart |
| Time + Numerical | Trend analysis | Line Chart |

For example, the relationship between customer tenure and monthly charges could be explored using a scatter plot.

---

# Multivariate Analysis

Multivariate analysis examines relationships among three or more variables.

Planned techniques include:

- Correlation analysis
- Pair plots
- Grouped comparisons
- Multi-variable visualizations
- Heatmaps

Multivariate analysis can help identify interactions and patterns that may not be visible when variables are analyzed individually.

---

# Visualization Strategies

Different visualizations will be selected according to the type and purpose of analysis.

| Visualization | Purpose |
|---------------|---------|
| Histogram | Understand numerical distribution |
| Bar Chart | Compare categories |
| Count Plot | Show category frequency |
| Box Plot | Identify spread and outliers |
| Scatter Plot | Study relationships between numerical variables |
| Line Chart | Analyze trends over time |
| Heatmap | Visualize correlations |
| Pair Plot | Explore relationships among multiple numerical variables |
| Interactive Plot | Explore data dynamically |

The choice of visualization should depend on the data type and the analytical question being addressed.

---

# Python Tools and Libraries

The planned Python tools and libraries are:

| Tool / Library | Purpose |
|----------------|---------|
| Python | Primary programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical operations |
| Matplotlib | Basic data visualization |
| Seaborn | Statistical visualization |
| Plotly | Interactive visualization |
| Jupyter Notebook | Analysis and documentation environment |

---

# EDA and Visualization Workflow

The planned workflow is:

Dataset Understanding
        ↓
Data Quality Checks
        ↓
Missing Value Analysis
        ↓
Outlier Detection
        ↓
Univariate Analysis
        ↓
Bivariate Analysis
        ↓
Multivariate Analysis
        ↓
Visualization
        ↓
Observation & Insight Documentation
        ↓
EDA Report
