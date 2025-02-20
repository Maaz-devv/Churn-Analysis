# 📊 Telco Churn Analysis 
## 📖 Table of Contents  

- [📌 Overview](#-overview)  
- [🗃️ Data Structure & Initial Deck](#data-structure--initial-deck)  
- [📈 Key Metrics](#-key-metrics)  
- [📊 Visual Insights](#-visual-insights)  
  - [1️⃣ Churn by Internet Service](#1️⃣-churn-by-internet-service)  
  - [2️⃣ Churn by Payment Method](#2️⃣-churn-by-payment-method)  
  - [3️⃣ Customers Churned by Tenure Month Range](#3️⃣-customers-churned-by-tenure-month-range)  
  - [4️⃣ CLTV of Churned Customers by Age](#4️⃣-cltv-of-churned-customers-by-age)  
  - [5️⃣ Top Churn Reasons](#5️⃣-top-churn-reasons)  
  - [6️⃣ Churned Customers by Age Range](#6️⃣-churned-customers-by-age-range)  
- [🔮 Predictive Enhancements](#-predictive-enhancements)  
- [📌 Recommendations](#-recommendations)  
- [📂 Deliverables](#-deliverables)  
- [🎯 Skills Developed](#-skills-developed)  
- [📌 Conclusion](#-conclusion)  



## 📌 Overview  
This Power BI dashboard analyzes customer churn for a telecommunications company. The goal is to uncover key trends, identify reasons behind churn, and provide actionable insights to help reduce churn rates and improve customer retention strategies.<br>
📊 An interactive PowerBI dashboard can be downloaded [here](https://github.com/Maaz-devv/Churn-Analysis/blob/main/Telecom%20Churn%20Analysis.pbix).<br>

---
## 🗃️ Data Structure & Initial Deck
- **Database Structure:** Consists of six tables:
  - **Core_transactions**
  - **Customer_details**
  - **Geographic_details**
  - **Services_details**
  - **Payment_details**
  - **Measure_Table**
- **Total Records:** 7,043 rows

### Entity-Relationship Diagram (ERD)
The ERD below provides an overview of the database structure and table relationships.
![churn data model](https://github.com/user-attachments/assets/4fd8d97e-cd3f-433a-8461-890bca9b6ca6)

---
## 📈 Key Metrics  
The top-level KPIs and visual insights include:  
- **Total Customers:** 7,043  
- **Churned Customers:** 1,869  
- **Churn Rate:** 26.5%  
- **Average Churn Score:** 58.70  

📌 These metrics highlight a significant **churn rate of 26.5%**, requiring focused interventions to address underlying issues.  
Below is the Overview page from the PowerBI dashboard

![Churn analysis Dashboard](https://github.com/user-attachments/assets/eeae2d8d-d24a-43f5-943f-bbc909078bd3)
---

## 📊 Visual Insights  

### **1️⃣ Churn by Internet Service**  
🔹 **Key Observations:**  
- **Fiber Optic** customers represent **69.4%** of churned customers.  
- **DSL** customers account for **24.56%**, while **No Service** remains negligible at **6.05%**.  

💡 **Insight:** High churn in Fiber Optic suggests potential dissatisfaction with service quality or competitive offerings.  

---

### **2️⃣ Churn by Payment Method**  
🔹 **Key Observations:**  
- **Electronic Check** customers show the highest churn rate (**1,000+ churned customers**).  
- **Mailed Check, Bank Transfer (Auto), and Credit Card (Auto)** methods have lower churn levels.  

💡 **Insight:** Customers using Electronic Checks may face payment challenges or prefer more modern payment methods.  

---

### **3️⃣ Customers Churned by Tenure Month Range**  
🔹 **Key Observations:**  
- Customers with a **tenure of 0–10 months churn the most**, followed by **11–20 months**.  
- Customers with **longer tenure (51–72 months)** have significantly lower churn rates.  

💡 **Insight:** New customers (0–20 months) are more likely to churn, indicating gaps in onboarding, service quality, or engagement.  

---

### **4️⃣ CLTV of Churned Customers by Age**  
🔹 **Key Observations:**  
- Customers aged **30–40 years** contribute the **highest Customer Lifetime Value (CLTV)** despite churning.  
- CLTV drops significantly for older customers (**above 50 years**).  

💡 **Insight:** **High-CLTV customers (30–40 years)** require special retention strategies due to their business value.  

---

### **5️⃣ Top Churn Reasons**  
🔹 **Key Observations:**  
Top reasons for churn:  
1. **Attitude of support person** (192 customers; **$795,465 CLTV**)  
2. **Competitor offered higher download speeds** (189 customers; **$787,135 CLTV**)  
3. **Competitor offered more data** (162 customers; **$682,978 CLTV**)  

💡 **Insight:** **Service-related issues (support, speed, data) drive churn**. Competitor offerings impact customer retention heavily.  

---

### **6️⃣ Churned Customers by Age Range**  
🔹 **Key Observations:**  
- Customers aged **20–40 years** experience the **highest churn**, aligning with CLTV trends.  

💡 **Insight:** Retention strategies should **target customers aged 20–40 years**, as they are more likely to churn and have high revenue potential.  

---

## 🔮 Predictive Enhancements  
In addition to visualizations:  
✅ Created a **ChurnScoreRange** measure using **DAX**:  
- Categorized churn scores into **Low, Medium, High, Very High**.  
- Identified **non-churn customers with high churn scores** as potential churn risks.  

💡 **Insight:** This measure predicts **at-risk customers before they churn**, allowing proactive engagement.  

---

## 📌 Recommendations  
✔ **Improve Fiber Optic Service**: Match competitor speeds & data plans.  
✔ **Engage Early-Tenure Customers**: Onboarding & personalized support for **0–20 month customers**.  
✔ **Modernize Payment Methods**: Encourage a shift from **Electronic Checks** to auto-payments.  
✔ **Retain High-CLTV Customers**: Loyalty programs for **30–40-year-olds**.  
✔ **Enhance Customer Support**: Address complaints & service-related churn.  

---

## 📂 Deliverables  
📊 **Power BI Dashboard**: Interactive visuals with filters for dynamic analysis.  
📈 **Churn Score Prediction**: Identifies at-risk customers for proactive intervention.  
📝 **Report**: Business insights & actionable recommendations for stakeholders.  

---

## 🎯 Skills Developed  
✅ **Data Cleaning & Preparation** (Power Query: handling missing data, removing duplicates, applying transformations)  
✅ **Data Wrangling & Transformation** (Merging queries, creating calculated columns, custom transformations in Power Query)  
✅ **Data Modeling** (Power BI: establishing relationships, optimizing data structure)  
✅ **DAX Calculations** (Creating measures like ChurnScoreRange, KPIs)  
✅ **Interactive Dashboards** (Power BI Visualizations, slicers, and drill-throughs)  
✅ **Business Insights & Storytelling** (Data-driven decision-making & strategy development)  
✅ **Predictive Analytics** (Identifying at-risk customers, segmentation analysis)  
  

---

## 📌 Conclusion  
The **Telco Churn Analysis** dashboard provides deep insights into customer churn patterns, key drivers, and **actionable strategies** to reduce churn. By leveraging **ChurnScoreRange** and predictive analytics, businesses can **proactively engage at-risk customers and improve retention efforts**. 🚀  

---

  
