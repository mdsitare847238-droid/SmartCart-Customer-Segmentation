# SmartCart Customer Segmentation

## Project Overview

SmartCart Customer Segmentation is a machine learning project that uses customer data to identify different groups of customers based on their purchasing behaviour and characteristics.

The dataset contains 2,240 customer records. The project performs data preprocessing, feature engineering, outlier handling, encoding, scaling, PCA, and customer clustering.

## Dataset

The dataset contains customer information such as:

- Education
- Income
- Recency
- Deal Purchases
- Web Purchases
- Catalog Purchases
- Store Purchases
- Web Visits per Month
- Complaints
- Response

Additional features are created during preprocessing, including:

- Age
- Customer Tenure
- Total Spending
- Total Children
- Living With

## Data Preprocessing

The following steps are performed in the project:

1. Missing values are handled.
2. New features are created from the existing data.
3. Unnecessary columns are removed.
4. Outliers are analysed and handled.
5. Categorical variables are encoded.
6. Numerical features are scaled.
7. PCA is applied for dimensionality reduction.

## PCA

Principal Component Analysis (PCA) is used to reduce the dimensionality of the processed dataset.

The project uses PCA components to visualise the customer data, including a 3D projection using PCA1, PCA2, and PCA3.

## K-Means Clustering

K-Means clustering is used to divide customers into different groups.

The Elbow Method and WCSS are used to determine the optimal number of clusters.

The optimal value obtained in the project is:

**Best K = 4**

Therefore, the customers are segmented into 4 clusters.

## Cluster Analysis

The resulting clusters are analysed to understand the differences between customer groups.

The analysis helps identify patterns in:

- Customer spending
- Income
- Purchase behaviour
- Customer engagement
- Other customer characteristics

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- K-Means
- PCA
- StandardScaler
- One-Hot Encoding
- KneeLocator

## Project Structure
```text
SmartCart-Customer-Segmentation/
│
├── smartcart.ipynb
└── README.md


