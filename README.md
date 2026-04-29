# CSE572-Group-20

# E-Commerce Customer Segmentation using Clustering

## 📌 Project Overview

This project focuses on customer segmentation for an e-commerce platform using data mining techniques. The goal is to group customers based on purchasing behavior and provide actionable business insights.

The project uses the **Online Retail II dataset** and applies clustering algorithms such as **K-Means, Hierarchical Clustering, and DBSCAN**.

---

## 🎯 Objectives

- Segment customers based on behavior
- Extend traditional RFM features with behavioral attributes
- Compare multiple clustering models
- Evaluate performance using different metrics
- Identify meaningful business segments

---

## 📊 Dataset

- Dataset: **Online Retail II**
- ~500,000 transaction records
- Features include:
  - Customer ID
  - Invoice details
  - Quantity, Price
  - Transaction date

Each transaction is converted into **customer-level features**.

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Removed missing Customer IDs
- Removed cancelled invoices
- Removed invalid transactions
- Created TotalAmount feature

---

### 2. Feature Engineering

#### RFM Features:
- Recency
- Frequency
- Monetary

#### Additional Features:
- AvgOrderValue
- AvgQtyPerInvoice
- UniqueProducts
- PurchaseSpan
- PurchaseRate
- ActivityScore

---

### 3. Clustering Models

We implemented and compared:

- **K-Means (RFM baseline)**
- **K-Means (extended features)**
- **Hierarchical Clustering**
- **DBSCAN**

---

### 4. Evaluation Metrics

- Silhouette Score (higher is better)
- Davies-Bouldin Index (lower is better)
- Calinski-Harabasz Score (higher is better)

---

## 📈 Results

| Model | Feature Set | Performance |
|------|------------|------------|
| KMeans | RFM | Strong baseline |
| KMeans | Extended | Lower performance |
| Hierarchical | Extended | Weakest |
| DBSCAN | Extended | Best cluster separation |

👉 **DBSCAN achieved the highest silhouette score**

---

## 👥 Final Customer Segments

- **Champions** → high-value, loyal customers  
- **At Risk** → inactive customers  
- **Outliers** → irregular or unusual behavior  

---

## 💡 Business Insights

- Champions → retain with loyalty programs  
- At Risk → re-engagement campaigns  
- Outliers → further analysis required  

---

## ⚠️ Limitations

- DBSCAN outliers are not always low-value customers  
- Different metrics suggest different best models  
- Results depend on parameter tuning  

---

## 🚀 Future Work

- Improve feature engineering  
- Tune clustering parameters  
- Explore hybrid clustering approaches  
- Add predictive models  

---

## 📂 Project Structure

📁 project/
│
├── 📁 data/
│ └── online_retail_II.xlsx
│
├── 📁 notebooks/
│ └── E_Commerce_Customer_Segmentation_Final.ipynb
│
├── 📁 outputs/
│ ├── model_comparison.csv
│ ├── cluster_profile.csv
│ └── final_customers.csv
│
├── 📁 report/
│ └── Final_ACM_Report.docx
│
└── README.md


---

## 🧪 How to Run

1. Install dependencies:
pip install pandas numpy matplotlib seaborn scikit-learn

2. Run the notebook:
jupyter notebook

3. Open and run:
E_Commerce_Customer_Segmentation_Final.ipynb

---

## 📄 Report

The final report is provided in ACM format:

📄 `Final_Report.docx`

---

## 👨‍💻 Team

- **Nafeez Ahamed Mohamed**  
  Masters in Software Engineering  

- **Pavithran Boopathi**  
  Masters in Data Science, Analytics and Engineering (Computing and Decision Analytics)

- **Adisree Rajasekar**  
  Masters in Data Science, Analytics and Engineering (Computing and Decision Analytics)

- **Mohamed Javed Khan Akbar Ali**  
  Masters in Data Science, Analytics and Engineering (Computing and Decision Analytics)

---

## 📚 References

- Online Retail II Dataset  
- Scikit-learn Documentation  
