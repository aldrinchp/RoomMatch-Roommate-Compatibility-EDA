## 📊 Exploratory Data Analysis (EDA) - Roommate Compatibility

## 📋 Overview
This project performs an exploratory data analysis on cohabitation preferences to identify compatibility between potential roommates. The dataset contains 750 records with 15 variables related to habits, personality, and lifestyle preferences.

## 🎯 Main Objective
Identify significant relationships between categorical variables using Chi-square tests and visualize compatibility patterns through bar charts and stacked bar charts.

## 🔧 Main Features
- Chi-square analysis between categorical variables and Cramér's V to determine the strength of the relationship, if any
- Visualizations with bar charts and stacked bar charts
- Statistical power calculation

## 🔧 Methodology Implemented
1. Data Preparation
Dataset loading and verification

Selection of relevant variables for compatibility analysis

Transformation of categorical variables

Categorical ordering for privacy_importance


Grouping of social_energy_rating into categories: "Unsocial", "Neutral", "Very Social"
## 📊 Results
Significant relationships were identified between the variables profession and room_type_preference.

## 📈 Key Findings
The analysis reveals compatibility patterns in:

profession and room_type_preference.

work_shift and dietary_restrictions

bedtime and dietary_restrrictions

## 🛠️ Technologies

- Python
- Pandas
- Scipy
- Matplotlib

##  Statistical Analysis 

# Chi-square

###  Calculation of correlations between categorical variables
```
chi2, p_value, dof, expected = chi2_contingency(tabla_contingencia)
```
Purpose: Determine whether there is a statistically significant relationship between pairs of categorical variables.

Interpretation:

p-value < 0.05: Significant relationship

p-value ≥ 0.05: No evidence of a relationship

# Cramér's V
Cramér's V is a measure of association between two categorical variables ranging from 0 to 1, where:

0 = No association between the variables

1 = Perfect association between the variables

```
v_cramer = np.sqrt(chi2 / (n * (min(tabla_contongencia.shape) - 1)))
```

Interpretation

0.00 - 0.10:    Null or very weak association 

0.10 - 0.20:    Weak association 

0.20 - 0.30:    Moderate association 

0.30 - 0.40:    Relatively strong association 

0.40 - 0.50:    Strong association 

0.50 - 1.00:    Very strong to perfect association 

## 📊 Statistical Power

The statistical power calculation complements the Chi-square analysis, determining the probability of detecting real effects in the population, considering:

Sample size (n=750)

Significance level (α=0.05)

Observed effect size


This approach ensures that the identified correlations are both statistically significant and practically relevant for decision-making on roommate compatibility.

---

> **Authors**

> 1. Aldrin Chávez
> 2. Kevin Sánchez
> 3. Daniela Analuisa
> 4. Ray Moya
