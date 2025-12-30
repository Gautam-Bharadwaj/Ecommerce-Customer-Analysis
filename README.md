# Simple E-commerce Customer Analysis

I made this project to show some basic data analysis on e-commerce sales. It’s a simple project that takes raw order data and turns it into easy-to-read charts.

## What is this project?
The goal here is simple:
1. Clean up a list of e-commerce orders.
2. Figure out which categories are selling the most.
3. Find out who the top customers are.

## The Data
The data comes from a CSV file with columns like:
- **Order Date:** When the purchase happened.
- **Category:** What kind of item was bought (Electronics, Clothing, etc.).
- **Price & Quantity:** How much it cost and how many were bought.
- **Discount:** Any money taken off the price.

## Steps I took

### 1. Cleaning the Data
I used Python to:
- Convert dates into a format the computer understands.
- Calculate the `total_amount` for every order (Price * Quantity - Discount).

### 2. Basic Charts
I created two main charts:
- **Sales by Category:** To see which products are the most popular.
- **Top Customers:** To see who is spending the most money.

### 3. Customer Status
I added a simple label to each order:
- **High Value:** If the spending is above average.
- **Standard:** If it’s below average.

## How to run it
1. Make sure you have `pandas`, `seaborn`, and `matplotlib` installed on your computer.
2. Open the `notebooks/analysis.ipynb` file in VS Code or Jupyter Notebook.
3. Run the cells to see the charts!

## Folder Structure
- `data/`: The CSV files (raw and cleaned).
- `notebooks/`: The Python code for the analysis.
- `README.md`: This file.

---
**Author:** Kumar Gautam  
A simple data analysis project.
