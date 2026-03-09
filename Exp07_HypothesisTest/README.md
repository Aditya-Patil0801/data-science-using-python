DSPL Experiment 07

Implementation of Statistical Hypothesis Test using SciPy and Scikit-learn
📌 Overview

This experiment demonstrates how to perform statistical hypothesis testing using SciPy and apply a machine learning model using Scikit-learn.

The dataset used is Dirty Cafe Sales Dataset, which contains sales transaction data. The experiment includes data cleaning, hypothesis testing, and regression modelling.

🎯 Aim

To implement a statistical hypothesis test using SciPy and build a simple machine learning regression model using Scikit-learn.

📂 Dataset

Dataset: dirty_cafe_sales.csv

Key attributes used in this experiment:

Column	Description
Quantity	Number of items purchased
Total Spent	Total amount spent in transaction

The dataset contains dirty values (e.g., "ERROR"), which require cleaning before analysis.

⚙️ Technologies Used

Python
SciPy
Scikit-learn
Pandas
Jupyter Notebook

🧪 Experiment Steps
1️⃣ Data Loading

Load the dataset using Pandas.

2️⃣ Data Cleaning

Convert columns to numeric values and remove invalid entries.

3️⃣ Hypothesis Testing

Perform a Two-Sample T-Test using SciPy to compare training and testing samples.

Decision Rule:

If p-value < 0.05 → Reject Null Hypothesis
If p-value ≥ 0.05 → Fail to Reject Null Hypothesis
4️⃣ Machine Learning Model

Use Linear Regression to model the relationship between:

Quantity → Total Spent
5️⃣ Model Evaluation

Evaluate the model using Mean Squared Error (MSE).

📊 Example Output
T Statistic: 0.20135398323712655
P Value: 0.8404314257219311
Fail to Reject Null Hypothesis

Model MSE: 18.611768431783844

📁 Project Structure
DSPL-Experiment-07
├── Exp07.ipynb
└── README.md
📌 Conclusion

The hypothesis test shows that there is no significant difference between the two samples, and the regression model successfully predicts Total Spent based on Quantity.

👨‍💻 Author

Aditya Patil