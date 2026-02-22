# TELCO-CHURN-VS-RETENTION-ANALYSIS-DASHBOARD
📊 Telco Customer Churn Analysis – Power BI Dashboard
📌 Project Overview

Customer churn is one of the biggest challenges in the telecom industry. This project analyzes customer churn behavior using a real-world telecom dataset and presents actionable business insights through an interactive Power BI dashboard.

The goal of this project is to identify churn drivers, measure revenue impact, and support data-driven retention strategies.

🏢 Business Problem

Telecom companies lose significant revenue when customers leave their services.
This project answers key business questions such as:

How many customers are churning?

Which customer segments are most likely to churn?

Which services and contract types drive churn?

How much revenue is lost due to churn?

📂 Dataset Information

Dataset Name: Telco Customer Churn

Source: Kaggle

Records: 7,032 customers

Columns: 21 features

Target Variable: Churn (Yes / No)

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

customerID

gender

SeniorCitizen

Partner

Dependents

2️⃣ Customer_Services_Billing (Fact Table)

Contains service, billing, tenure, and churn information.

A one-to-many relationship was created using customerID.

📈 Key KPIs & Metrics

The dashboard focuses on industry-relevant churn metrics:

Total Customers

Churned Customers

Active Customers

Churn Rate (%)

Retention Rate (%)

Average Monthly Charges

Average Tenure

Active Monthly Revenue

Revenue Lost Due to Churn

These KPIs help quantify churn behavior and financial impact.

🧮 Sample DAX Measures
Churn Rate (%)
Churn Rate % =
DIVIDE(
    [Churned Customers],
    [Total Customers],
    0
)
Revenue Lost Due to Churn
Revenue Lost to Churn =
CALCULATE(
    SUM(Customer_Services_Billing[MonthlyCharges]),
    Customer_Services_Billing[Churn] = "Yes"
)
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
