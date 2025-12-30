# E-commerce Customer Analysis

## Objective
The objective of this project is to perform an advanced analysis of e-commerce customer data to understand purchasing behavior, identify high-value customers, calculate customer lifetime value (CLV), and analyze churn patterns. The insights derived from this analysis aim to support data-driven business and marketing decisions.

---

## Dataset Description
The dataset contains transactional data from an e-commerce platform, including customer details, orders, products, pricing, and discounts.

### Key Columns:
- customer_id  
- order_id  
- order_date  
- product_id  
- category  
- price  
- quantity  
- discount  
- payment_method  
- country  

---

## Tools & Technologies Used
- **Python** (Pandas, NumPy)
- **Data Visualization** (Matplotlib, Seaborn)
- **Jupyter Notebook**
- **Power BI** (for dashboard – optional)
- **Git & GitHub**

---

## Key Analysis Performed

### 1. Data Cleaning & Preparation
- Removed duplicate records
- Handled missing values
- Converted date columns to proper datetime format
- Created new features such as total revenue and order month

---

### 2. Exploratory Data Analysis (EDA)
- Monthly revenue trends
- Customer purchasing patterns
- Product and category-level insights

---

### 3. RFM Analysis (Recency, Frequency, Monetary)
- **Recency**: Days since last purchase  
- **Frequency**: Number of orders  
- **Monetary**: Total amount spent  

Customers were scored and segmented based on RFM values to identify:
- Champions
- Loyal Customers
- At-Risk Customers
- Customers Needing Attention

---

### 4. Customer Segmentation
Customers were grouped into meaningful segments using RFM scores to help tailor marketing and retention strategies.

---

### 5. Customer Lifetime Value (CLV)
CLV was calculated using:
CLV = Average Order Value × Purchase Frequency × Customer Lifespan

yaml
Copy code
This helps identify customers who contribute the most long-term revenue.

---

### 6. Churn Analysis
- Customers with no purchases in the last **90 days** were marked as churned
- Churn trends were analyzed across different customer segments

---

## Dashboard (Optional)
A dashboard was created to visualize:
- Revenue trends
- Customer segments
- Top-performing products
- Churn distribution

*(Dashboard files or screenshots are available in the `dashboard/` folder.)*

---

## Key Insights
- A small group of **Champion customers** contributes a large portion of total revenue.
- Customers inactive for more than 90 days show a high probability of churn.
- Loyal customers demonstrate consistent purchasing behavior and high engagement.
- Heavy discounting does not always correlate with higher customer lifetime value.

---

## Business Recommendations
- Offer exclusive rewards and early access deals to Champion customers.
- Run personalized re-engagement campaigns for At-Risk customers.
- Optimize discount strategies to focus on high-CLV segments.
- Use customer segmentation for targeted marketing and retention strategies.

---

## How to Run the Project
1. Clone the repository:
git clone <repository-url>

css
Copy code
2. Navigate to the project folder:
cd ecommerce-customer-analysis

markdown
Copy code
3. Open the notebook:
jupyter notebook notebooks/analysis.ipynb

yaml
Copy code

---

## Project Structure
ecommerce-customer-analysis/
│
├── dashboard/
├── data/
│ ├── raw_data.csv
│ └── cleaned_data.csv
├── notebooks/
│ └── analysis.ipynb
├── README.md
└── report.pdf

yaml
Copy code

---

## Conclusion
This project demonstrates how data analytics techniques such as RFM analysis, customer segmentation, churn detection, and CLV modeling can be applied to real-world e-commerce data to drive meaningful business decisions.

---

## Author
**Kumar Gautam**  
Data Analytics | Python | SQL | Business Insights
