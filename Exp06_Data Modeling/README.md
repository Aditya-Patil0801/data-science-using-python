# Data Modelling using Dataset Partition (Experiment 06)

## 📌 Overview

This experiment demonstrates the process of **data modelling using dataset partitioning**. The objective is to train and evaluate different machine learning classification algorithms using cross-validation and a train-test split.

The experiment uses a **dirty dataset of cafe sales**, which requires preprocessing before applying machine learning models.

---

## 📂 Dataset

**Dataset Name:** `dirty_cafe_sales.csv`

The dataset contains information about cafe transactions such as:

* Transaction ID
* Item
* Quantity
* Price Per Unit
* Total Spent
* Payment Method
* Location
* Transaction Date

Since the dataset contains **dirty values such as `UNKNOWN` and `ERROR`**, data cleaning is performed before modelling.

---

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the dataset using **Pandas**
2. Replaced dirty values (`UNKNOWN`, `ERROR`) with `NaN`
3. Converted numeric columns to appropriate data types
4. Removed missing values
5. Selected relevant features for modelling
6. Encoded categorical variables using **LabelEncoder**

---

## 📊 Features and Target Variable

**Input Features (X):**

* Quantity
* Price Per Unit

**Target Variable (y):**

* Payment Method

The goal is to **predict the payment method used for a transaction**.

---

## 🤖 Machine Learning Models Used

The following classification algorithms were used:

* Support Vector Machine (SVM)
* Decision Tree Classifier
* Logistic Regression
* Random Forest Classifier
* K-Nearest Neighbors (KNN)

---

## 🔍 Model Evaluation

### 1️⃣ Cross Validation

Each model was evaluated using **5-fold cross validation**.

```python
cross_val_score(model, X, y, cv=5)
```

### 2️⃣ Train-Test Split

The dataset was split into:

* **80% Training Data**
* **20% Testing Data**

```python
train_test_split(X, y, test_size=0.2)
```

### 3️⃣ Confusion Matrix

Used to evaluate classification performance.

```python
confusion_matrix(y_test, y_pred)
```

### 4️⃣ Accuracy Score

Measures how accurately the model predicts the target variable.

```python
accuracy_score(y_test, y_pred)
```

---

## 📈 Result

Among all models, **Random Forest Classifier** produced the best performance for the given dataset.

The model was trained using the training data and evaluated on the testing dataset.

---

## 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Jupyter Notebook / VS Code

---

## 🎯 Conclusion

This experiment demonstrates how machine learning models can be applied to a real-world dataset after proper preprocessing. The dataset was cleaned, partitioned into training and testing sets, and multiple classification algorithms were evaluated using cross validation and accuracy metrics.

---

## 👨‍💻 Author

Aditya Patil
