---
title: "Exploratory Data Analysis on The Titanic Dataset"
date: 2025-11-29 12:00:00 +0300
categories: [Data Science, EDA]
tags: [python, kaggle, titanic, eda, visualization]
image:
  path: /assets/titanic-banner.png
  width: 1200
  height: 600
---

## Overview

This project explores the **Titanic dataset** using Python and Kaggle Notebook.  
The goal was to understand survival patterns through **univariate, bivariate, multivariate**, and **target-variable analysis**.

🔗 **Kaggle Notebook:**  
[View full code here](YOUR_KAGGLE_LINK_HERE)

---

## Tools Used

- **Python**
- **Pandas** – data manipulation  
- **NumPy** – numerical operations  
- **Matplotlib & Seaborn** – visualizations  
- **Missingno** – missing data visualization  
- **SciPy** – winsorizing / statistical tools  
- **Kaggle Notebook** – environment

---

## Data Understanding

The Titanic dataset contains variables such as:

- Passenger Class  
- Name, Sex, Age  
- Number of Siblings/Spouses  
- Parents/Children  
- Fare  
- Cabin  
- Survival target variable

Initial checks included:

- Checking dimensions
- Data types
- Missing values (using `missingno.bar`)



---

## Univariate Analysis

I explored the distribution of single variables:

- Age distribution  
- Fare distribution  
- Survival rate  
- Passenger class  
- Gender

Key findings:
- The dataset has significant **missing Age values**.
- Most passengers traveled in **3rd class**.
- More men than women were on board.

[!age_distribution](/assets/distribution_of_age(1).png)
---

## Bivariate Analysis

Focus: relationship between two variables.

Examples:

- **Sex vs Survival**  
- **Pclass vs Survival**  
- **SibSp vs Survival**

Findings:
- Females had a significantly higher survival probability.  
- First-class passengers survived more than third-class.  
- Having many siblings/spouses reduced survival chances.

---

## Multivariate Analysis

Here I looked at combinations like:

- **Pclass + Sex + Survival**
- **Age + Fare + Survival**

Insights:
- Young passengers in higher classes had better survival outcomes.  
- Older adults in 3rd class had the lowest survival probability.

---

## Data Cleaning Steps

Actions taken:

- Dropped irrelevant columns (`PassengerId`, `Name`)  
- Handled missing values  
- Visualized missingness  
- Performed winsorization/feature capping  
- Normalized/standardized distributions where necessary  

---

## Key Insights

- Survival strongly depends on **gender** and **passenger class**.  
- Children had better survival chances than adults.  
- High fare values correlated with higher survival.
- Missing cabin information is extremely common (over 75%).

---

## Conclusion

This EDA provided clear survival patterns and highlighted which variables matter most.

🔗 **Full notebook & code**:  
[View on Kaggle](https://www.kaggle.com/code/annwairimukiarie/ann-kiarie-eda)

---

## What’s Next

- Feature engineering for ML modeling  
- Building a prediction model  
- Hyperparameter tuning
