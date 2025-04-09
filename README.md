# Insurance Expense Prediction Project

## Overview
This project uses **Alteryx** to build a linear regression model that estimates insurance expenses based on personal and health-related attributes. The goal is to help insurance companies predict the premium to be charged to their customers.

## Project Structure
![image](https://github.com/user-attachments/assets/ccb0541d-de90-4526-8aba-b2e4f6a5af00)


## Description

### Dataset Used
- **insurance_data.csv**: Contains the following columns:
  - `age`: Age of the individual
  - `sex`: Gender
  - `bmi`: Body Mass Index
  - `children`: Number of children
  - `smoker`: Smoking status
  - `region`: Geographical region
  - `expenses`: Medical expenses incurred

### Workflow Process
- Imported the dataset using the **Input Data** tool.
- Added a **Field Summary** tool to understand the distribution of each variable.
- Used a **Unique Tool** to identify and separate duplicate rows from unique entries.
- Visualized relationships using **Scatter Plot** to explore variation in `expenses` with respect to `age` and `bmi`.
- Used the **Correlation Tool** to quantify relationships between variables.
- Split the data using the **Create Samples Tool** (Estimation - 80%, Validation - 20%).
- Applied **Linear Regression Tool** with `expenses` as the target variable.
- Scored the validation dataset using the **Score Tool**.
- Visualized the actual vs. predicted expenses using another **Scatter Plot Tool**.

## Results
After executing the workflow:
- A linear regression model is created to predict insurance costs.
- Model scoring provides a comparison between **actual vs. estimated expenses**.
- Insights derived can assist insurers in setting fair and accurate premium rates for customers.
