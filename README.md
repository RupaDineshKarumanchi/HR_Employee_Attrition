# Employee Attrition Analysis
This project analyzes employee attrition using an HR dataset to identify patterns, trends, and potential factors influencing employees leaving the organization. It covers data cleaning, preprocessing, feature engineering, and exploratory data analysis (EDA) to uncover insights that can help organizations improve employee retention.

# Dataset Overview
1. Rows: 1470
2. Columns: 35
3. Target Variable: Attrition (Yes = employee left, No = employee stayed)

#Key Features:
1. Demographics: Age, Gender, Marital Status, Education, EducationField
2. Job-related: JobRole, JobSatisfaction, YearsAtCompany, WorkLifeBalance, OverTime
3. Performance & Pay: MonthlyIncome, PercentSalaryHike, PerformanceRating
4. Other: DistanceFromHome, NumCompaniesWorked, TrainingTimesLastYear

# Project Workflow
1. Data Preprocessing
- Checked for null values → No missing data found.
- Checked for duplicates → None found.
- Verified data types and structure.

2. Outlier Detection & Removal
- Applied Interquartile Range (IQR) method to remove outliers from numeric features.
- Dataset reduced from 1470 to 699 records after outlier removal.

3. Categorical Encoding
- Applied Label Encoding to categorical features:
- Attrition, BusinessTravel, Department, EducationField, Gender, JobRole, MaritalStatus, Over18, OverTime.

4. Feature Engineering
Created a new feature: Age_at_joining = Age - YearsAtCompany (to estimate age when employee joined).

# Exploratory Data Analysis (EDA)
Attrition Distribution
1. Majority of employees stayed (Attrition = 0).
2. Fewer employees left (Attrition = 1).

# Key Observations
1. Age vs Attrition: Attrition exists across all age groups, but no strong age-based pattern.
2. Job Satisfaction vs Attrition: Even with low satisfaction, attrition is not always high.
3. Job Role vs Attrition: Certain roles have slightly closer attrition-to-retention ratios.
4. Marital Status vs Attrition: No significant difference across categories.
5. Correlation Heatmap: No strong correlation between Attrition and other features.

# Technologies Used
1. Python
2. Pandas – Data manipulation
3. NumPy – Numerical operations

# How to Run

1. Clone Repository
git clone https://github.com/your-username/attrition-analysis.git
cd attrition-analysis

2. Install Requirements
pip install -r requirements.txt

3. Run Scripts
python attrition_analysis.py  

Matplotlib & Seaborn – Data visualization

Scikit-learn – Label encoding
