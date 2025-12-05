📊 Impact Analysis of Age and Gender on COVID-19 Mortality Rates

This repository contains all analysis, code, datasets, and the final project report for “Impact Analysis of Age and Gender on COVID-19 Mortality Rates.”
The project investigates how age and gender influence variation in COVID-19 mortality in the United States using CDC data.

📄 Full report: annotated-final.pdf (uploaded in this repo)

🔍 Research Questions
1️⃣ Is age correlated with COVID-19 mortality?

Yes — mortality increases sharply with age.
Age groups 65–74, 75–84, and 85+ show the highest deaths.

2️⃣ Are mortality rates significantly different for males vs. females?

Although males consistently show higher raw mortality counts,
t-tests indicate no statistically significant gender differences across all age groups (p > 0.05).

3️⃣ Within the highest-risk age group (85+), what factors influence mortality?

The 85+ group shows extremely high mortality and high variability.
Machine learning models (Logistic Regression, Decision Tree, Random Forest) were trained but produced low predictive accuracy due to high variance and limited features.

📂 Project Structure
.
├── data/
│   └── Provisional_COVID-19_Deaths_by_Sex_and_Age.csv
├── cleaned_covid_mortality_data.csv
├── notebook/
│   └── covid_analysis.ipynb
├── annotated-final.pdf
└── README.md

📈 Key Findings
Age Trends

Mortality is extremely age-dependent.

85+ has the highest total deaths.

Children and adolescents show extremely low mortality.

Gender Trends

Males have higher observed deaths in nearly every age group.

However, t-tests show no statistically significant difference between male and female mortality within age groups.

Machine Learning Results

Models trained on the highest-risk age group show:

Accuracy ~ 8% (very low)

Death counts have hundreds of distinct values, making classification challenging

Random Forest and Decision Tree outperform Logistic Regression but still weak overall

🛠️ Methods
Data Processing

Removed missing values

Converted categorical variables (Age Group, Sex)

Exported cleaned dataset for downstream use

Statistical Analysis

Grouped by age and gender

Descriptive statistics

Boxplots and bar charts

Independent two-sample t-tests

95% confidence intervals for mortality rate differences

Machine Learning

Models used:

Logistic Regression

Decision Tree Classifier

Random Forest Classifier

Evaluation metrics:

Accuracy

Classification Report

Confusion Matrix

📊 Visualizations Generated

Total COVID-19 deaths by age group

Mortality boxplots by gender

Mortality rate bar charts with 95% confidence intervals
