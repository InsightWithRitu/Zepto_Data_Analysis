# 🛒 Zepto  Data Analysis  
**Operational Efficiency & Pricing Strategy using PostgreSQL & Tableau**

## 📌 Project Overview
This project analyzes **Zepto grocery inventory data** to uncover insights around **pricing strategy, discount effectiveness, stock health, and revenue potential**.  
The analysis is designed to support **data-driven decision making** in inventory optimization, logistics planning, and margin improvement.

The entire analysis was performed using **PostgreSQL for querying** and **Tableau for visualization**, simulating a real-world business analytics workflow.

---

## 🎯 Business Objectives
- Identify **high-value and high-risk inventory**
- Analyze **discount strategies across categories**
- Detect **revenue leakage due to stock-outs**
- Evaluate **logistics efficiency using weight vs revenue**
- Support strategic decisions with **actionable insights**

---

## 🧰 Tech Stack
- **Database:** PostgreSQL  
- **Visualization:** Tableau  
- **Data Handling:** SQL (CTEs, Aggregations, Filtering)  
- **Metrics:** Revenue Potential, Discount %, Stock Status, Price per Unit  

---

## 📂 Dataset Preparation & Cleaning
To ensure reliable insights, the dataset was rigorously cleaned and validated:

- 🔍 **Null Value Checks**  
  Verified missing values in critical columns (Product Name, MRP, Discount %, Stock Status)

- ❌ **Invalid Record Removal**  
  Removed rows where:
  - MRP = 0  
  - Discounted Selling Price = 0  

- 🔄 **Unit Standardization**  
  Converted prices from **Paise to Rupees** for business readability

- 🧾 **Duplicate SKU Analysis**  
  Identified multiple entries of the same product to understand SKU depth

---

## 📊 Key Business Insights

### 1️⃣ Pricing & Discount Strategy

**🔹 Best Value Products**
- Identified **Top 10 products with highest discount %**
- These act as **loss leaders** to attract customer traffic

**🔹 Category-Level Discount Trends**
- Calculated **average discount per category**
- Highlighted categories heavily dependent on discounts vs stable pricing

**🔹 Premium Low-Discount Products**
- Products with:
  - MRP > ₹500  
  - Discount < 10%
- Indicates **price-inelastic, high-margin products**

---

### 2️⃣ Revenue & Inventory Potential

**💰 Revenue Projection by Category**
- Formula used:  
  `SUM(Selling Price × Available Quantity)`
- Revealed **₹224.31M+ worth of potential revenue** in inventory

**⚖️ Inventory Weight Analysis**
- Aggregated total weight per category
- Crucial for **logistics & delivery cost optimization**

---

### 3️⃣ Stock Health & Operational Efficiency

**📦 Stock Availability Analysis**
- Compared **In-Stock vs Out-of-Stock items**
- Highlighted lost revenue opportunities

**🚨 High-Value Stock-Out Alert**
- Identified products:
  - MRP > ₹300  
  - Currently out of stock
- These represent **direct revenue leakage**

---

### 4️⃣ Unit Economics

**⚖️ Price per Gram Analysis**
- Calculated cost per gram for products >100g
- Enables comparison between **value packs vs standard packs**

**📦 Pack Size Segmentation**
- Low (<1kg)  
- Medium (<5kg)  
- Bulk  
- Useful for **delivery planning & warehouse optimization**

---

## 📈 Interactive Dashboard (Tableau)
An interactive Tableau dashboard was built to convert SQL insights into real-time business intelligence.

### Dashboard Highlights
- **Total Revenue Potential:** ₹224.31M  
- **Weight vs Revenue Matrix:** Identifies logistics-heavy categories  
- **Discount Depth by Category**  
- **High-Value Stock-Out Alerts**

---

## 🧠 Strategic Recommendations

### 🔧 Inventory Optimization
- High-revenue categories also carry the **highest logistics weight**
- Supply chain optimization needed to reduce transportation cost

### 💸 Discount Strategy Improvement
- Fruits & Vegetables show **>15% average discount**
- Recommended **A/B testing reduced discounts** to improve margins

### 🚑 Revenue Leakage Control
- Immediate restocking of **Top 5 high-MRP out-of-stock SKUs**
- Prevents avoidable revenue loss

---

## 📌 Key Learnings
- Strong hands-on experience with **business-focused SQL analysis**
- Ability to translate **raw data into executive-level insights**
- Practical exposure to **inventory, pricing & operations analytics**

---

## 🚀 Future Scope
- Automate alerts for high-value stock-outs  
- Integrate demand forecasting models  
- Deploy dashboard for real-time monitoring  

---

## 👩‍💻 Author
**Ritu Saxena**  
Aspiring Data Analyst | SQL • Tableau • Business Analytics  

📫 *Open to Data Analyst & Business Analyst roles*
