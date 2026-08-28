# 🛍️ Customer Shopping Behavior Analysis – Retail Customer Insights

_Analyzing customer shopping behavior, spending patterns, and subscription dynamics to support data-driven retail and marketing decisions using SQL, Python, and Power BI._

---

## 📌 Table of Contents
- <a href="#overview">Overview</a>
- <a href="#business-problem">Business Problem</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools--technologies">Tools & Technologies</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#data-cleaning--preparation">Data Cleaning & Preparation</a>
- <a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a>
- <a href="#research-questions--key-findings">Research Questions & Key Findings</a>
- <a href="#dashboard">Dashboard</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#final-recommendations">Final Recommendations</a>
- <a href="#author--contact">Author & Contact</a>

---
<h2><a class="anchor" id="overview"></a>Overview</h2>

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across various product categories. The goal is to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior to guide strategic business decisions. A complete pipeline was built using Python for data cleaning and feature engineering, PostgreSQL for structured business-question analysis, and Power BI for visualization and reporting.

---
<h2><a class="anchor" id="business-problem"></a>Business Problem</h2>

Understanding customer shopping behavior is critical for improving retail strategy and customer retention. This project aims to:
- Compare revenue contribution across gender, age group, and subscription status
- Identify high-value customers who respond well to discounts
- Determine which products and categories perform best by rating and order volume
- Evaluate the impact of shipping type and subscription status on spend
- Segment customers into New, Returning, and Loyal tiers to guide retention strategy

---
<h2><a class="anchor" id="dataset"></a>Dataset</h2>

- 3,900 rows across 18 columns
- Customer demographics: Age, Gender, Location, Subscription Status
- Purchase details: Item Purchased, Category, Purchase Amount, Season, Size, Color
- Shopping behavior: Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type
- Missing data: 37 values in the Review Rating column

---
<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>

- Python (Pandas — data cleaning, feature engineering)
- PostgreSQL (Common Table Expressions, Window Functions, Aggregations)
- Power BI (Interactive Visualizations)
- GitHub

---
<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>

```
customer-trends-data-analysis-sql-python-powerbi/
│
├── README.md
│
├── notebooks/
│   └── Customer_Shopping_Behavior_Analysis.ipynb
│
├── sql/
│   └── customer_behavior_sql_queries.sql
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── dashboard/
│   └── customer_behavior_dashboard.pbix
│
└── docs/
    ├── Customer_Shopping_Behavior_Analysis.pdf
    └── Customer-Shopping-Behavior-Analysis.pptx
```

---
<h2><a class="anchor" id="data-cleaning--preparation"></a>Data Cleaning & Preparation</h2>

- Loaded the dataset using Pandas; checked structure with `df.info()` and summary stats with `.describe()`
- Identified 37 missing values, all in the Review Rating column
- Imputed missing Review Rating values using the median rating of each product category
- Standardized column names to snake_case for readability
- Engineered an `age_group` column by binning customer ages into four quantile-based groups (Young Adult, Adult, Middle-aged, Senior)
- Engineered a `purchase_frequency_days` column, mapping purchase frequency labels (e.g. Weekly, Quarterly) to numeric day intervals
- Verified `discount_applied` and `promo_code_used` were identical across all rows; dropped the redundant `promo_code_used` column
- Connected the cleaned DataFrame to PostgreSQL for structured SQL analysis

---
<h2><a class="anchor" id="exploratory-data-analysis-eda"></a>Exploratory Data Analysis (EDA)</h2>

**Revenue by Gender:**
- Male customers generated **$157,890** in total revenue vs. **$75,191** from female customers — male customers contribute the larger share

**Product Ratings:**
- Top 5 products by average review rating: **Gloves (3.86)**, **Sandals (3.84)**, **Boots (3.82)**, **Hat (3.80)**, **Skirt (3.78)**

**Shipping Type Impact:**
- Express shipping customers average **$60.48** per purchase vs. **$58.46** for Standard — a modest but consistent premium

**Subscription Impact:**
- Subscribers (1,053 customers): average spend **$59.49**, total revenue **$62,645**
- Non-subscribers (2,847 customers): average spend **$59.87**, total revenue **$170,436**
- Non-subscribers slightly out-spend subscribers on average, and contribute far more in aggregate revenue simply due to volume

