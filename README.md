# Ecommerce Customer Analysis

I built this project to dive deep into how e-commerce businesses can actually use their data to make better decisions. Instead of just looking at total sales, I wanted to see if I could figure out who the most valuable customers are, who we might be losing, and how much a customer is likely to be worth over time.

## Why this project?
In a real business, you can't treat every customer the same. Some people buy once and never come back, while others are "champions" who keep the lights on. I wanted to apply common data science techniques like RFM analysis and CLV modeling to a transactional dataset to turn raw numbers into actual business strategy.

## What's in the data?
The dataset tracks individual transactions. It's got the usual stuff you'd expect:
- Customer and Order IDs
- Transaction dates
- Product info (categories, prices)
- Discounts and payment methods
- Locations (mostly India, USA, UK, etc.)

## The Game Plan
I broke the analysis down into a few main stages:

### 1. Cleaning and Prep
Data is rarely ever ready to go. I had to handle missing values, get rid of duplicates, and make sure dates were actually in a format Python could work with. I also calculated the "total amount" for each order by factoring in price, quantity, and discounts.

### 2. Exploratory Analysis (EDA)
Before doing anything fancy, I looked at the trends. I plotted out monthly revenue to see how the business was performing over time and checked which categories were the most popular.

### 3. RFM Analysis & Segmentation
This was the core part. I scored every customer on three things:
- **Recency:** How long has it been since their last order?
- **Frequency:** How often do they shop?
- **Monetary:** How much have they spent in total?

Based on these scores, I grouped them into segments like 'Champions', 'Loyal Customers', 'At Risk', and 'Needs Attention'. This makes it much easier to decide who to send a discount code to and who to invite to a loyalty program.

### 4. CLV and Churn
I also calculated the **Customer Lifetime Value (CLV)** to estimate long-term revenue and flagged anyone who hadn't bought anything in over 90 days as "churned."

## What I found
- A small group of **Champions** actually drives a huge chunk of the revenue.
- If a customer stops buying for 90 days, there's a really high chance they won't come back without some kind of nudge.
- Discounts are great, but they don't always mean a customer will stay loyal in the long run.

## Recommendations
- **Reward the best:** Give the "Champions" early access or special perks.
- **Save the "At Risk":** Focus re-engagement emails on people who used to be active but have gone quiet.
- **Watch the margins:** Don't just throw discounts at everyone; use the CLV data to see where it actually makes sense.

## How to run it
If you want to check out the code:
1. Clone this repo.
2. Make sure you have `pandas`, `matplotlib`, and `seaborn` installed.
3. Open up `notebooks/analysis.ipynb` in Jupyter or VS Code.

## Project Structure
- `data/`: Contains the raw and processed CSV files.
- `notebooks/`: This is where the actual Python analysis lives.
- `report.pdf`: A summary report of the findings.
- `dashboard/`: A placeholder for some visual charts.

---
**Author:** Kumar Gautam  
Just a project to explore the intersection of Data and Business.
