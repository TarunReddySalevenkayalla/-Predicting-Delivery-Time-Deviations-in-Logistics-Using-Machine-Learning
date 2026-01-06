# Delivery Time Deviation Prediction Using Machine Learning # 

# Project Description

This repository contains the source code developed for an MSc Data Science individual project focused on predicting delivery time deviation in logistics operations using supervised machine-learning techniques. The project investigates how ensemble-based regression models can capture complex, non-linear relationships between operational, environmental, behavioural, and risk-related factors that influence delivery performance.

The implementation supports the experimental analysis and results presented in the accompanying MSc project report submitted to the University of Hertfordshire.
------

# Research Objective

The primary objective of this project is to evaluate the effectiveness of ensemble machine-learning models in predicting delivery time deviation as a continuous outcome variable. The study also examines the impact of feature engineering and interaction effects on predictive accuracy and model generalisation.

⸻

# Dataset

A publicly available logistics and supply chain dataset sourced from Kaggle was used in this study. The dataset contains approximately 32,000 delivery records with 26 attributes, representing:
	•	Operational variables (e.g. lead time, congestion indicators)
	•	Environmental conditions (e.g. weather severity)
	•	Behavioural indicators (e.g. driver fatigue and behaviour scores)
	•	Risk-related factors (e.g. port congestion and customs clearance)

A synthetic yet realistic target variable representing delivery time deviation was constructed using weighted operational signals with added Gaussian noise to simulate real-world uncertainty.
------

# Methodology

The project follows a structured machine-learning workflow:
	1.	Data loading and validation
	2.	Exploratory Data Analysis (EDA)
	3.	Data cleaning and preprocessing
	4.	Feature engineering, including interaction features
	5.	Train–test split (80% training, 20% testing)
	6.	Model training and evaluation
	7.	Feature importance analysis



# Machine-Learning Models

The following ensemble regression models were implemented and compared:
	•	Gradient Boosting Regressor
	•	Histogram-Based Gradient Boosting Regressor
	•	Random Forest Regressor
	•	Extra Trees Regressor

All models were trained under identical experimental conditions to ensure fair comparison.


# Key Results
	•	Boosting-based models achieved the strongest performance
	•	Gradient Boosting and Histogram-Based Gradient Boosting achieved R² ≈ 0.97
	•	Feature importance analysis identified customs clearance time, port congestion, traffic intensity, and weather severity as key drivers of delivery delay
