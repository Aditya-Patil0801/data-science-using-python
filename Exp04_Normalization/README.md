# 📊 Exp04 – Normalization & Standardization  
### DSPL (Data Science Programming Lab)

---

## 🎯 Aim
To apply **Normalization** and **Standardization** techniques on a dataset.

---

## 📂 Dataset Used
**dirty_cafe_sales.csv**

The dataset contains 10,000 records with the following columns:

- Transaction ID  
- Item  
- Quantity  
- Price Per Unit  
- Total Spent  
- Payment Method  
- Location  
- Transaction Date  

---

## 🧹 Data Preprocessing

Before applying scaling techniques, the following steps were performed:

1. Loaded dataset using `pandas`.
2. Identified numerical columns:
   - Quantity
   - Price Per Unit
   - Total Spent
3. Converted columns to numeric using:

```python
pd.to_numeric(errors='coerce')

4. Replaced invalid values (e.g., "ERROR") with NaN.

5. Handled missing values using mean imputation.

🔢 Techniques Applied:-
 1️⃣ Min-Max Normalization

 Rescales data between 0 and 1.

 Formula:

  X' = (X - Xmin) / (Xmax - Xmin)

 Implemented using:
  from sklearn.preprocessing import MinMaxScaler

2️⃣ Standardization (Z-Score Scaling)

 Transforms data such that:
  Mean = 0
  Standard Deviation = 1
 
 Formula:
  Z = (X - μ) / σ
 
 Implemented using:
  from sklearn.preprocessing import StandardScaler


🛠 Libraries Used
  pandas
  scikit-learn

📊 Results

 ✔ Successfully applied Min-Max Normalization
 ✔ Successfully applied Standardization
 ✔ Verified Mean ≈ 0 and Standard Deviation ≈ 1 after scaling

📌 Conclusion

In this experiment, feature scaling techniques were successfully applied to numerical data.

Normalization ensures values are scaled within a fixed range (0–1), while Standardization transforms data to have zero mean and unit variance. These techniques improve machine learning model performance and ensure fair feature contribution.

👨‍💻 Author

Aditya Patil.
