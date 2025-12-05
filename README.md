Impact Analysis of Age and Gender on COVID-19 Mortality Rates

This repository contains the full analysis, code, and documentation for the project “Impact Analysis of Age and Gender on COVID-19 Mortality Rates.”
The study examines how age and gender shape COVID-19 mortality patterns in the United States using publicly available CDC data.
The analysis integrates statistical inference, data visualization, and machine learning modeling to evaluate demographic risk factors.

The complete written project report is provided in: annotated-final.pdf.

Overview

Understanding how demographic factors influence COVID-19 mortality is essential for designing targeted public health interventions. This project explores:

The strength of the relationship between age and COVID-19 mortality

Whether gender differences in mortality are statistically significant

Whether simple predictive models can capture mortality patterns within the highest-risk age group

The project employs rigorous data cleaning, exploratory data analysis, hypothesis testing, and baseline machine learning models.

Research Questions
1. How strongly is age associated with COVID-19 mortality?

COVID-19 mortality increases monotonically with age.
The highest mortality counts occur in the 65–74, 75–84, and 85+ age groups.
The 85+ age group exhibits the most pronounced risk.

2. Are mortality differences between males and females statistically significant?

Although males consistently exhibit higher raw mortality counts,
independent two-sample t-tests show no statistically significant differences between male and female mortality within each age group (p > 0.05).

3. Within the highest-risk age group (85+), can mortality patterns be modeled using machine learning?

Baseline models (Logistic Regression, Decision Tree, Random Forest) were evaluated.
Model accuracy remained low due to:

High variance in mortality counts

Limited available features

A large number of distinct target values

This suggests that more complex feature sets or regression-based modeling would be necessary for meaningful prediction.

Methodology
Data Cleaning

Selected key variables: Sex, Age Group, COVID-19 Deaths

Removed rows with missing demographic information

Standardized categorical encodings for age and gender

Exported a cleaned dataset (cleaned_covid_mortality_data.csv)

Exploratory Data Analysis

Summarized deaths across age categories

Generated bar plots to visualize mortality trends

Created gender-stratified boxplots to compare distributions

Identified high-risk demographic segments

Statistical Hypothesis Testing

Performed gender comparison using two-sample t-tests within each age group

Calculated 95% confidence intervals for mortality rates

Assessed statistical significance and effect size

Machine Learning Modeling

Focused on the highest-risk age group: 85+

Encoded categorical variables and created dummy features

Trained and evaluated:

Logistic Regression

Decision Tree Classifier

Random Forest Classifier

Assessed using:

Accuracy

Classification report

Confusion matrix

The modeling results underscore the complexity of predicting mortality counts using limited demographic variables alone.

Key Findings
Age as a Primary Risk Factor

Age is the strongest determinant of COVID-19 mortality, with risk increasing exponentially among older adults.

Gender Differences Are Not Statistically Significant

Observed differences between male and female mortality are not significant under formal hypothesis testing.

Predictive Modeling Limitations

Baseline models fail to capture meaningful patterns in mortality within the oldest age group, suggesting the need for:

Additional clinical or socioeconomic predictors

Alternative modeling frameworks (e.g., regression, survival analysis)

Project Structure

.
├── data/
│ └── Provisional_COVID-19_Deaths_by_Sex_and_Age.csv
├── cleaned_covid_mortality_data.csv
├── notebook/
│ └── covid_analysis.ipynb
├── annotated-final.pdf
└── README.md

data/: Raw CDC dataset

covid_analysis.ipynb: Full Python workflow (cleaning → EDA → tests → ML models)

annotated-final.pdf: Final polished written report

How to Run the Project
1. Clone the repository

git clone https://github.com/yourusername/yourrepo.git

cd yourrepo

2. Install required packages

pip install -r requirements.txt

3. Open the Jupyter Notebook

jupyter notebook

4. Run covid_analysis.ipynb to reproduce all results.
Data Source

United States Centers for Disease Control and Prevention (CDC)
Provisional COVID-19 Deaths by Sex and Age (Public Dataset)

Author

Shuozishan (Doris) Wang
B.S. in Applied Statistics
University of Washington, Seattle

