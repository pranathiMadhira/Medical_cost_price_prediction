# Medical_cost_price_prediction
Analyzed medical insurance data to predict healthcare costs based on factors such as age, BMI, smoking status, and number of children. Performed data cleaning, exploratory data analysis, feature encoding, and built a regression model. Evaluated performance using MAE, RMSE, and R² metrics.

## Problem Statement
Healthcare expenses differ significantly among individuals due to factors like lifestyle habits and demographic characteristics. The goal of this project is to analyze these factors and develop a predictive model that estimates medical insurance charges based on the available data.

## Dataset
The dataset used in this project contains demographic and health-related information for individuals.

### Main features in the dataset include:
- Age – Age of the individual
- Sex – Gender of the individual
- BMI – Body Mass Index
- Children – Number of children covered by insurance
- Smoker – Smoking status
- Region – Residential region
- Charges – Medical insurance cost (target variable)

## Project Workflow
1. Data Loading - The dataset was loaded using Pandas and inspected to understand its structure.
2. Data Cleaning - Checked for missing values, removed duplicate records, verified data types
3. Exploratory Data Analysis (EDA) - Data visualization was performed to identify patterns and relationships between variables. Key visualizations included: Age distribution, BMI distribution, Smoking status vs medical charges, Correlation heatmap
4. Feature Engineering - Categorical variables such as sex, smoker, and region were converted into numerical form using one-hot encoding.
5. Train-Test Split - The dataset was divided into training and testing sets to evaluate the model on unseen data.
6. Feature Scaling - StandardScaler was applied to normalize numerical features.
7. Model Training - A Linear Regression model was trained to predict medical charges.
8. Model Evaluation - The model performance was evaluated using the following metrics: R-squared: 0.8672, Mean Absolute Error (MAE): 0.21, Root Mean Squared Error (RMSE): 0.38

## Key Insights
- Smoking status significantly increases medical insurance costs.
- Individuals with higher BMI and older age tend to have higher healthcare expenses.
- Lifestyle factors play a major role in determining insurance charges.

## Summary
This project demonstrates how machine learning can be used to predict medical insurance costs based on demographic and lifestyle attributes. The analysis shows that smoking status, BMI, and age significantly influence healthcare expenses.

## Project Structure
```
Medical_cost_price_prediction/
├── data/
│   └── insurance.csv
├── notebooks/
│   └── medical_cost_prediction.ipynb
├── models/
│   └── medical_cost_model.pkl
├── images/
│   └── plots.png
├── requirements.txt
└── README.md
```