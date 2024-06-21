# Employee Attrition Analysis

## Overview

This repository contains an analysis of employee attrition using a fictional dataset provided by IBM data scientists. The dataset aims to identify significant factors contributing to employee attrition and to develop strategies for reducing turnover rates. The analysis includes exploratory data analysis, statistical modeling, and insights into how various factors influence employee attrition.

## Report Contents

### 1. Introduction

- **Dataset**:
  - The dataset is sourced from Kaggle and contains 1,470 rows and 35 columns with no missing data.
  - Dependent Variable: `Attrition` (Yes/No)
  - Independent Variables: Personal Details, Work Life, and Income variables.
  
- **Key Questions**:
  - What is the impact of attrition rate on company reputation?
  - What are the most significant factors in employee attrition?
  - How do pay and time worked at the company affect attrition?
  - What are the differences in attrition between departments?
  - How does distance from home affect attrition? Would remote work efforts help with attrition?
  - Is overtime and work-life balance correlated and how do they affect attrition?

### 2. Data Exploration

- **Dependent Variable**:
  - Attrition is split into "Yes" (16%) and "No" (84%), indicating the percentage of employees leaving or staying with the company.
  
- **Independent Variables**:
  - **Personal Details**: Age, Education, Gender, Marital Status, etc.
  - **Work Life**: Business Travel, Job Role, Job Satisfaction, Overtime, etc.
  - **Income**: Monthly Income, Stock Option Level, Percent Salary Hike, etc.
  
- **Observations**:
  - Younger and single employees have higher attrition rates.
  - Employees in certain roles like Sales and Laboratory Technicians show higher turnover.
  - Distance from home and overtime correlate with higher attrition rates.

### 3. Statistical Modeling

- **Data Splitting**:
  - The data was split into 70% training and 30% testing datasets to evaluate model performance.

- **Models Used**:
  - **Decision Tree**:
    - Achieved 83% accuracy in predicting employee attrition.
    - Key factors: Monthly Income, Overtime, Stock Option Level, Job Level, etc.
  - **Logistic Regression (Logit)**:
    - Identified significant roles and factors affecting attrition, such as Lab Technicians and Sales Representatives.
  - **Support Vector Machine (SVM)**:
    - Achieved 85% accuracy but did not provide insights into which factors were significant.

### 4. Business Questions and Insights

- **Impact on Company Reputation**:
  - Attrition affects company reputation, especially if it involves key roles or specific demographics.
  - Understanding whether attrition is voluntary or involuntary can provide deeper insights.

- **Significant Factors in Attrition**:
  - Monthly Income, Overtime, and Job Level are crucial in determining attrition rates.
  - Single employees and those with high job involvement or overtime are more likely to leave.

- **Pay and Time Worked**:
  - Higher pay correlates with lower attrition rates.
  - Employees with longer tenure and higher salaries tend to stay, though some leave due to retirement.

- **Departmental Differences**:
  - Sales has the highest attrition rate, followed by Human Resources and Research & Development.
  - Specific roles within departments, like Sales Representatives, are more prone to leaving.

- **Distance from Home and Remote Work**:
  - Longer commute distances increase attrition rates.
  - Implementing remote work options could help reduce turnover for employees living farther away.

- **Overtime and Work-Life Balance**:
  - Both factors are linked to attrition, with higher overtime leading to higher turnover.
  - Addressing work-life balance issues can help mitigate attrition.

### 5. Data and Tools

- **Dataset**: [HR Employee Attrition](https://www.kaggle.com/datasets/whenamancodes/hr-employee-attrition?select=HR+Employee+Attrition.csv)
- **Tools**: Python, Pandas, Scikit-learn, Matplotlib, Seaborn, and ggplot2 for visualizations.

## Authors

- Nathaniel Bowen
- Elizabeth Curinga
- Sean Deery
- Mackenzie Houser
- Binosh Padman

## How to Use This Repository

1. **Data Exploration and Analysis**: 
   - Open the `employee-attrition-eda.Rmd`, `employee-attrition-decision-tree.Rmd` and `employee-attrition-neural-network.Rmd` files in RStudio to explore the detailed analysis.
   - Run the R Markdown files to reproduce the visualizations and statistical models used in the analysis.
   
2. **Review the Full Report**: 
   - Access the `employee-attrition-report.docx` file to read the in-depth report on employee attrition, including business insights and recommendations.
   

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

