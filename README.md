# SmartCart-Customer-Segmentation
# 🛒 SmartCart Clustering System

## 📌 Problem Statement

SmartCart is a growing e-commerce platform serving customers across multiple countries. The company has collected customer data containing **2,240 customer records and 22 attributes**, including customer demographics, purchase behaviour, website activity, and customer response.

Currently, SmartCart uses generic marketing and engagement strategies for all customers without clearly understanding different customer behaviour patterns.

This can result in inefficient marketing, missed opportunities to retain high-value customers, and delayed identification of churn-prone users.

To solve this problem, SmartCart aims to build an **intelligent customer segmentation system using unsupervised machine learning**.

The system analyses customers based on:

- Purchasing behaviour
- Engagement levels
- Loyalty indicators

The objective is to group customers into meaningful clusters and discover hidden patterns in customer behaviour.

---

## 🎯 Project Objective

The main objective of this project is to develop a **customer segmentation system using clustering algorithms**.

The system identifies different customer groups based on their behaviour and characteristics.

---

## 📊 Dataset

The dataset contains **2,240 customer records and 22 attributes**.

The dataset includes:

### Customer Demographics
- ID
- Year of Birth
- Education
- Marital Status
- Income
- Kidhome
- Teenhome
- Customer Joining Date

### Purchase Behaviour
- Wine spending
- Fruit spending
- Meat product spending
- Fish product spending
- Sweet product spending
- Gold product spending

### Purchase Frequency
- Deal purchases
- Web purchases
- Catalog purchases
- Store purchases
- Website visits per month

### Customer Feedback
- Recency
- Complaints
- Response

---

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

1. Missing values in the `Income` column were handled using the median.
2. New features were created:
   - Age
   - Customer Tenure
   - Total Spending
   - Total Children
3. Education categories were grouped into:
   - Undergraduate
   - Graduate
   - Postgraduate
4. Marital status was transformed into a `Living_With` feature.
5. Unnecessary columns were removed.
6. Outliers were analysed and handled.
7. Categorical features were encoded.
8. Numerical features were scaled for clustering.

---

## 🔧 Feature Engineering

The following new features were created:

- **Age** – calculated from `Year_Birth`
- **Customer_Tenure_Days** – calculated from customer joining date
- **Total_Spending** – total amount spent across product categories
- **Total_Children** – total number of children and teenagers
- **Living_With** – simplified marital-status category

---

## 📉 Dimensionality Reduction

**Principal Component Analysis (PCA)** was applied to the processed customer data.

Three principal components were used to visualise the customer data in a 3D space:

- PCA1
- PCA2
- PCA3

---

## 🤖 K-Means Clustering

The project uses **K-Means clustering** for customer segmentation.

The Elbow Method and WCSS were used to analyse the suitable number of clusters.

The optimal number of clusters obtained was:

**Best K = 4**

Therefore, customers were divided into **4 different clusters**.

---

## 📊 Cluster Analysis

After applying K-Means clustering, the customer groups can be analysed based on their characteristics and purchasing behaviour.

The clustering results help identify different patterns among SmartCart customers.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- K-Means Clustering
- PCA
- StandardScaler
- One-Hot Encoding
- KneeLocator

---

## 📁 Project Structure

```text
SmartCart-Customer-Segmentation/
│
├── smartcart.ipynb
├── smartcart_customers.csv
└── README.md

##  Conclusion

The SmartCart Customer Segmentation project uses K-Means clustering to identify different customer groups based on their characteristics and purchasing behaviour.

After data preprocessing, feature engineering, and PCA, the Elbow Method was used to determine the optimal number of clusters. The optimal value obtained was **K = 4**.

This segmentation helps in understanding customer behaviour and can support better customer targeting and marketing decisions.
