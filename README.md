# TELCO-CHURN-VS-RETENTION-ANALYSIS-DASHBOARD
RIZE TECHNOLOGIES
📊 Telco Customer Churn Analysis – Power BI Dashboard
📌 Project Overview

Customer churn is one of the biggest challenges in the telecom industry. This project analyzes customer churn behavior using a real-world telecom dataset and presents actionable business insights through an interactive Power BI dashboard.The goal of this project is to identify churn drivers, measure revenue impact, and support data-driven retention strategies.

🏢 Business Problem
Telecom companies lose significant revenue when customers leave their services.
This project answers key business questions such as:
1.How many customers are churning?
2.Which customer segments are most likely to churn?
3.Which services and contract types drive churn?
4.How much revenue is lost due to churn?

📂 Dataset Information
Dataset Name: Telco Customer Churn
Source: Kaggle
Records: 7,032 customers
Columns: 21 features

Key Attributes
Customer demographics (gender, senior citizen, dependents)
Service usage (internet, phone, streaming, tech support)
Contract & payment details
Billing information (monthly & total charges)

🛠 Tools & Technologies
Power BI Desktop
Power Query (data transformation)
DAX (measure calculations)
Power BI Service (publishing)

🧱 Data Modeling Approach
To follow industry best practices, the dataset was split into two logical tables using Power Query:
1️⃣ Customer_Profile (Dimension Table)
Contains static customer attributes:
-customerID
-gender
-SeniorCitizen
-Partner
-Dependents

2️⃣ Customer_Services_Billing (Fact Table)
Contains service, billing, tenure, and churn information.

A one-to-many relationship was created using customerID.

📈 Key KPIs & Metrics

The dashboard focuses on industry-relevant churn metrics:

1️⃣ Total Customers

Total number of customers currently present in the dataset.

2️⃣ Churned Customers

Number of customers who have discontinued the service.

3️⃣ Active Customers

Number of customers who are still using the services.

4️⃣ Churn Rate (%)

Percentage of customers who have left the company.

5️⃣ Retention Rate (%)

Percentage of customers who continue using the services.

6️⃣ Average Monthly Charges

Average monthly amount billed to customers.

7️⃣ Average Customer Tenure

Average number of months customers stay with the company.

8️⃣ Active Monthly Revenue

Total monthly revenue generated from active customers.

9️⃣ Revenue Lost Due to Churn

Estimated monthly revenue lost from churned customers.

🔟 Churn Rate by Contract Type

Comparison of churn rates across different contract types (Month-to-Month, One Year, Two Year).

1️⃣1️⃣ Churn Rate by Internet Service

Analysis of churn behavior across internet service types (DSL, Fiber Optic, No Internet).

1️⃣2️⃣ Churn Rate by Payment Method

Comparison of churn rates across different payment methods.

1️⃣3️⃣ Churn Rate by Senior Citizen

Churn comparison between senior citizens and non-senior customers.

1️⃣4️⃣ Average Monthly Charges (Churned vs Active)

Comparison of billing amounts between churned and active customers.

1️⃣5️⃣ Average Tenure (Churned vs Active)

Comparison of customer tenure between churned and retained customers.

📊 Dashboard Highlights
KPI cards for quick business overview
Gauge visual for churn rate with an industry benchmark target
Churn breakdown by:
Contract Type
Internet Service
Payment Method
Senior Citizen
Revenue impact analysis
Interactive slicers for deeper insights

🔍 Key Insights
Month-to-month contracts show the highest churn rate
Customers with higher monthly charges are more likely to churn
Fiber optic internet users churn more than DSL users
Churn leads to significant monthly revenue loss

🎯 Business Impact

This dashboard enables stakeholders to:

Identify high-risk customer segments

Understand revenue loss drivers

Design targeted retention strategies

Support data-driven decision-making

🚀 How to Use This Project

Download the .pbix file

Open it in Power BI Desktop

Explore the dashboard using slicers and visuals

Review DAX measures for KPI logic

📸 Dashboard Preview

(Add screenshots of your dashboard here)

📌 Future Improvements

Add churn prediction using machine learning

Create customer lifetime value (CLV) metrics

Segment customers using tenure-based cohorts

Automate refresh with live data

🙋‍♂️ About Me

I am a data analytics enthusiast with strong interest in Power BI, business intelligence, and data-driven storytelling.
This project is part of my learning and portfolio development.

⭐ Feedback & Contributions

Feedback, suggestions, and improvements are always welcome!
If you find this project useful, feel free to ⭐ the repository.
