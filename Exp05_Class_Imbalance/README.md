# Exp 05 – Handling Class Imbalance Using SMOTE

## 📌 Objective
To handle class imbalance in the Student Depression Dataset using SMOTE (Synthetic Minority Over-sampling Technique) and evaluate model performance before and after balancing.

---

## 📂 Dataset
**File Used:** `cleaned_student_depression_dataset.csv`  

The dataset contains student-related attributes such as:

- Gender  
- Age  
- Academic Pressure  
- CGPA  
- Sleep Duration  
- Financial Stress  
- Family History of Mental Illness  
- Depression (Target Variable)

### 🎯 Target Variable:
`depression`
- 0 → Not Depressed  
- 1 → Depressed  

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)

---

## 🔍 Steps Performed

1️⃣ Data Loading
- Imported dataset using Pandas.
- Displayed dataset structure and information.

2️⃣ Data Preprocessing
- Checked for missing values.
- Checked for duplicate rows.
- Dropped unnecessary column (`id`).
- Encoded categorical variables using `LabelEncoder`.

3️⃣ Checking Class Imbalance
- Visualized class distribution using `countplot`.
- Observed imbalance in the `depression` column.

4️⃣ Train-Test Split
Dataset was split into:
- 80% Training Data
- 20% Testing Data

```python
train_test_split(X, y, test_size=0.2, random_state=42)
5️⃣ Model Before SMOTE

Applied Logistic Regression.

Evaluated using:

Accuracy

Classification Report

Confusion Matrix

6️⃣ Applying SMOTE

SMOTE was applied only to training data:

from imblearn.over_sampling import SMOTE

SMOTE generates synthetic samples of the minority class to balance the dataset.

7️⃣ Model After SMOTE

Re-trained Logistic Regression using balanced data.

Evaluated performance again.

📊 Results
✅ Before SMOTE:

Model showed bias toward majority class.

Lower recall for minority class.

✅ After SMOTE:

Balanced class distribution.

Improved recall and better overall classification performance.

Reduced bias toward majority class.

📈 Evaluation Metrics Used

Accuracy Score

Precision

Recall

F1-Score

Confusion Matrix

🧠 Key Concept – What is SMOTE?

SMOTE (Synthetic Minority Over-sampling Technique) is used to:

Handle imbalanced datasets

Generate synthetic data points for minority class

Improve classification performance

SMOTE is applied only on training data to avoid data leakage.

🎯 Conclusion

The dataset had class imbalance in the depression variable.

Applying SMOTE improved model fairness.

Logistic Regression performed better after balancing.

Handling class imbalance is essential for real-world ML problems.

🚀 How to Run

Install required library:

pip install imbalanced-learn

Run notebook cells in order.

👨‍💻 Author

Aditya Patil