# Customer Sales & Risk Analysis using Python

## Problem Statement
Businesses need to understand customer purchasing behavior to improve revenue and reduce churn.
This project performs an end-to-end exploratory data analysis (EDA) and risk profiling on customer sales data
to identify high-value customers, revenue concentration risks, and churn-prone segments.

## Tech Stack
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

## Dataset
Retail transaction dataset containing invoices, products, customer IDs, pricing, and country information.

## Key Analysis Performed
- Data cleaning and preprocessing
- Feature engineering (TotalPrice, time-based features)
- Customer segmentation (High / Medium / Low value)
- Repeat vs One-time customer analysis
- Revenue concentration risk analysis
- Visual trend and distribution analysis

## Key Insights
- Top customers contribute a significant portion of total revenue, indicating concentration risk
- High-value customers form a small segment but drive most revenue
- One-time, low-value customers represent high churn risk
- Sales show seasonal trends across months

## Business Recommendations
- Introduce loyalty programs for high-value customers
- Target medium-value customers with personalized offers
- Reduce marketing spend on low-value one-time customers
- Diversify customer base to minimize revenue dependency risk

## Project Structure
customer-sales-analysis/
├── data/
├── notebooks/
├── outputs/
└── README.md
