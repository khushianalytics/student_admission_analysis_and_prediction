# Student Admission Analysis and Prediction using Linear Regression

Google Colab Notebook:
https://colab.research.google.com/drive/1pRMlhuMQmZYKaLU5CVTT0XluHG7Bi0TK#scrollTo=lhjyhtCDdttJ


## Project Overview
- This project analyzes historical student admission data to identify the factors that influence admission probability and builds a **Linear Regression** model to predict a student's chance of admission based on their academic and profile-related attributes.
- The project follows a complete machine learning workflow, including data understanding, data cleaning, exploratory data analysis (EDA), preprocessing, model building, evaluation, and business recommendations.

## Business Objective
The objective of this project is to:
- Analyze the key factors affecting student admission chances.
- Identify relationships between academic profiles and admission probability.
- Build a regression model capable of predicting admission chances for new student profiles.
- Generate actionable insights to support data-driven decision making.

## Business Questions
This project aims to answer the following questions:
- Which factors influence admission chances?
- Does CGPA have a stronger impact than GRE Score?
- Does research experience improve admission probability?
- Which academic and profile-related features contribute positively to admission chances?

## Dataset Information
- **Dataset:** Graduate Admission Dataset (Jamboree Admission Prediction)
- **Records:** 500 Students
- **Features:** 7 Input Features + 1 Target Variable

## Features
- GRE Score
- TOEFL Score
- University Rating
- SOP
- LOR
- CGPA
- Research

## Target Variable
- Chance of Admit

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook


## Project Workflow

### Business Understanding
- Defined business objective
- Identified key business questions

### Dataset Understanding
- Loaded dataset
- Checked dataset shape
- Reviewed data types
- Generated descriptive statistics
- Understood feature information

### Data Cleaning
- Checked missing values
- Checked duplicate records
- Validated data types
- Verified data ranges
- Removed the non-predictive **Serial No.** column
- Detected potential outliers using boxplots
- Retained valid observations without outlier removal

### Data Preprocessing
- Separated features and target variable
- Performed an 80-20 Train-Test Split
- Skipped feature scaling because Linear Regression does not require scaling for prediction, while documenting this design decision.

### Linear Regression Model
- Built the Linear Regression model
- Trained the model
- Generated predictions on the test dataset

### Model Evaluation

The model was evaluated using:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

### Model Performance

| Metric | Value |
|---------|--------|
| MAE | 0.0427 |
| MSE | 0.0037 |
| RMSE | 0.0609 |
| R² Score | 0.8188 |


## Key Findings
- CGPA has a strong positive relationship with admission probability.
- Research experience positively contributes to admission chances.
- LOR also has a positive association with admission probability.
- GRE Score, TOEFL Score, University Rating, and SOP contribute positively to the prediction.
- The model explains approximately **81.88%** of the variation in admission probability.



## Business Recommendations
- Students should prioritize maintaining a strong CGPA to improve admission prospects.
- Participating in research projects can strengthen an applicant's profile.
- High-quality Letters of Recommendation can positively influence admission chances.
- Universities and admission consultants can leverage predictive models to provide personalized guidance to applicants.


## Future Improvements
- Experiment with Ridge and Lasso Regression.
- Perform Hyperparameter Tuning.
- Compare Linear Regression with Decision Tree and Random Forest models.
- Deploy the model using Streamlit or Flask for real-time predictions.
