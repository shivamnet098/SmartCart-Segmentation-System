# 🛒 SmartCart Customer Segmentation System

## 📌 Overview

The **SmartCart Customer Segmentation System** is an Unsupervised Machine Learning project that groups customers into meaningful segments based on their behavior, spending patterns, and demographics.

🎯 Goal:
To help businesses understand different types of customers and design **targeted marketing strategies**.

---

## 📂 Dataset Information

* 📊 Total Records: **2240 customers**
* 📌 Features: **22 original features → 18 processed features**

### Key Attributes:

* Customer demographics (Age, Education, Marital Status)
* Income & spending habits
* Purchase behavior (web, store, catalog)
* Campaign response & complaints

---

## ⚙️ Tech Stack

* **Python**
* **Pandas, NumPy**
* **Matplotlib, Seaborn**
* **Scikit-learn**
* **KMeans, Agglomerative Clustering**
* **PCA (Dimensionality Reduction)**

---

## 🔧 Data Preprocessing

### ✔️ Handling Missing Values

* Filled `Income` missing values using **median**

### ✔️ Feature Engineering

Created powerful new features:

* `Age` → current age of customer
* `Customer_Tenure_Days` → loyalty duration
* `Total_Spending` → overall purchase value
* `Total_Children` → family size

### ✔️ Data Cleaning

* Removed unnecessary columns:

  * ID, Date, Birth Year, raw spending columns
* Handled categorical consistency:

  * Education grouped into levels
  * Marital status → `Living_With` (Alone / Partner)

---

## 📊 Exploratory Data Analysis (EDA)

* Pairplots to understand relationships
* Heatmap for correlation analysis
* Outlier detection & removal:

  * Age < 90
  * Income < 600,000

---

## 🔄 Data Transformation

### ✔️ Encoding

* One-Hot Encoding for:

  * Education
  * Living_With

### ✔️ Scaling

* StandardScaler used for normalization

---

## 📉 Dimensionality Reduction

Applied **PCA (Principal Component Analysis)**:

* Reduced data to **3 dimensions**
* Explained variance:

  * PC1 → 23.16%
  * PC2 → 11.38%
  * PC3 → 10.40%

---

## 📌 Finding Optimal Clusters

### 🔹 Elbow Method

* Optimal K = **4**

### 🔹 Silhouette Score

* Validated clustering quality

---

## 🧠 Clustering Models Used

### 1️⃣ K-Means Clustering

* Partition-based clustering
* Used for initial segmentation

### 2️⃣ Agglomerative Clustering

* Hierarchical clustering
* Final clustering applied

---

## 📊 Customer Segments (Insights)

### 🔴 Cluster 0: Low Spenders (Family Group)

* Lower income & spending
* More children
* Prefer store purchases

---

### 🔵 Cluster 1: High-Value Customers

* High income & high spending
* Frequent buyers
* Strong campaign response

---

### 🟡 Cluster 2: Budget-Conscious Individuals

* Low income & low spending
* Mostly living alone
* Less engagement

---

### 🟢 Cluster 3: Premium Independent Customers

* High income
* High spending
* Mostly single
* Highest response rate

---

## 📈 Visualizations

* 3D PCA cluster visualization
* Income vs Spending scatter plot
* Cluster distribution charts

---

## 🏆 Key Outcomes

✔️ Identified **4 distinct customer segments**
✔️ Enabled targeted marketing strategies
✔️ Improved understanding of customer behavior

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/shivamnet098/SmartCart-eCommerce.git

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn kneed

# Run the notebook
```

---

## 🎯 Future Improvements

* Apply advanced clustering (DBSCAN, GMM)
* Build recommendation system
* Deploy dashboard using Streamlit
* Real-time customer segmentation

---

## 👨‍💻 Author

**Shivam Kumar**
B.Tech CSE (AI & DS)
LNCT Bhopal

---

## ⭐ Project Highlights

* End-to-end ML pipeline
* Real-world business use case
* Strong feature engineering
* Data-driven insights

---
