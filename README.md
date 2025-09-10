🚗 Waze Customer Churn Project

Predicting user churn in the Waze navigation app using machine learning.
Analyzes engagement metrics (sessions, drives, activity days) to identify churn predictors.
Builds and compares models (Logistic Regression, Decision Tree, Random Forest, XGBoost) to guide retention strategies.



📖 Project Overview

This project investigates user churn prediction in Waze. High churn, caused by declining engagement and inconsistent usage, threatens platform growth and user retention. The goal is to develop a predictive framework that identifies at-risk users and provides insights to guide retention strategies.
	•	Objective: Predict whether a Waze user will churn (leave/inactive) or remain retained.
	•	Dataset: ~15,000 anonymized user records
	•	Features: sessions, drives, activity_days, driven_km_drives, device (Android/iPhone).
	•	Target Variable: churned → 1 = churned, 0 = retained.



⚙️ Methodology

🏗️ Training Phase
	1.	Data Collection → Waze dataset of ~15k users.
	2.	Data Cleaning & Preparation → Handle missing labels, encode categorical variables, drop redundant columns.
	3.	EDA & Statistical Testing → Descriptive stats, correlation heatmaps, t-tests, chi-square tests.
	4.	Model Development → Logistic Regression, Decision Tree, Random Forest, XGBoost.
	5.	Model Evaluation → Accuracy, Precision, Recall, F1 Score, ROC-AUC, PR-AUC, Confusion Matrices.

🔮 Prediction Phase
	•	Preprocess new user data.
	•	Apply best-performing model (Logistic Regression).
	•	Generate churn risk score.
	•	Flag high-risk users for retention campaigns.



📊 Results
	•	Best Model: Logistic Regression (ROC-AUC = 0.763, best precision-recall balance).
	•	Key Predictors:
	•	activity_days (most important)
	•	sessions
	•	drives
	•	driven_km_drives
	•	Insights: Engagement frequency strongly reduces churn risk. Device type has only a modest effect compared to activity.



💡 Recommendations
	•	⚠️ Build an early warning system to flag disengaged users.
	•	📲 Run re-engagement campaigns (notifications, rewards, gamification).
	•	🚀 Strengthen onboarding by encouraging early usage and setting favorite destinations.
	•	🔁 Retrain models regularly with updated datasets to capture evolving behavior.



🛠️ Tech Stack
	•	Languages: Python 3
	•	Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost
	•	Visualization: Matplotlib, Seaborn
	•	Environment: Google Colab / Jupyter Notebook


🚀 How to Run
	1.	Clone the repository
 git clone https://github.com/VaanathyKajatheepan/waze-customer-churn-project
cd waze-churn-prediction

	2. Install dependencies
 pip install -r requirements.txt

 	3. Run Notebook
  Open the Jupyter Notebook or Google Colab file.
  Open the pbix file in Power BI
  Explore the analysis, visualizations, and churn prediction models.

	4. Access Agile Scrum Framework from Tiaga for the waze project
 https://tree.taiga.io/project/vaanathykajatheepan-waze-customer-churn/backlog
 

