☕ Cafe Sales Prediction using Logistic Regression
📌 Project Overview

This project focuses on building a Machine Learning model to predict the Payment Method used by customers based on cafe sales data.

The implementation includes:

Data preprocessing
Handling missing values
Encoding categorical data
Feature scaling
Model training using Logistic Regression
Performance evaluation
📂 Dataset

The dataset used is:

dirty_cafe_sales_cleaned.csv
Features:
Item
Quantity
Price Per Unit
Total Spent
Location
Target:
Payment Method
⚙️ Technologies Used
Python 🐍
Pandas
Scikit-learn
🚀 Steps Performed
1. Import Libraries

Essential libraries like Pandas and Scikit-learn are used.

2. Load Dataset

Dataset is loaded using pandas.read_csv().

3. Handle Missing Values

Missing values are filled using:

Mean (for numerical columns)
Mode (for categorical columns)
4. Drop Unnecessary Columns

Removed:

Transaction ID
Transaction Date
5. Encode Categorical Variables

Used Label Encoding for:

Item
Location
6. Feature Scaling

Applied StandardScaler to normalize data.

7. Train-Test Split
80% Training
20% Testing
8. Model Training

Used Logistic Regression with:

max_iter = 300
class_weight = 'balanced'
9. Prediction

Predicted payment method on test data.

10. Evaluation Metrics
Accuracy Score
Classification Report
Confusion Matrix
📊 Output Example
Accuracy Score
Precision, Recall, F1-score
Confusion Matrix
🧠 Key Learnings
Data preprocessing is crucial for model performance
Feature scaling improves Logistic Regression results
Handling class imbalance using class_weight='balanced'
Importance of evaluation metrics beyond accuracy
▶️ How to Run
Clone the repository:
git clone <your-repo-link>
Install dependencies:
pip install pandas scikit-learn
Run the notebook:
jupyter notebook EXP09.ipynb
📌 Future Improvements
Try advanced models (Random Forest, XGBoost)
Hyperparameter tuning
Deploy model using Flask / Streamlit
Add visualization dashboards
👨‍💻 Author

Aditya Patil