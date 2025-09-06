# Credit_card_financial_dashboard
## Comprehensive credit card weekly dashboard that provides real-time insights

## 1. Problem Statement

Financial institutions often struggle to monitor credit card performance due to the sheer volume of customer and transaction data. Without a centralized system, it becomes difficult to track **revenue streams, customer segments, delinquency rates, and regional performance** on a weekly basis.

The goal of this project was to **design and implement a Credit Card Financial Dashboard** that provides real-time insights into customer behavior, revenue trends, and operational KPIs. This enables management to make data-driven decisions and improve overall business performance.

## **2. Methodology**

### **a. Data Collection**

- **Source:** Transaction and customer data (CSV files provided).
- **Storage:** Imported into **PostgreSQL/MySQL** database for structured storage.
- **Tables Created:**- `customer` → customer demographics, age, income, location
- `credit_card` → credit card transactions, fees, interest
### **b. Data Processing**

- **SQL Queries** used to clean, join, and prepare datasets.
- Data transformations included:
    - Handling missing values.
    - Converting dates into week numbers for time-series analysis.
    - Creating revenue measures:Revenue=Annual Fees+Transaction Amount+Interest Earned
### **c. Data Modeling in Power BI**

- **Relationship Model:**
    - `customer (Customer_ID)` ↔ `credit_card (Customer_ID)`
- **DAX Measures:**
    - Age Groups: segmented into 20–30, 30–40, 40–50, 50–60, 60+.
    - Income Groups: Low (<35K), Medium (35K–70K), High (>70K).
    - Revenue (weekly, current vs previous week).
    - KPIs: Customer Count, Activation Rate, Delinquency Rate.
### **. Dashboard Design**

The Power BI dashboard was designed with interactivity and storytelling in mind:

- **KPIs Cards:** Revenue, Transactions, Customers, Delinquency Rate.
- **Trend Analysis:** Revenue comparison (current vs previous week).
- **Customer Segmentation:** Age group, income group, gender contribution.
- **Product Analysis:** Revenue share by card type (Silver, Blue, Gold, Platinum).
- **Geographic Analysis:** Regional contribution by state (TX, NY, CA).
- **Year-to-Date (YTD) Overview:** Cumulative revenue, transactions, interest earned.
## **3. Key Insights (Sample – Week 53, 31st Dec)**
<img width="2048" height="1184" alt="image" src="https://github.com/user-attachments/assets/eb5620c6-1620-43e2-9a8f-5277202f4cde" />
<img width="2048" height="1184" alt="image" src="https://github.com/user-attachments/assets/51ef59a1-3e77-42b3-8bcc-eb74027bc223" />



- **Revenue:** Increased by **28.8% week-over-week (WoW)**.
- **YTD Performance:**
    - Total Revenue: **$55M**
    - Transaction Volume: **$45M**
    - Interest Earned: **$8M**
- **Customer Segmentation:**
    - Male customers contributed **$31M**, females **$26M**.
    - Majority of revenue came from **age group 30–40**.
- **Product Analysis:**
    - **Blue & Silver cards = 93%** of overall transactions.
- **Geography:**
    - Top 3 states (TX, NY, CA) contributed **68%** of revenue.
- **Operational Metrics:**
    - **Activation Rate:** 57.5%
    - **Delinquency Rate:** 6.06%
## **4. Tools & Technologies**

- **Database:** PostgreSQL / MySQL
- **Data Processing:** SQL, DAX in Power BI
- **Visualization:** Microsoft Power BI
- **Version Control:** GitHub

## **5. Conclusion**

The **Credit Card Financial Dashboard** successfully transformed raw transactional data into meaningful business insights. Stakeholders can now:

- Track revenue growth and customer acquisition on a weekly basis.
- Identify high-value customer segments.
- Monitor delinquency rates to mitigate risk.
- Make data-driven product and marketing decisions.
  
