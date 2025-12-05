# Impact Analysis of Age and Gender on COVID-19 Mortality Rates

This repository contains the full analysis, cleaned data, statistical modeling, and written report for the project **“Impact Analysis of Age and Gender on COVID-19 Mortality Rates.”** The study examines how age and gender shape COVID-19 mortality patterns in the United States using CDC public health records. The analysis integrates **statistical inference**, **data visualization**, and **baseline machine learning models** to evaluate demographic risk factors.

The complete written report is included in: **annotated-final.pdf**

---

## Overview

Understanding how demographic factors influence COVID-19 mortality is essential for designing targeted public health interventions.  
This project investigates three core questions:

- How strongly age is associated with COVID-19 mortality  
- Whether gender differences are statistically significant  
- Whether simple predictive models can capture mortality patterns within the highest-risk age group  

The project includes rigorous data cleaning, exploratory data analysis, hypothesis testing, and baseline machine learning.

---

## Research Questions

### 1. Relationship Between Age and Mortality
COVID-19 mortality increases sharply with age. The age groups **65–74**, **75–84**, and **85+** show the highest mortality, with **85+** being the most vulnerable.

### 2. Gender Differences
Although males exhibit higher observed mortality,  
**statistical testing shows no significant gender differences** within age groups (p > 0.05).

### 3. Predictive Modeling for the 85+ Age Group
Models tested:

- Logistic Regression  
- Decision Tree  
- Random Forest  

Accuracy was low due to high variability and limited features, indicating that more complex predictors are required.

---

## Methods

### Data Cleaning
- Selected key variables  
- Standardized categorical encodings  
- Removed missing values  
- Produced cleaned dataset (`cleaned_covid_mortality_data.csv`)

### Exploratory Data Analysis
- Mortality by age  
- Mortality by gender  
- Boxplots and bar charts  
- Identification of high-risk groups  

### Statistical Analysis
- Two-sample t-tests within each age group  
- 95% confidence intervals  
- Effect-size evaluation  

### Machine Learning
- Training on the 85+ subgroup  
- Evaluation using accuracy, confusion matrix, and classification report  

---

## Key Findings

- **Age** is the strongest determinant of COVID-19 mortality  
- **Gender differences are not statistically significant**  
- **Predictive models** fail to capture mortality complexity with demographic features alone  



---

## Data Source
United States Centers for Disease Control and Prevention (CDC)  
Provisional COVID-19 Deaths by Sex and Age Dataset

---

## Author
**Shuozishan (Doris) Wang**  
B.S. Applied Statistics, University of Washington  



