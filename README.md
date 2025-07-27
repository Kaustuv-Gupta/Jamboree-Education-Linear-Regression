# Jamboree-Education-Linear-Regression

## Project Context
Jamboree has helped thousands of students achieve top scores in exams like GMAT, GRE, and SAT through unique problem-solving methods. Recently, Jamboree launched a feature on their website that estimates the probability of a student getting into an Ivy League college, specifically from an Indian perspective. This project aims to analyze the factors influencing graduate admissions and predict the chances of admission based on various variables.

## Objective
The goal is to help Jamboree understand which factors are most important in graduate admissions, how these factors interrelate, and to build a predictive model for admission chances.


## Dataset
**File:** `Jamboree_Admission.csv`

**Columns:**
- Serial No. (Unique row ID)
- GRE Scores (out of 340)
- TOEFL Scores (out of 120)
- University Rating (out of 5)
- Statement of Purpose and Letter of Recommendation Strength (out of 5)
- Undergraduate GPA (out of 10)
- Research Experience (0 or 1)
- Chance of Admit (ranging from 0 to 1)

---

## Project Workflow Summary

This project follows a comprehensive data science workflow to analyze and predict graduate admission chances using the Jamboree dataset. The main steps are:

1. **Exploratory Data Analysis (EDA):**
   - Examined data shape, types, and performed univariate and bivariate analysis.
   - Visualized distributions and relationships between features and the target variable.
   - Key insight: CGPA, GRE, and TOEFL scores are most strongly correlated with admission chances.

2. **Data Preprocessing:**
   - Checked for duplicates and missing values (none found).
   - Outlier analysis showed no significant outliers.
   - Feature engineering: Dropped irrelevant columns and prepared data for modeling.

3. **Model Building:**
   - Built and compared Linear Regression, Ridge, and Lasso models.
   - Displayed and interpreted model coefficients.
   - Found that CGPA, GRE, and TOEFL are the most influential predictors.

4. **Assumption Testing:**
   - Checked for multicollinearity (VIF), linearity, homoscedasticity, and normality of residuals.
   - Removed features with high VIF and confirmed model assumptions were met.

5. **Model Evaluation:**
   - Evaluated models using MAE, RMSE, R², and Adjusted R² on both train and test sets.
   - All models performed well, with no overfitting and strong generalization.

6. **Insights & Recommendations:**
   - CGPA is the most important factor for admission prediction.
   - Additional features (demographics, university reputation, work experience) could further improve the model.
   - The model can be integrated into real-world admission systems for efficient, data-driven decision-making.

---

This summary reflects the step-by-step approach and key findings as implemented in the Jupyter notebook `Business_Case_Jamboree_Education_Linear_Regression.ipynb`.

