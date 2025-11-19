🚢 Maritime CO₂ Emission Prediction using Machine Learning
📌 Project Overview

This project focuses on predicting CO₂ emissions from maritime ships based on operational parameters such as fuel consumption, distance, weather conditions, and ship type. The objective is to build a machine learning model that helps optimize fuel usage and reduce carbon emissions in maritime logistics—aligned with global sustainability goals.

The dataset was synthetically created to simulate real-world maritime operational records.

🎯 Objectives

Perform exploratory data analysis (EDA) and understand core relationships.

Apply feature engineering to enhance predictive capability.

Train and evaluate multiple machine learning regression models.

Identify the best-performing model using evaluation metrics.

Demonstrate a real-world business problem-solving approach.

📂 Dataset Description
Column Name	Description
ship_id	Unique identifier for ship
ship_type	Category of vessel
route_id	Route identifier
month	Month of travel
distance	Distance covered (km)
fuel_type	Type of fuel used
fuel_consumption	Fuel consumed (liters)
CO2_emissions	CO₂ emitted (kg)
weather_conditions	Weather severity rating
engine_efficiency	Engine performance score
fuel_per_km	Engineered feature
co2_per_km	Engineered feature
season / season_name	Derived from month
🔧 Feature Engineering Performed

Created fuel_per_km = fuel_consumption / distance

Created co2_per_km = CO2_emissions / distance

Extracted seasonal category & labels from month

📊 Model Comparison
Model	R² Score	RMSE	MAE
Linear Regression	0.9984	204	141
Gradient Boosting	0.9971	276	137
Random Forest	0.9954	351	213
Tuned Random Forest	0.9937	408	226
🏆 Best Model: Linear Regression

Selected for highest accuracy and best generalization.

🔍 Key Insights

Fuel consumption and distance strongly correlate with emissions.

Weather severity & engine efficiency significantly influence fuel usage.

Simple models can outperform complex ensemble methods in clean linear patterns.

🚀 Tech Stack

Python

Pandas, NumPy, Matplotlib, Seaborn

Scikit-learn

Jupyter Notebook

📦 Project Structure
├── data/
├── notebooks/
├── models/
├── README.md
└── requirements.txt

🧠 Future Improvements

Deploy API using FastAPI / Flask

Integrate dashboard via Streamlit or Power BI

Test deep learning models such as LSTM for time-series ship data

🙌 Acknowledgements

This project was developed as part of interview preparation for a Business Analyst / Data Analyst role in the maritime domain. Inspired by operational sustainability initiatives like ZeroNorth.
