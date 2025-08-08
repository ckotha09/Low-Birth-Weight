## Low Birth Weight Prediction Using Machine Learning in Python

## Objective
To predict the likelihood of low birth weight in newborns using maternal, clinical, and sociodemographic factors through statistical analysis, feature selection, and multiple machine learning models.

--- 

## Source: 
Public birth records, NC births dataset - https://www.openintro.org/data

---
## Size & Features:
~1,000+ records with variables such as gestational weeks, maternal weight gain, prenatal visits, birth term, marital status, smoking status, race, and maternal age.

---
## Target Variable: 
Baby weight category (Normal vs. Low Birth Weight)

---
## Preparation: 
Cleaned dataset by removing irrelevant columns (e.g., father’s age), imputing missing values with median/mode, and encoding categorical variables.

----
## Methods Used
## 1. Data Preprocessing:
- Removed high-missing-value/uninformative columns.
- Imputed missing data using median for continuous and mode for categorical features.
- Encoded categorical variables into binary (0/1) format.
- Normalized continuous variables for algorithms like SVM.

## 2. Exploratory Data Analysis (EDA):
- Histograms, scatter plots, and correlation heatmaps to identify trends.
- Count plots to analyze distribution across categories.

---- 
## 3. Statistical Analysis:
- T-tests, Chi-square tests, and ANOVA to identify significant relationships between predictors and baby weight category.

-----
## Feature Selection:
- Chi-Square (SelectKBest) for univariate importance.
- Recursive Feature Elimination (RFE) with Logistic Regression.
- Extra Trees Classifier for ensemble-based ranking.

-----
## Modeling:
- Logistic Regression – Baseline model for interpretability.
- Random Forest – For capturing non-linear patterns and interactions.
- Support Vector Machine (SVM) – For optimal class separation in high-dimensional space.
- XGBoost – Gradient boosting for enhanced accuracy.

----
## Model Evaluation:
- Accuracy, Precision, Recall, F1-Score, AUC-ROC.
- 5-fold cross-validation for performance stability.

---
## Observations
- Gestational Weeks and Birth Term (Premie) emerged as the most consistent predictors across feature selection methods.
- Logistic Regression provided good interpretability but lower recall for low birth weight cases.
- Random Forest achieved the most balanced performance between precision and recall.
- SVM and XGBoost also performed well but had slightly lower recall compared to Random Forest.

----
## Key Insights
- Prenatal care factors (gestational weeks, prenatal visits) strongly influence birth weight outcomes.
- Sociodemographic factors like smoking and marital status, though statistically weaker, hold public health relevance.
- Addressing class imbalance (low birth weight as minority) can further improve recall in future models.
- Best Model: Random Forest – balanced precision/recall with high overall accuracy.
