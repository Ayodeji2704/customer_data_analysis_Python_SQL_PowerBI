# 👨🏻‍💻Customer Shopping Behaviour Analysis

## 📋 Overview

This project analyzes transactional data from 3,900 purchases to uncover insights into customer spending patterns, segmentation, product preferences, and subscription behavior. The goal is to support data-driven business decisions through exploratory analysis, SQL queries, and interactive dashboarding.

### 📁 Dataset
Rows: 3,900

Columns: 18

Key Features:

- Customer demographics (Age, Gender, Location, Subscription Status)

- Purchase details (Item, Category, Amount, Season, Size, Color)

- Shopping behavior (Discount Applied, Promo Code Used, Previous Purchases, Frequency, Review Rating, Shipping Type)

- Missing Data: 37 values in the Review Rating column (handled during preprocessing).

## **🛠 Tech Stack & Methodology**

Python (Pandas) – Data cleaning, preprocessing, and feature engineering

PostgreSQL – Structured querying and business intelligence analysis

Power BI – Interactive dashboard for visualization and reporting

Methodology:

Data cleaning and imputation
Feature engineering (age groups, purchase frequency)
SQL analysis for business questions
Dashboard creation for stakeholder presentation
### 📊 Steps
1. Data Preparation (Python)
   - Loaded dataset using pandas

   - Explored structure and statistics ```df.info()``` & ```df.describe()```

   - Handled missing values in Review Rating using median imputation per category

   - Standardized column names to snake_case

   - Created new features:

     ```age_group``` (binned ages)

     ```purchase_frequency_days```

   - Removed redundant column (promo_code_used)

   - Exported cleaned data to PostgreSQL

2. SQL Analysis (PostgreSQL)  
   Performed 11 key analyses, including:

   - Revenue by gender

   - High-spending discount users

   - Top-rated products

   - Shipping type comparison

   - Subscriber vs. non-subscriber behavior

   - Customer segmentation (New, Returning, Loyal)

   - Top products by category and season

   - Repeat buyer subscription likelihood

   - Revenue by age group

3. Dashboarding (Power BI)  
Built an interactive dashboard to visualize:

   - Revenue trends

   - Customer segments

   - Product performance

   - Seasonal purchasing patterns

   - Subscription insights

4. Presentation & Reporting  
Developed a PowerPoint presentation summarizing insights and business recommendations

## 📈 Dashboard
The Power BI dashboard provides an interactive view of key metrics and trends, allowing stakeholders to filter by demographics, season, product category, and more.

<img width="950" height="560" alt="customer_analysis POWER BI Dashboard" src="https://github.com/user-attachments/assets/1104d236-5a22-41e8-8341-446facfded15" />


**Dashboard screenshot also included in project report.**

## 📌 Key Results & Insights
- Gender Revenue Gap - Female customers contributed significantly more revenue than male customers.

- Discount Impact - High spending customers still use discounts, indicating price sensitivity among big buyers.

- Top Products - Identified highest-rated and most frequently purchased items per category.

- Shipping Preference - Express shipping users tend to spend more on average.

- Subscriber Value - Subscribers generate higher average purchase values and total revenue.

- Seasonal Trends - Clear purchasing patterns aligned with seasons.

- Loyalty Potential - Repeat buyers are more likely to subscribe.

## 🧭 Business Recommendations
- Boost Subscriptions – Offer exclusive perks to increase subscriber conversion.

- Loyalty Programs – Incentivize repeat purchases to move customers into “Loyal” segment.

- Discount Strategy – Review discount policies to balance sales volume and profit margins.

- Product Highlighting – Promote top-rated and best-selling products in marketing campaigns.

- Seasonal Planning – Optimize inventory and promotions based on seasonal top-sellers.

- Targeted Marketing – Focus on high-revenue age groups and express shipping users.

## 🚀 How to Run
### Prerequisites
  - Python 3.8+

  - PostgreSQL

  - Power BI (for dashboard viewing)

  - Jupyter Notebook or preferred Python IDE

### Steps 
1. Clone the repository  
   ```
   git clone https://github.com/Ayodeji2704/customer_data_analysis_Python_SQL_PowerBI.git
   cd customer_data_analysis_Python_SQL_PowerBI
   ```
2. Install required Python Packages
   ```
   pip install pandas psycopg2 sqlalchemy
   ```
3. Run the Python script to clean and load the data into PostgreSQL

4. Execute SQL queries in PostgreSQL to answer business questions and reproduce the analysis

5. Open the Power BI file to explore the interactive dashboard 
