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

The dashboard focuses on industry-important churn metrics. Below are the main KPIs along with 
their DAX formulas and explanations. 
Total Customers 
Total Customers = 
DISTINCTCOUNT(Customer_Services_Billing[customerID]) 
Description: 
Shows the total customer base of the company. 
Churned Customers 
Churned Customers = 
CALCULATE( 
DISTINCTCOUNT(Customer_Services_Billing[customerID]), 
Customer_Services_Billing[Churn] = "Yes" 
) 
Description: 
Counts how many customers have left the company. 
Active Customers 
Active Customers = 
CALCULATE( 
DISTINCTCOUNT(Customer_Services_Billing[customerID]), 
Customer_Services_Billing[Churn] = "No" 
) 
Description: 
Shows customers currently using services. 
Churn Rate (%) 
Churn Rate % = 
DIVIDE( 
[Churned Customers], 
[Total Customers], 
0 
) 
Description: 
The most critical KPI — indicates the percentage of customers who churned. 
Retention Rate (%) 
Retention Rate % = 
DIVIDE( 
[Active Customers], 
[Total Customers], 
0 
) 
Description: 
Shows how successful the company is at retaining customers. 
Average Monthly Charges 
Avg Monthly Charges = 
AVERAGE(Customer_Services_Billing[MonthlyCharges]) 
Description: 
Represents the typical monthly bill paid by customers. 
Average Tenure 
Avg Tenure = 
AVERAGE(Customer_Services_Billing[tenure]) 
Description: 
Shows how long customers stay with the company on average. 
Revenue Lost Due to Churn 
Revenue Lost to Churn = 
CALCULATE( 
SUM(Customer_Services_Billing[MonthlyCharges]), 
Customer_Services_Billing[Churn] = "Yes" 
) 
Description: 
Estimates the monthly revenue impact caused by churned customers. 
Active Monthly Revenue 
Active Monthly Revenue = 
CALCULATE( 
SUM(Customer_Services_Billing[MonthlyCharges]), 
Customer_Services_Billing[Churn] = "No" 
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
