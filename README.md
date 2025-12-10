# 🧠 Customer Behavior Analysis  
### **Python • MySQL • Power BI**  

This project delivers an end-to-end customer behavior analytics pipeline.  
The workflow begins with **Python-based exploratory analysis**, then moves into **SQL-driven business queries**, and concludes with an **interactive Power BI dashboard**.  
The goal is to uncover insights into customer spending patterns, product preferences, discount behavior, and demographic influences.

---

## 🖼 Final Dashboard  
<img width="1486" height="810" alt="Final DashBoard" src="https://github.com/user-attachments/assets/40e7703c-e147-4afc-80eb-c2f4ae0846b1" />


---

## 📌 Project Overview

This analysis examines how customers shop across demographics, product categories, subscription status, shipping behaviors, and discount usage.  
The project workflow is intentionally simple, reproducible, and business-focused.

### What this project accomplishes:
- Identifies purchase trends and revenue drivers  
- Evaluates discount effectiveness  
- Segments customers using behavioral logic  
- Finds top-performing products and categories  
- Compares demographic groups (age, gender, subscription, etc.)  
- Generates a clean visual story through Power BI  

---

## 🧱 Architecture

The workflow follows a straight-line, minimal-friction design inspired by the structure of your reference repository.

           ┌──────────────────────┐
           │      Raw Dataset      │
           └───────────┬──────────┘
                       │
                       ▼
           ┌──────────────────────┐
           │   Python (EDA)       │
           │ - Load data          │
           │ - Explore patterns   │
           │ - Clean basic fields │
           └───────────┬──────────┘
                       │
                       ▼
           ┌──────────────────────┐
           │     MySQL Queries     │
           │ - Business insights   │
           │ - Aggregations        │
           │ - Trend evaluation    │
           └───────────┬──────────┘
                       │
                       ▼
           ┌──────────────────────┐
           │    Power BI Report    │
           │ - Visual analytics    │
           │ - Filters & segments  │
           │ - Storytelling layer  │
           └──────────────────────┘

---

## 📂 Project Structure

Customer-Behavior-Analysis/
│
├── notebooks/
│ └── Customer_Shopping_Behavior_Analysis.ipynb # Python EDA
│
├── sql/
│ └── customer_behavior_sql_query.sql # All business queries
│
├── powerbi/
│ └── customer_behavior_dashboard.pbix # Power BI file
│
├── images/
│ └── dashboard.png # (Add your dashboard export)
│
└── README.md


---

# 🔍 Step-by-Step Workflow

## 1️⃣ Python: Exploratory Data Analysis

The analysis starts in the Jupyter notebook:

- Load the dataset  
- Check missing values, distributions, and column types  
- Conduct univariate and multivariate analysis  
- Examine purchase behavior, ratings, and demographic patterns  
- Identify early hypotheses for SQL validation  

Run the notebook:

```bash
jupyter notebook notebooks/Customer_Shopping_Behavior_Analysis.ipynb
```

## 2️⃣ MySQL: Business Analysis Queries

The SQL layer validates insights discovered in Python and computes business-critical metrics.

Examples of questions answered via SQL:

- Revenue contribution by gender

- Impact of discount usage

- Top-rated and top-purchased products

- Subscription vs. non-subscription spending

- Category-wise performance

- Age group revenue distribution

- Customer segmentation using previous purchases


## 3️⃣ Power BI: Interactive Dashboard

Power BI brings the insights to life using:

- Dynamic segmentation

- Revenue and frequency charts

- Customer segment KPIs

- Product performance visuals

- Category and discount insights

- Smart slicers for demographics & behaviors


---

## 📈 Key Insights Uncovered

- Based on Python EDA + SQL queries:

- Gender differences in total revenue

- Products with the highest rating vs. highest purchase volume

- Age groups that contribute most revenue

- Discount usage behaviors and purchase lift

- Whether subscription users spend more

- Category-wise top 3 items

- New vs. returning vs. loyal customer segmentation

These insights form the backbone of the Power BI story.

---

## 🗃 Dependencies
- Python

- pandas

- numpy

- matplotlib / seaborn

- jupyter

- mysql-connector-python

- Install using:
```bash
pip install -r requirements.txt
```

---

🚀 Future Improvements

- Machine learning segmentation (K-means, DBSCAN)

- Forecasting purchase amounts

- Anomaly detection for unusual transactions

- Automated SQL → Power BI refresh pipeline

- Web or API interface for insights

