# Loan Approval Prediction

This project focuses on analyzing loan data to predict the approval status of loan applications. 
Using a combination of data preprocessing, exploratory data analysis (EDA), and machine learning models, 
the project evaluates which factors most influence loan approval and selects the best predictive model.


## Project Overview

The goal is to preprocess and analyze a dataset of loan applications, visualize key patterns, and build predictive models to determine loan approval status. 
Models are evaluated based on their accuracy to identify the most effective approach.


## Steps in the Project

### Data Cleaning
   
Addressed missing values in columns such as Gender, Married, and Dependents using the mode.

Filled missing values in LoanAmount and Loan_Amount_Term with mean and mode respectively.

Removed inconsistencies and ensured the dataset was complete for analysis.

### Feature Engineering
   
Created new features:

LoanAmount_log: Log-transformed values of LoanAmount to normalize skewed data.

TotalIncome and TotalIncome_log: Aggregated applicant and co-applicant incomes to evaluate combined financial capability.


### Exploratory Data Analysis (EDA)
   
Visualized distributions of numerical columns (ApplicantIncome, LoanAmount, etc.).

Compared loan approval rates across categorical variables like Gender, Education, and Property_Area.


### Model Training
   
Applied multiple classification algorithms:

Logistic Regression

Support Vector Machine (SVM)

Random Forest

Decision Tree

Evaluated model performance using accuracy on the test dataset.


## Key Findings

Best Model: Logistic Regression achieved the highest accuracy of 80%, outperforming other models like SVM (68%) and Random Forest (32%).

Feature Importance: Variables such as Credit_History, ApplicantIncome, and LoanAmount significantly impacted loan approval predictions.


## Approval Trends:

Urban applicants had higher approval rates than rural ones.

Graduate applicants were more likely to be approved.


## Libraries Used

Pandas, NumPy: Data preprocessing and manipulation.

Seaborn, Matplotlib: Data visualization.

Scikit-Learn: Model training and evaluation.


## Next Steps

Experiment with additional advanced models like XGBoost.

Optimize hyperparameters for better accuracy.

Deploy the final model as a web application for loan approval predictions.
