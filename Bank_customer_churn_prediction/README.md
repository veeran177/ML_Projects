Bank Customer Churn Prediction (ML Classification Project)

Customer churn is one of the biggest challenges faced in the banking sector. Retaining an existing customer is 5x cheaper than acquiring a new one.
This project uses Machine Learning techniques to predict whether a customer is likely to leave the bank, enabling proactive retention strategies.

This repository contains a clean, analysis-first, ML pipeline to understand churn behavior and build predictive models.

Project Structure
Bank_customer_churn_prediction/
├── Bank_customer_churn_prediction_system.ipynb   # Main notebook
├── Bank_churn.csv                                 # Dataset
├── README.md                                       

Objective

Analyze customer behaviour
Identify which factors cause churn
Build ML models to predict customer churn
Compare model performance
Provide actionable insights

Dataset Description
The dataset contains 10,000 bank customers with features like:

Feature	Description
Geography	Country of customer
Gender	Male/Female
Age	Customer age
Balance	Account balance
Tenure	Number of years with bank
NumOfProducts	Count of bank products
HasCrCard	Credit card ownership
IsActiveMember	Activity indicator
EstimatedSalary	Salary estimation
Exited	Target variable (1 = churned, 0 = stayed)
🧹 1. Data Cleaning & Preprocessing

✔ Handled missing values
✔ Encoding categorical variables
✔ Feature scaling (StandardScaler)
✔ Train–test split

📊 2. Exploratory Data Analysis (with visuals)
🧁 Churn Distribution
![Churn Distribution](assets/churn_dist.png)

🎂 Churn by Gender
![Churn vs Gender](assets/churn_gender.png)

🌍 Churn by Geography
![Churn vs Geography](assets/churn_geo.png)

📈 Age vs Churn
![Age vs Churn](assets/age_churn.png)

🔥 Correlation Heatmap
![Correlation Heatmap](assets/corr_heatmap.png)


(You can export these from your notebook and store in assets/ folder.)

🤖 3. Machine Learning Models Trained

The following models were trained and evaluated:

Model	Type
Logistic Regression	Baseline classifier
Decision Tree	Non-linear classification
Random Forest	Ensemble learning
Gradient Boosting	Boosting algorithm
XGBoost	Advanced boosting
SVM	Margin-based classifier
KNN	Distance-based learning

📈 4. Model Evaluation

Evaluation metrics include:

Accuracy

Precision

Recall

F1 Score

ROC–AUC Curve

Confusion Matrix

🏆 Model Comparison (Bar Chart)
![Model Comparison](assets/model_compare.png)

📉 ROC Curves
![ROC Curves](assets/roc_curves.png)

Feature importance
<img width="855" height="570" alt="image" src="https://github.com/user-attachments/assets/c735aa0c-f7d2-45b7-abaf-260adf576e51" />

(Add these from your notebook too.)

💡 5. Key Insights
🔍 Customers more likely to churn:

Age 40–55 segment shows highest churn

Customers with 2+ products tend to churn less

Inactive members show significantly higher churn

High balance customers surprisingly churn more

Customers in Germany show highest churn

🛠 Recommended Business Actions:

Targeted retention offers for at-risk age segment

Customer engagement campaigns to increase activity

Better service offerings for German customers

Loyalty programs for high-balance customers

🧠 6. Final Best Model

The winning model in your notebook was:

⭐ Gradient Boosting / XGBoost

(Depending on your notebook results)

Why it performed better?

Handles non-linearity

Captures complex interactions

Robust against overfitting

Superior precision & recall

🚀 How to Run the Notebook

Clone the repository

Install required packages:

pip install -r requirements.txt


Run Jupyter Notebook

jupyter notebook


Open Bank_customer_churn_prediction_system.ipynb

📬 Contact

If you want help improving your ML/DS portfolio:
📧 veeran.k (or any email you share later)
💼 GitHub: github.com/veeran177
