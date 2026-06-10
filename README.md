# Customer-Segmentation-Kmeans-Clustering
Customer Segmentation using K-Means Clustering, Silhouette Analysis, Feature Scaling, and Customer Profiling to identify meaningful customer groups for targeted marketing and business insights.
# 🛍️ Customer Segmentation Using K-Means Clustering

A Machine Learning project that segments mall customers into distinct groups using K-Means Clustering. The project analyzes customer demographics and spending behavior to identify meaningful customer segments that can help businesses improve marketing strategies, customer targeting, and decision-making.

---

## 📌 Project Overview

Customer segmentation is a crucial business strategy that helps organizations understand different types of customers based on their purchasing behavior and demographics.

In this project, K-Means Clustering is used to group customers based on:

- Annual Income
- Spending Score
- Age
- Gender

The project also evaluates clustering performance using the Silhouette Score and generates cluster profiles for business insights.

---

## 🎯 Objectives

- Identify customer groups with similar behavior.
- Analyze spending patterns across customer segments.
- Evaluate cluster quality using the Elbow Method and Silhouette Score.
- Generate customer profiles for business intelligence.
- Export segmented customer data for Power BI and Tableau dashboards.

---

## 📂 Dataset

Dataset: **Mall Customers Dataset**

Features:

| Feature | Description |
|----------|-------------|
| CustomerID | Unique Customer Identifier |
| Gender | Male / Female |
| Age | Customer Age |
| Annual Income (k$) | Annual Income in Thousand Dollars |
| Spending Score (1-100) | Customer Spending Score |

Dataset File:

```text
Mall_Customers.csv
```

---

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## ⚙️ Machine Learning Workflow

### 1. Data Collection

Load customer dataset using Pandas.

### 2. Data Exploration

- Dataset shape
- Data types
- Missing value analysis
- Basic statistics

### 3. Feature Selection

Initial clustering uses:

```text
Annual Income (k$)
Spending Score (1-100)
```

---

### 4. Finding Optimal Number of Clusters

The Elbow Method is used to determine the optimal value of K.

WCSS (Within Cluster Sum of Squares) is calculated for:

```text
K = 1 to K = 10
```

An elbow graph is plotted to identify the best number of clusters.

---

### 5. Customer Segmentation Using K-Means

K-Means clustering is applied with:

```python
n_clusters = 5
```

Each customer is assigned to a cluster based on purchasing behavior.

---

### 6. Cluster Visualization

Customer groups are visualized using scatter plots showing:

- Annual Income
- Spending Score
- Cluster Centroids

This helps understand how customers are distributed across segments.

---

### 7. Cluster Evaluation

Silhouette Score is used to evaluate cluster quality.

```python
from sklearn.metrics import silhouette_score
```

Higher values indicate better-defined clusters.

---

### 8. Customer Profile Analysis

Average values are calculated for each cluster:

- Age
- Annual Income
- Spending Score

Cluster sizes are also analyzed to understand customer distribution.

---

### 9. Advanced Segmentation

Additional features are included:

- Age
- Gender
- Annual Income
- Spending Score

Steps:

- Gender Encoding
- Feature Scaling using StandardScaler
- K-Means Clustering

This provides more detailed customer segmentation.

---

### 10. Export Segmented Dataset

Final segmented dataset is saved for visualization tools:

```text
Segmented_Mall_Customers.csv
```

Compatible with:

- Power BI
- Tableau
- Excel

---

## 📊 Results

The model successfully segments customers into 5 distinct groups based on spending behavior and income patterns.

Examples of identified customer segments:

- High Income - High Spending Customers
- High Income - Low Spending Customers
- Low Income - High Spending Customers
- Low Income - Low Spending Customers
- Average Customers

These insights can help businesses:

- Improve targeted marketing campaigns
- Increase customer retention
- Optimize promotional strategies
- Enhance customer experience

---

## 📁 Project Structure

```text
customer-segmentation-kmeans/
│
├── Mall_Customers.csv
├── Customer Segmentation using K-Means Clustering,silhouette_score and Standardscaler.ipynb
├── Segmented_Mall_Customers.csv
├── requirements.txt
├── README.md
```

---

## ▶️ Installation

### Clone Repository

```bash
git clone https://github.com/vatsaldhuvad23-droid/customer-segmentation-kmeans.git
```

### Navigate to Project Folder

```bash
cd customer-segmentation-kmeans
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Project

```bash
python customer_segmentation.py
```

---

## 📈 Visualizations

### Elbow Method

Used to determine the optimal number of clusters.

### Customer Segmentation Scatter Plot

Displays:

- Customer Groups
- Cluster Boundaries
- Cluster Centroids

### Cluster Profile Analysis

Provides average customer characteristics for each cluster.

---

## 📊 Sample Output

### Silhouette Score

```text
The average silhouette score is: 0.55
```

### Cluster Profiles

```text
Cluster_Group
Age
Annual Income
Spending Score
Cluster Size
```

Business insights can be generated from these profiles.

---

## 🚀 Future Enhancements

- Interactive Streamlit Dashboard
- Power BI Dashboard Integration
- Tableau Dashboard
- Customer Lifetime Value Analysis
- Hierarchical Clustering
- DBSCAN Clustering
- Real-Time Customer Segmentation

---

## 💼 Business Applications

- Customer Relationship Management (CRM)
- Personalized Marketing
- Customer Retention Strategy
- Market Basket Analysis
- Retail Analytics
- Sales Optimization

---

## 📚 Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Visualization
- Unsupervised Machine Learning
- K-Means Clustering
- Elbow Method
- Silhouette Analysis
- Feature Engineering
- Data Preprocessing
- Business Intelligence

---

## 👨‍💻 Author

**Vatsal Dhuvad**

GitHub: https://github.com/vatsal-dhuvad

---

## ⭐ If you found this project useful, consider giving it a star on GitHub.
