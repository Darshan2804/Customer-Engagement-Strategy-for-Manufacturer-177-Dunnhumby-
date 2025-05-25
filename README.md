# 🍼 Customer Engagement & Sales Strategy for Manufacturer 177  
**MGMT 687 – AI for Business Decisions | Purdue University**

This project leverages Dunnhumby’s “The Complete Journey” dataset to develop a customer engagement and sales strategy for **Manufacturer 177**, a market leader in the **Baby Foods** category. We explored segmentation, churn prediction, and campaign effectiveness to guide discount targeting, loyalty efforts, and sales forecasting.

---

## 🎯 Objective

To deliver a comprehensive AI-driven solution to:
- Identify and segment customers based on purchase behavior
- Predict churn and loyalty
- Optimize coupon and promotional strategies
- Forecast future sales using time series modeling

---

## 🧠 Why Baby Foods? Why Manufacturer 177?

- Baby Foods is **non-seasonal**, consistently in demand, and not subject to obsolescence  
- Manufacturer 177 leads the category with **72.3% market share**, but is facing **competitive pressure** from Brands 1282 and 131  
- Baby Foods is the **‘Star Product’** in the portfolio (high-growth and high-volume)

---

## 🔍 Business Questions Addressed

1. Who are our most **loyal** customers?
2. Which customer segments are most **responsive to coupons**?
3. Which **promotional methods** (e.g., display types, mailers) drive the most sales?
4. Who is at **risk of churn**, and how can we retain them?
5. What are the **expected sales trends** under current marketing strategies?

---

## 🛠 Methodology & Tools

| Task | Technique | Tools |
|------|-----------|-------|
| **Segmentation** | K-Means clustering (via Yellowbrick) | Python, Scikit-learn  
| **Coupon Sensitivity** | Linear regression with cluster × coupon interaction terms | Statsmodels  
| **Loyalty Analysis** | Linear regression with cluster × manufacturer interaction | Python  
| **Churn Prediction** | Random Forest Classifier | Scikit-learn  
| **Sales Forecasting** | ARIMA with causal factors | Statsmodels  

---

## 📈 Data Overview

**Source**: Dunnhumby Complete Journey Dataset  
**Scope**:  
- 2,500+ households  
- 100+ weeks of transaction data  
- Household-level demographics, campaign exposure, coupon redemptions, store displays, and mailers

**Key Tables**:  
- `transaction_data` – purchase behavior  
- `hh_demographic` – household segmentation  
- `coupon_redempt`, `coupon`, `campaign_table`, `campaign_desc` – campaign history  
- `product`, `causal_data` – product and display insights

---

## 🔑 Key Findings & Insights

### 🎯 Segmentation
- **K-Means clustering** identified **4 actionable segments**
- **Clusters 2 & 3**: Most **responsive to coupons** (ideal for acquisition campaigns)
- **Cluster 1**: Most **loyal to Manufacturer 177** (best for retention)

### 💸 Promotion & Placement Impact
- **Mailer Type A** and **Rear End Cap displays (Type 5)** generated the highest incremental sales  
  - Mailer A: $436.51 vs. Mailer 0 (no mailer): $84.92  
  - Rear End Cap: $35.16, 2nd best display performance

### 🚨 Churn Prediction
- Defined churn as **no transactions in the last 12 weeks**
- Built a **Random Forest Classifier** using features like Recency, Frequency, and Campaign Engagement
- Key churn drivers:
  - **Low recency**
  - Exposure to **Type B campaigns** (not well-optimized)

### 🔮 Sales Forecasting
- Used **ARIMA** for time series modeling with causal variables
- Forecasted baseline sales trajectory without future promo lift
- Helps inform budgeting and campaign planning

---

## 📊 Recommendations

- **Target Clusters 2 & 3** with aggressive **coupon campaigns**—these groups currently favor competitors but are price responsive  
- Focus **retention efforts** (catalogs, loyalty perks) on **Cluster 1**, which shows strong brand loyalty  
- Avoid overexposing Cluster 1 to discounts—preserve value perception  
- Optimize marketing spend around **Mailer A + Rear End Cap** pairings  
- For customers flagged as high churn risk, test **personalized reactivation offers**

---

## 👥 Team Members

- **Darshan Upadhyay**  
- Jayesh Chaudhari  
- Soutik Banerjee  

---

## 📌 Summary

This project demonstrates the power of AI and data science in solving real-world retail challenges—showcasing a full-stack solution from clustering and prediction to marketing recommendations. The integration of promotional effectiveness, customer loyalty, and predictive analytics led to actionable strategies that can directly impact Manufacturer 177’s sales and engagement performance.

> ✉️ Contact: **upadhy33@purdue.edu** for questions or collaboration.
