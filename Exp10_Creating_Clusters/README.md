
☕ Cafe Sales Clustering using K-Means
📌 Project Overview

This project demonstrates the use of K-Means Clustering, an unsupervised machine learning algorithm, to group cafe sales data into meaningful clusters.

The goal is to identify patterns in customer purchases based on features like spending, quantity, and location.

📂 Dataset

File Used:

dirty_cafe_sales_cleaned.csv
Features in Dataset:
Item
Quantity
Price Per Unit
Total Spent
Location
⚙️ Technologies Used
Python 🐍
Pandas
NumPy
Matplotlib
Scikit-learn
🚀 Steps Performed
1. Data Loading

Dataset is loaded using pandas.read_csv().

2. Data Preprocessing
Handled missing values:
Mean for numerical columns
Mode for categorical columns
Removed unnecessary columns:
Transaction ID
Transaction Date
3. Encoding
Converted categorical data (Item, Location) into numeric using Label Encoding
4. Feature Scaling
Applied StandardScaler to normalize features
5. Finding Optimal Clusters
Used Elbow Method to determine the best number of clusters (K)
6. Model Training
Applied K-Means Clustering
Used n_clusters = 3 (based on elbow method)
7. Visualization
Plotted clusters using Matplotlib
📊 Output
Clustered dataset with an additional Cluster column
Elbow graph for optimal K
Scatter plot visualization of clusters
🧠 Key Learnings
Understanding of unsupervised learning
Importance of feature scaling in distance-based algorithms
How to determine optimal clusters using the elbow method
Data preprocessing techniques
▶️ How to Run
Clone the repository:
git clone <your-repo-link>
Install dependencies:
pip install pandas numpy matplotlib scikit-learn
Run the notebook:
jupyter notebook EXP09.ipynb
📌 Future Improvements
Use advanced clustering techniques (DBSCAN, Hierarchical Clustering)
Visualize clusters using PCA
Build a dashboard using Streamlit
Analyze customer segments in depth
👨‍💻 Author

Aditya Patil