****A MACHINE LEARNING APPROACH TO IDENTIFY MATERNAL RISK PATTERNS FOR LOW BIRTH WEIGHT
**
This project applies statistical analysis and machine learning models to predict the likelihood of low birth weight in newborns using maternal and clinical factors.
The dataset includes 1,000+ birth records with features such as gestational weeks, maternal weight gain, prenatal visits, birth term, marital status, smoking status, and race.

Key Steps in the Project
****Data Preprocessing:
**
- Removed irrelevant or high-missing-value columns (e.g., father’s age).
- Imputed missing values using median/mode strategies.
- Performed encoding of categorical variables and normalization of continuous features.

****Exploratory Data Analysis (EDA):
**
- Visualized distributions, relationships, and correlations using histograms, scatter plots, and heatmaps.
- Identified key predictors such as gestational weeks and birth term.

****Statistical Testing:
**
- Conducted t-tests, Chi-square tests, and ANOVA to evaluate significant relationships between features and target variable.

**Feature Selection:
- Applied Chi-Square, Recursive Feature Elimination (RFE), and Extra Trees Classifier to identify the most influential variables.

**Model Development & Evaluation:
- Built and compared Logistic Regression, Random Forest, Support Vector Machine (SVM), and XGBoost classifiers.
- Evaluated models using accuracy, precision, recall, F1-score, and AUC-ROC.
- Random Forest emerged as the best-balanced model for precision and recall.

**Results:
- Achieved up to 94% accuracy across models.
- Random Forest provided the best trade-off between sensitivity and specificity for identifying low birth weight cases.
