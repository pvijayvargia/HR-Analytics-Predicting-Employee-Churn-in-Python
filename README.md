# HR-Analytics-Predicting-Employee-Churn-in-Python

# Employee Attrition Analysis

## Project Overview

This project aims to analyze employee attrition (also referred to as churn) within a company. Using a dataset that includes various employee attributes, the goal is to identify key factors that influence employee attrition and develop a predictive model to help the company understand and mitigate employee turnover. The analysis is performed using a decision tree classifier to leverage its interpretability and ability to handle both categorical and numerical data.

## Dataset Description

The dataset used in this project is `turnover.csv`, which contains the following columns:
- **satisfaction_level**: Employee satisfaction level
- **last_evaluation**: Last evaluation score
- **number_project**: Number of projects completed
- **average_montly_hours**: Average monthly working hours
- **time_spend_company**: Number of years spent in the company
- **Work_accident**: Whether the employee had a work accident (0 or 1)
- **promotion_last_5years**: Whether the employee was promoted in the last 5 years (0 or 1)
- **department**: Employee's department
- **salary**: Employee's salary level (low, medium, high)
- **churn**: Whether the employee left the company (0 or 1)

## Project Steps

1. **Data Exploration**
   - Load the dataset and inspect the first few rows.
   - Print the unique values in the `department` and `salary` columns.

2. **Data Preprocessing**
   - Convert the `salary` column to categorical type with a specified order (low, medium, high).
   - Apply one-hot encoding to the `department` column and drop the original column to avoid the dummy variable trap.
   - Join the encoded department data back to the main dataset.

3. **Attrition Analysis**
   - Calculate the overall attrition rate within the company.
   - Identify departments with higher attrition rates by calculating the mean attrition rate per department.

4. **Feature Engineering**
   - Split the dataset into training and testing sets.
   - Train a decision tree classifier on the training data.
   - Calculate and sort feature importances to identify key predictors of attrition.

5. **Model Evaluation**
   - Evaluate the model's accuracy, recall, and ROC/AUC scores to understand its performance.
  
6. **Insights and Recommendations**
   - Based on the analysis, identify high attrition departments and key factors influencing employee turnover.
   - Provide actionable recommendations to improve employee retention.

## Key Findings

- **Overall Attrition Rate**: Approximately 23.81% of employees have left the company.
- **High Attrition Departments**: Departments such as accounting, IT, and support exhibit higher attrition rates.
- **Important Features**: Satisfaction level, last evaluation, and number of projects are the top predictors of employee attrition.
- **Impact of Salary**: Although salary is a factor, it is not as significant as employee satisfaction and performance evaluations.

## Recommendations

1. **Targeted Retention Strategies**:
   - Focus on departments with high attrition rates to address specific issues such as workload and job satisfaction.
2. **Improve Employee Satisfaction**:
   - Implement programs to boost employee morale and job satisfaction, such as recognition initiatives and career development opportunities.
3. **Review Salary Structures**:
   - Ensure competitive and fair salary packages, especially for employees in lower salary categories.