**Discount-Dependent Products:**
- Highest discount-purchase rates: **Hat (50.00%)**, **Sneakers (49.66%)**, **Coat (49.07%)**, **Sweater (48.17%)**, **Pants (47.37%)**

**Customer Segmentation** (by previous purchase count):
- **Loyal: 3,116** customers, **Returning: 701**, **New: 83**

**Repeat Buyers & Subscription:**
- Among customers with more than 5 previous purchases, **2,518** are not subscribed vs. **958** who are — repeat purchasing does not strongly correlate with subscription

**Revenue by Age Group:**
- **Young Adult: $62,143**, **Middle-aged: $59,197**, **Adult: $55,978**, **Senior: $55,763** — revenue is fairly evenly distributed across age groups

---
<h2><a class="anchor" id="research-questions--key-findings"></a>Research Questions & Key Findings</h2>

1. **Revenue by Gender**: Male customers generate significantly more total revenue than female customers ($157,890 vs. $75,191)
2. **High-Spending Discount Users**: 839 customers used a discount while still spending above the overall average purchase amount, indicating discounts don't always signal price sensitivity
3. **Top-Rated Products**: Gloves, Sandals, and Boots lead in average customer satisfaction (all above 3.8)
4. **Shipping Preference**: Express shipping customers spend marginally more per order ($60.48 vs. $58.46) than Standard shipping customers
5. **Subscription Value**: Subscribers do not out-spend non-subscribers on a per-purchase basis — subscription status alone isn't a reliable spend predictor
6. **Customer Loyalty**: The vast majority of the customer base (3,116 of 3,900) already qualifies as "Loyal" by purchase history, with only 83 truly new customers
7. **Category Leaders**: Jewelry, Blouse, Sandals, and Jacket rank as the top-ordered items in their respective categories (Accessories, Clothing, Footwear, Outerwear)

---
<h2><a class="anchor" id="dashboard"></a>Dashboard</h2>

- Power BI Dashboard ("Customer Behavior Dashboard") shows:
  - KPI cards: Number of Customers, Average Purchase Amount, Average Review Rating
  - % of Customers by Subscription Status (donut chart)
  - Revenue by Category and Sales by Category (column charts)
  - Revenue by Age Group and Sales by Age Group (bar charts)
  - Slicers: Subscription Status, Gender, Category, Shipping Type

![image alt](https://github.com/samyakmda/customer-trends-data-analysis-sql-python-powerbi/blob/d31c33927c465a5ef0ae526c26b2c4cb9cf0583e/Images/Screenshot%202026-08-28%20143752.png)

---
<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

1. Clone the repository:
```bash
git clone https://github.com/samyakmda/customer-trends-data-analysis-sql-python-powerbi.git
```
2. Open and run the data cleaning and feature engineering notebook:
```
notebooks/Customer_Shopping_Behavior_Analysis.ipynb
```
3. Load the cleaned data into PostgreSQL, then run the analysis queries:
```
sql/customer_behavior_sql_queries.sql
```
4. Open the Power BI dashboard:
```
dashboard/customer_behavior_dashboard.pbix
```

---
<h2><a class="anchor" id="final-recommendations"></a>Final Recommendations</h2>

- Target high-revenue segments — male customers and the Young Adult age group — with tailored campaigns
- Promote express shipping upgrades, since these customers already show a higher average spend
- Reassess subscription program value proposition, since subscribers currently spend about the same as non-subscribers per purchase
- Focus new-customer acquisition efforts, since only 83 of 3,900 customers currently fall into the "New" segment
- Highlight top-rated products (Gloves, Sandals, Boots) in marketing and product placement
- Review discount strategy for high-discount-rate items (Hat, Sneakers, Coat) to balance sales volume against margin

---
<h2><a class="anchor" id="author--contact"></a>Author & Contact</h2>

**Samyak Meshram**
Data Analyst
📧 Email: [samyakmda@gmail.com](mailto:samyakmda@gmail.com)
🔗 [LinkedIn](https://www.linkedin.com/in/ayushi-mishra-30813b174/)
🔗 [Portfolio](https://www.youtube.com/@techclasses0810/)
