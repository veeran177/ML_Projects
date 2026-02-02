Airline Fare Prediction – End-to-End Data Science Project

A Real-World Machine Learning Project on Travel Domain (EaseMyTrip Dataset)
1. Problem Overview
Airline ticket prices are dynamic. They depend on multiple factors such as demand, route, airline carrier, time of travel, number of stops, and even seasonality. Predicting flight fares with high accuracy is a multi-factor regression problem used widely in the travel industry for:
Revenue optimization
Competitive pricing
Customer recommendation systems
Fare alerts & price forecasting engines

This project uses a real flight booking dataset inspired by EaseMyTrip, and applies statistical analysis + feature engineering + ML models to predict airline fares.

2. Project Structure
Airline_fare_prediction/
│── README.md
│── dataset.xlsx
│── airline_fare_prediction.ipynb


3. Business Objectives
✔ Understand key factors influencing flight ticket prices
✔ Perform exploratory data analysis
✔ Apply statistical hypothesis testing
✔ Engineer high-quality features
✔ Build multiple regression models
✔ Compare & select the best model
✔ Provide actionable insights for business decisions

4. Dataset Information
Column	Description
Airline	Name of airline carrier
Date_of_Journey	Travel date
Source	Departure city
Destination	Arrival city
Route	Flight route combination
Dep_Time	Departure time
Arrival_Time	Arrival time
Duration	Total travel time
Total_Stops	Number of stops
Price	TARGET variable (fare amount)

Rows: ~10,000
Target: Price (continuous numeric)

5. Exploratory Data Analysis (EDA)
Key insights discovered during EDA:

1. Jet Airways & IndiGo are the most frequently booked airlines.
2. Evening flights are generally more expensive.
3. Non-stop flights have significantly higher fares.
4. Duration shows strong correlation with flight price.
5. Price varies heavily by month and travel season.

Visualizations Included:

Flight Price Distribution
Airline vs Average Fare
Source–Destination Fare Heatmap
Number of Stops vs Fare
Duration vs Fare Regression Plot
Correlation Heatmap
Feature importances

6. Feature Engineering

To improve model performance, the following features were engineered:

✔ Date Features
Journey_Day
Journey_Month
Journey_Year

✔ Time Features
Dep_hour, Dep_minute
Arrival_hour, Arrival_minute

✔ Duration Features
Converted duration into minutes
Extracted hours/minutes separately

✔ Route Features
Number of legs in route
Presence of common layovers

✔ Stops
Converted text → numeric:

Text	Value
non-stop	0
1 stop	1
2 stops	2
3 stops	3

7. Statistical Hypothesis Testing
1️⃣ ANOVA

Used to determine whether different airlines have significantly different mean ticket prices.

Result: Significant (p < 0.05) → Airline strongly impacts fare.

2️⃣ t-Test

Compared non-stop vs multi-stop flights.

Result: Non-stop flights are significantly more expensive.

3️⃣ Correlation Significance Test

Duration shows statistically significant correlation with price.

8. Models Applied

This project uses a full regression modeling pipeline, including:

✔ Linear Regression
✔ Lasso Regression
✔ Ridge Regression
✔ Random Forest Regressor
✔ Gradient Boosting Regressor
✔ XGBoost Regressor
✔ LightGBM Regressor

Each model was evaluated using:
RMSE
MAE
R² Score

9. Model Performance Comparison
Model	RMSE	MAE	R²
Linear Regression	High error	–	Poor
Random Forest	Best	Best	0.87
Gradient Boosting	Moderate	–	0.81
XGBoost	Competitive	–	0.84
LightGBM	Similar to RF	–	0.85

Best Model: RandomForestRegressor
✔ Excellent generalization
✔ Handles categorical + numerical mix well
✔ Less sensitive to outliers

10. How to Run the Project
1. Clone Repo
git clone https://github.com/veeran177/ML_Projects.git
cd ML_Projects/Airline_fare_prediction

2. Install Requirements
pip install -r requirements.txt

3. Run Notebook
Open:
airline_fare_prediction.ipynb

4. Adjust file paths if needed

11. Future Improvements
✔ Add Deep Learning (ANN Regressor)
✔ Add price forecasting using Time Series
✔ Build a simple Streamlit dashboard (optional)
✔ Add SHAP explainability
✔ Add hyperparameter optimization via Optuna
✔ Deploy using FastAPI or Flask (optional)

12. Tech Stack Used

Languages: Python
Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, XGBoost, LightGBM
Tools: Jupyter Notebook, Git

13. Credits
Dataset inspired by EaseMyTrip flight booking data.
Project by Veeran K (2025).
