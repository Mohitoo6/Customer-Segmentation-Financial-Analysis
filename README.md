# 📊 Customer Segmentation & Risk Analysis

## 🚀 Project Overview

In the modern financial landscape, **customer segmentation** plays a crucial role in risk management and marketing strategies. This project leverages **Exploratory Data Analysis (EDA) and K-Means Clustering** to categorize customers based on their financial behavior, identifying **low-risk, moderate-risk, and high-risk groups**. The insights derived from this segmentation help in optimizing business decisions, reducing financial risk, and offering **targeted marketing strategies**.

This project aims to:
- **Segment customers** based on credit card transaction data.
- **Identify financially risky customers** using clustering techniques.
- **Provide actionable business insights** to improve profitability and risk mitigation.

---

## 📂 Dataset Overview

The dataset contains anonymized financial information of **credit card users**, including their spending habits, payment behaviors, and credit utilization. Key features include:

- **BALANCE** → Outstanding balance on the credit card.
- **PURCHASES** → Total purchase amount made by the customer.
- **CASH_ADVANCE** → Amount of cash advances taken.
- **PAYMENTS** → Total payments made by the customer.
- **CREDIT_LIMIT** → Maximum credit limit assigned to the customer.
- **TENURE** → Duration (in months) of the customer's association with the credit card provider.

---

## 📊 Exploratory Data Analysis (EDA)

Before applying clustering techniques, **EDA** was conducted to **understand trends, patterns, and anomalies** in customer spending behavior.

### **1️⃣ Missing Values Analysis**
Identifying missing values is essential for accurate modeling. The heatmap below highlights missing data points in the dataset:

![Missing Values Heatmap](https://github.com/Mohitoo6/Customer-Segmentation-Financial-Analysis/blob/main/missing_values_heatmap.png)

**Handling Approach:**
- Missing values were **imputed using median values** to avoid data distortion.

### **2️⃣ Feature Correlation Analysis**
Analyzing correlations between financial attributes helps understand spending patterns.

![Feature Correlation Heatmap](visualizations/correlation_heatmap.png)

**Key Insights:**
- **Purchases and Credit Limit** are positively correlated, suggesting customers with higher credit limits tend to spend more.
- **Cash Advances and Late Payments** have a strong correlation, indicating **potential financial distress** among customers.

### **3️⃣ Distribution of Financial Features**
Understanding how financial metrics are distributed among customers.

![Feature Distributions](visualizations/feature_distributions.png)

**Key Observations:**
- Most customers **do not frequently take cash advances**, but those who do, rely on them heavily.
- Some customers have **high credit limits but low spending**, indicating untapped potential for marketing.

---

## 🤖 Customer Segmentation Using K-Means Clustering

### **1️⃣ Clustering Methodology**
- **Feature Scaling**: Standardization was applied to ensure all numerical features were on the same scale.
- **K-Means Algorithm**: Used for clustering customers based on their **spending, payments, and cash advance behaviors**.
- **Elbow Method**: Determined the optimal number of clusters.

### **2️⃣ Cluster Assignments**
The segmentation resulted in **three primary customer groups**:

| Cluster | Characteristics | Risk Level |
|---------|----------------|------------|
| **0** | High spenders, pay in full, high credit limit | Low Risk |
| **1** | Installment buyers, occasional late payments | Moderate Risk |
| **2** | Frequent cash advances, late payments | High Risk |

**Cluster Distribution:**

![Cluster Distribution](visualizations/cluster_distribution.png)

---

## 📌 Business Impact & Recommendations

### **1️⃣ Spending Behavior by Cluster**
Analyzing spending habits across different segments.

![Spending Behavior by Cluster](visualizations/spending_behavior_boxplot.png)

**Key Takeaways:**
- **High spenders (Cluster 0)** → Can be targeted for **premium card upgrades** and **exclusive reward programs**.
- **Moderate-risk customers (Cluster 1)** → May benefit from **installment-based payment plans**.
- **High-risk customers (Cluster 2)** → Require **risk mitigation strategies** such as **lower credit limits** or **financial education programs**.

### **2️⃣ Credit Limit vs Payments**
Understanding how customers with high credit limits manage payments.

![Credit Limit vs Payments](visualizations/credit_limit_vs_payments.png)

**Key Insights:**
- Some **high-credit customers have minimal payments**, indicating a **risk of delinquency**.
- Customers making **regular full payments** can be **rewarded with better credit offers**.

### **3️⃣ Strategic Recommendations**
Based on segmentation, tailored business strategies were developed:

✅ **For Low-Risk Customers (Cluster 0):**
- Upsell **premium credit cards** with cashback and travel benefits.
- Offer **higher credit limits** to boost engagement.

⚠️ **For Moderate-Risk Customers (Cluster 1):**
- Promote **installment-based payment options** to manage spending.
- Educate them on **improving credit scores**.

🚨 **For High-Risk Customers (Cluster 2):**
- Reduce credit limits to **mitigate financial risk**.
- Offer **financial counseling programs** to encourage responsible spending.
- Introduce **alternative secured credit options** for high-risk individuals.

### **Expected Business Improvement**
- **15% increase** in customer spending from personalized promotions ([McKinsey Report](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights/the-value-of-getting-personalization-right-or-wrong-is-multiplying?utm_source=chatgpt.com)).
- **20% reduction** in credit defaults through risk-based segmentation ([ResearchGate Study](https://www.researchgate.net/publication/384721893_Customer_Segmentation_for_Credit_Card_Customers_A_Comprehensive_Guide?utm_source=chatgpt.com)).
- **Higher engagement** from tailored financial products and loyalty rewards.

---

## 🎯 Next Steps

- **Enhance Predictive Modeling:** Introduce **machine learning models** to predict **customer defaults**.
- **Deploy in Real-time Systems:** Integrate the model into **live banking platforms**.
- **Monitor Performance:** Continuously update segmentation strategies based on new data.

---

## 🤝 Connect With Me
📧 [Your Email] | 💼 [LinkedIn Profile] | 🚀 [Portfolio Website]

---

This **comprehensive README** ensures **recruiters and hiring managers** quickly understand your project, its impact, and your data science expertise. 🚀

