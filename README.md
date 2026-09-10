# HR Employee Attrition Analysis

An exploratory data analysis and logistic regression model examining 
factors associated with employee attrition, using IBM's HR Analytics 
Employee Attrition & Performance dataset from Kaggle.

**[View the full report here](https://aryakumaradhikary-ship-it.github.io/IBM-Attrition/index.html)**

## Contents
- `IBM.Rmd` — full R Markdown analysis (code + narrative)
- `IBM.html` — knitted report (open in a browser to view)
- `WA_Fn-UseC_-HR-Employee-Attrition(in).csv` — dataset (source: [Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset))

## What's in the analysis
- Missing data check
- Attrition patterns by department, overtime, income, and job satisfaction
- A logistic regression model predicting attrition, with odds ratio interpretation
- A discussion of class imbalance and classification threshold trade-offs

## Key findings
- Overtime was the strongest predictor of attrition — employees who work 
  overtime are about 4.4x more likely to leave.
- Job satisfaction, income, and age were also significant predictors.
- Department's apparent effect disappeared once other factors were controlled 
  for in the model.
- The model's overall accuracy (84.6%) was misleading due to class imbalance; 
  lowering the classification threshold improved recall at the cost of more 
  false positives.

## Tools
R, tidyverse (dplyr, ggplot2), R Markdown
