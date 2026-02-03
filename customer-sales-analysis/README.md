# Customer Sales & Risk Analysis using Python

## Problem Statement
Businesses need to understand customer purchasing behavior to improve revenue and reduce churn.
This project performs an end-to-end exploratory data analysis (EDA) and risk profiling on customer sales data
to identify high-value customers, revenue concentration risks, and churn-prone segments.

## Tech Stack
- Python
- Pandas, NumPy
-Customer Sales & Churn Risk Analysis (EDA + ML)
🔍 Project Overview

This project performs an end-to-end customer sales analysis and churn risk prediction using Python.
It starts with exploratory data analysis (EDA) to understand customer behavior and revenue patterns, followed by machine learning models to identify customers at high risk of churn.

The goal is to help businesses reduce revenue loss by proactively identifying churn-prone customers and enabling targeted retention strategies.

🧠 Business Problem

Businesses often lose revenue because they fail to identify customers who are likely to churn.
Using historical transaction data, this project aims to:

Understand customer purchasing behavior

Identify high-value and high-risk customers

Predict churn risk using machine learning models

🛠️ Tech Stack

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

Jupyter Notebook

📊 Dataset Description

Retail sales transaction dataset containing:

Invoice details

Product pricing and quantity

Customer identifiers

Country-level information

Each row represents a transaction, which is later aggregated to a customer-level dataset for machine learning.

🔍 Project Workflow

Data loading and cleaning

Exploratory Data Analysis (EDA)

Feature engineering (Total Revenue, Purchase Frequency, etc.)

Customer segmentation and risk profiling

Churn risk label creation using business logic

Model training (Logistic Regression & Random Forest)

Model evaluation using ROC-AUC

Threshold tuning for business impact

📈 Key Insights

A small percentage of customers contribute a large portion of total revenue (revenue concentration risk)

One-time and low-value customers represent high churn risk

Purchase frequency and total revenue are the strongest churn predictors

Random Forest outperformed Logistic Regression in identifying high-risk customers

🤖 Machine Learning Models
Model	Purpose
Logistic Regression	Baseline, interpretable model
Random Forest	Captures non-linear customer behavior

Evaluation Metric: ROC-AUC
Final Strategy: Threshold tuning to maximize recall and reduce missed churn cases

💡 Business Recommendations

Implement loyalty programs for high-value customers

Use predictive churn scores to trigger retention campaigns

Reduce dependency on a small group of customers

Continuously retrain models with new transaction data

📂 Project Structure
customer-sales-analysis/
├── data/
├── notebooks/
├── outputs/
└── README.md

🚀 Outcome

This project demonstrates how raw transactional data can be transformed into actionable business insights and predictive models, making it suitable for real-world deployment in CRM and marketing systems.
Matplotlib, Seaborn
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
