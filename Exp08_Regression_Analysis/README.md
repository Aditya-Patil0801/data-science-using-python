📊 Regression Analysis on Cafe Sales Dataset
📌 Overview

This project demonstrates a machine learning-based regression/classification analysis using a cleaned cafe sales dataset. The goal is to analyze customer purchase behavior and predict the Location based on transaction features like quantity, price, and total spending.

🎯 Objective

To preprocess and clean real-world data

To apply machine learning techniques

To build a predictive model using Logistic Regression

To evaluate model performance using accuracy and confusion matrix

🗂️ Dataset

File Used: dirty_cafe_sales_cleaned.csv

The dataset contains:

Quantity

Price Per Unit

Total Spent

Location (Target Variable)

⚙️ Technologies Used

Python 🐍

Pandas

Scikit-learn

🔄 Steps Performed
1. Data Loading

Dataset loaded using Pandas

2. Data Cleaning

Removed missing values

Trimmed column names

Converted numeric columns to proper format

3. Feature Selection

Input Features (X):

Quantity

Price Per Unit

Total Spent

Target Variable (y):

Location

4. Data Encoding

Converted categorical target variable using LabelEncoder

5. Train-Test Split

Split data into:

80% Training

20% Testing

6. Model Building

Applied Logistic Regression model

7. Prediction

Predicted values using test dataset

8. Evaluation

Accuracy Score

Confusion Matrix

📈 Results

Model performance is evaluated using:

Accuracy Score

Confusion Matrix

(Actual values will depend on dataset at runtime)

📌 Key Learnings

Importance of data cleaning in ML

Handling categorical variables

Implementing Logistic Regression

Evaluating model performance

🚀 How to Run

Install required libraries:

pip install pandas scikit-learn

Run the notebook:

jupyter notebook

Ensure dataset path is correct:

df = pd.read_csv("your_dataset_path.csv")
⚠️ Note

Logistic Regression is used here for classification (predicting location), not continuous regression.

Make sure dataset is cleaned before training the model.

👨‍💻 Author

Aditya Patil