# 👨🏻‍💻Customer Behavior Data Analyst Portfolio Project
This project represents a complete, industry standard, end-to-end data analytics workflow, designed to mirror the real responsibilities of professional analysts in modern business environments. The project encompasses all critical stages of data analysis, from data preparation and modeling to insight generation, visualization, and reporting.


## 📌 Project Overview
The goal of this project is to simulate a corporate-grade end-to-end data analytics workflow, demonstrating the ability to translate raw data into strategic business intelligence by:

✅ Data Preparation,Modeling & Exploratory Data Analysis (Python): Clean and transform the raw dataset for analysis.

✅ Data Analysis (SQL): Simulate business transactions, and run queries to extract insights on customer segments, loyalty, and purchase drivers.

✅ Visualization & Insights (Power BI): Build an interactive dashboard that highlights key patterns and trends, enabling stakeholders to make data-driven decisions.

✅ Report and Presentation: Write a clear project report summarizing your key findings and business recommendations. Prepare a presentation that visually communicates insights and actionable recommendations to stakeholders.

![Project Workflow](https://github.com/user-attachments/assets/8bbd5dc9-eb6c-40c1-8f19-c08b4107f654)

## 🛠️ How to Use This Project

1. **Clone the repository**
   ```bash
   git clone https://github.com/amlanmohanty1/customer-trends-data-analysis-SQL-Python-PowerBI.git
   cd customer-trends-data-analysis-SQL-Python-PowerBI
   ```
2. **Open Customer_Shopping_Behavior_Analysis.ipynb notebook**

    This file contains:

      - Data Import

      - Data exploration

      - Data cleaning

      - Connection to SQL Database
  
3. **Load the data from Python notebook into MySQL/PostgreSQL/MS SQL Server**

      - Create a database in SQL

      - Run Python code to load data into SQL database
  
      - Open **customer_behavior_sql_queries.sql**
  
      - Answer Business Questions using SQL Queries 
      
4. **Connect the SQL Database to Power BI**

      - Open **customer_behavior_dashboard.pbix**
   
      - Create interactive dashboard in Power BI
  
6. **Create Project Report and Presentation**

      - Create project report
   
      - Build presentation deck using Gamma AI


# 👨🏻‍💻 Customer Behavior Data Analyst Portfolio Project

*Analyzing customer shopping behavior to uncover purchasing patterns, customer segments, loyalty drivers, and actionable business insights using SQL, Python, and Power BI.*

---

## 📌 Table of Contents

* <a href="#overview">Overview</a>
* <a href="#business-problem">Business Problem</a>
* <a href="#dataset">Dataset</a>
* <a href="#tools--technologies">Tools & Technologies</a>
* <a href="#project-structure">Project Structure</a>
* <a href="#data-cleaning--preparation">Data Cleaning & Preparation</a>
* <a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a>
* <a href="#research-questions--key-findings">Research Questions & Key Findings</a>
* <a href="#dashboard">Dashboard</a>
* <a href="#how-to-run-this-project">How to Run This Project</a>
* <a href="#final-recommendations">Final Recommendations</a>
* <a href="#author--contact">Author & Contact</a>

---

<h2><a class="anchor" id="overview"></a>Overview</h2>

This project analyzes customer shopping behavior through an end-to-end data analytics workflow. The objective is to transform raw customer transaction data into meaningful business insights that can support customer segmentation, loyalty analysis, purchasing strategy, and data-driven decision-making.

The project follows an industry-oriented analytics workflow covering data preparation, exploratory analysis, SQL-based business analysis, dashboard development, and business recommendations.

---

<h2><a class="anchor" id="business-problem"></a>Business Problem</h2>

Understanding customer purchasing behavior is essential for improving customer engagement, retention, and revenue.

This project aims to:

* Identify important customer purchasing patterns
* Analyze customer segments and shopping behavior
* Understand factors influencing purchasing decisions
* Evaluate customer loyalty and repeat-purchase behavior
* Identify high-value customer segments
* Analyze purchasing trends across customer demographics and categories
* Generate actionable recommendations for business stakeholders

---

<h2><a class="anchor" id="dataset"></a>Dataset</h2>

The project uses a customer shopping behavior dataset containing transactional and customer-level information.

The dataset is used to analyze:

* Customer demographics
* Product categories
* Purchase amounts
* Purchase frequency
* Customer segments
* Discounts and promotional behavior
* Shopping preferences
* Customer ratings
* Payment methods
* Subscription and loyalty-related behavior

The raw data is first processed using Python and subsequently loaded into a SQL database for structured business analysis.

---

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>

* **Python** — Data cleaning, transformation, and Exploratory Data Analysis
* **Pandas** — Data manipulation and analysis
* **NumPy** — Numerical analysis
* **Matplotlib & Seaborn** — Data visualization
* **SQL** — Business analysis, filtering, aggregation, joins, and analytical queries
* **Power BI** — Interactive dashboard and visualization
* **Jupyter Notebook** — Analysis and documentation
* **GitHub** — Version control and project documentation

---

<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>

```text
customer-trends-data-analysis-SQL-Python-PowerBI/
│
├── README.md
├── requirements.txt
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── notebooks/
│   └── Customer_Shopping_Behavior_Analysis.ipynb
│
├── sql/
│   └── customer_behavior_sql_queries.sql
│
├── dashboard/
│   └── customer_behavior_dashboard.pbix
│
├── report/
│   └── Customer_Behavior_Analysis_Report.pdf
│
└── presentation/
    └── Customer_Behavior_Analysis_Presentation.pdf
```

---

<h2><a class="anchor" id="data-cleaning--preparation"></a>Data Cleaning & Preparation</h2>

Python and Pandas were used to prepare the raw customer shopping dataset for analysis.

Key data preparation steps included:

* Imported the raw customer shopping dataset
* Inspected dataset structure and data types
* Identified missing and inconsistent values
* Cleaned and transformed relevant columns
* Converted columns into appropriate data types
* Performed exploratory data analysis to understand the dataset
* Prepared the cleaned dataset for SQL analysis
* Loaded the processed data into a SQL database

---

<h2><a class="anchor" id="exploratory-data-analysis-eda"></a>Exploratory Data Analysis (EDA)</h2>

Exploratory Data Analysis was performed using Python to understand customer behavior and identify important patterns before conducting SQL analysis.

The analysis focused on:

* Customer demographics
* Purchase behavior
* Product category performance
* Purchase frequency
* Customer spending patterns
* Discounts and promotional behavior
* Customer ratings
* Payment methods
* Subscription behavior
* Customer segmentation

Visualizations were created using Matplotlib and Seaborn to identify trends, distributions, relationships, and potential business opportunities.

---

<h2><a class="anchor" id="research-questions--key-findings"></a>Research Questions & Key Findings</h2>

The project uses SQL to answer business-oriented questions related to customer behavior and purchasing patterns.

Key areas of analysis include:

1. **Customer Segmentation**
   Analyze customers based on their purchasing behavior, demographics, and spending patterns.

2. **Customer Loyalty**
   Identify behavioral patterns associated with loyal and repeat customers.

3. **Purchase Drivers**
   Investigate factors that influence customer purchasing decisions.

4. **Product Category Analysis**
   Determine which product categories perform strongly across different customer segments.

5. **Discount & Promotion Analysis**
   Analyze the relationship between discounts and customer purchasing behavior.

6. **Customer Spending Analysis**
   Identify high-value customers and understand their purchasing characteristics.

7. **Subscription & Loyalty Analysis**
   Evaluate customer behavior based on subscription and loyalty-related attributes.

8. **Customer Ratings**
   Analyze customer ratings to identify patterns in customer satisfaction and purchasing behavior.

> **Note:** Add your actual numerical findings here after completing the SQL analysis and Power BI dashboard. Avoid adding percentages or business conclusions that have not been calculated from the dataset.

---

<h2><a class="anchor" id="dashboard"></a>Dashboard</h2>

The Power BI dashboard provides an interactive view of customer shopping behavior and business performance.

The dashboard focuses on:

* Customer demographics
* Customer segments
* Purchase behavior
* Product category performance
* Revenue and spending patterns
* Discount behavior
* Customer loyalty
* Subscription analysis
* Customer ratings
* Interactive filters and business KPIs

The dashboard enables stakeholders to explore customer behavior and identify actionable trends through interactive visualizations.

---

<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

### 1. Clone the repository

```bash
git clone https://github.com/samyakmda/customer-trends-data-analysis-SQL-Python-PowerBI.git
cd customer-trends-data-analysis-SQL-Python-PowerBI
```

### 2. Install the required Python libraries

```bash
pip install -r requirements.txt
```

### 3. Open the Python notebook

Open:

```text
notebooks/Customer_Shopping_Behavior_Analysis.ipynb
```

The notebook contains:

* Data import
* Data exploration
* Data cleaning
* Data transformation
* Exploratory Data Analysis
* SQL database connection
* Data loading

### 4. Load the data into SQL

Create a database using your preferred SQL database system such as:

* PostgreSQL
* MySQL
* Microsoft SQL Server

Run the Python notebook to load the processed dataset into the SQL database.

### 5. Run SQL analysis

Open:

```text
sql/customer_behavior_sql_queries.sql
```

Execute the queries to answer the project's business questions and generate customer behavior insights.

### 6. Open the Power BI dashboard

Open:

```text
dashboard/customer_behavior_dashboard.pbix
```

Connect Power BI to the SQL database and refresh the data if required.

### 7. Review the project report and presentation

The project report summarizes:

* Analytical approach
* Key findings
* Business insights
* Recommendations

The presentation communicates the major insights and recommendations in a stakeholder-friendly format.

---

<h2><a class="anchor" id="final-recommendations"></a>Final Recommendations</h2>

Based on the analysis, the project is designed to provide recommendations around:

* Targeting high-value customer segments
* Improving customer loyalty and retention
* Optimizing promotional and discount strategies
* Personalizing marketing campaigns
* Improving product-category strategies
* Identifying opportunities to increase customer spending
* Using customer behavior to improve business decision-making

> **Important:** Final recommendations should be updated with specific evidence from your SQL analysis and Power BI results.

---

<h2><a class="anchor" id="author--contact"></a>Author & Contact</h2>

**Samyak Meshram**
Data Analyst

📧 Email: [samyakmda@gmail.com](mailto:samyakmda@gmail.com)

🔗 LinkedIn: https://www.linkedin.com/in/ayushi-mishra-30813b174/

🔗 Portfolio: https://www.youtube.com/@techclasses0810/

---

## ⭐ Project Highlights

This project demonstrates an end-to-end Data Analyst workflow:

**Raw Data → Python → Data Cleaning → EDA → SQL → Business Analysis → Power BI → Insights → Recommendations**

The project showcases practical skills in:

* Data Cleaning
* Exploratory Data Analysis
* SQL Analytics
* Customer Segmentation
* Business Intelligence
* Data Visualization
* Dashboard Development
* Business Problem Solving
* Insight Generation

  


💼 LinkedIn: [Amlan Mohanty](https://www.linkedin.com/in/amlanmohanty1/)
- Let’s connect professionally and grow your data career
