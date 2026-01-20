💳 Credit Card Fraud Risk Analysis Dashboard

Power BI | DAX | Risk Analytics | Business Intelligence | Fintech

📌 Project Overview

This project delivers an interactive fraud risk intelligence dashboard built using Power BI to help banks and fintech companies monitor fraud exposure, detect high-risk transactions, and reduce financial losses.
The dashboard transforms raw transaction data into executive-level KPIs and operational insights, enabling Fraud Analysts, Risk Teams, and Business Stakeholders to make data-driven decisions in real time.

🎯 Business Objective

To design a centralized fraud monitoring system that:
Identifies high-risk fraud types, regions, and merchant categories
Tracks monthly fraud trends and emerging risk patterns
Measures financial impact caused by fraudulent transactions
Improves response time for critical risk cases

🛠 Tools & Technologies

Power BI – Dashboard design & visualization
DAX – KPI and fraud metric calculations
Power Query – Data cleaning and transformation
CSV Dataset – Transaction-level fraud data
GitHub – Version control and documentation

📊 Executive KPIs
Metric	Description	Business Value
Fraud Rate (%)	Percentage of total transactions flagged as fraud	Measures detection system effectiveness
Fraudulent Transactions	Count of flagged fraud cases	Estimates investigation workload
Critical Risk Transactions	High-priority fraud alerts	Supports faster escalation
Fraud Loss Amount (₹)	Total monetary value of fraudulent transactions	Tracks financial exposure

📈 Dashboard Features

🎛 Interactive Filters

Fraud Type
State
Merchant Name

📊 Visual Insights

Fraud by Type & Transaction Category (Stacked Bar Chart)
Transactions by Risk Level (Donut Chart)
Fraud by State (Column Chart)
Monthly Fraud Trend (Line Chart)
KPI Cards (Fraud Rate, Fraud Count, Critical Risk, Fraud Amount)

🧠 Sample DAX Measures

Fraudulent Transactions =
CALCULATE(
    COUNTROWS('Credit Card Fraud Risk Analysis'),
    'Credit Card Fraud Risk Analysis'[Is_Fraud] = 1
)


Fraud Rate % =
DIVIDE(
    [Fraudulent Transactions],
    COUNTROWS('Credit Card Fraud Risk Analysis'),
    0
) * 100


Total Fraud Loss =
CALCULATE(
    SUM('Credit Card Fraud Risk Analysis'[Transaction_Amount]),
    'Credit Card Fraud Risk Analysis'[Is_Fraud] = 1
)


💼 Business Impact

This solution helps organizations:
📉 Reduce financial loss due to fraud
⚡ Improve response time for high-risk transactions
🧭 Identify high-risk states and vulnerable merchant categories
📊 Support risk strategy, compliance, and policy decisions

🤝 Strengthen customer trust and transaction security
