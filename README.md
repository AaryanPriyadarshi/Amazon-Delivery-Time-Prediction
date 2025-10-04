# Amazon Delivery Time Prediction

##### **Project Type**    - EDA / Regression / Forecasting  
##### **Domain**          - E-Commerce & Logistics  
##### **Tech Stack**      - Python, Pandas, NumPy, Matplotlib, Seaborn, Plotly, Scikit-Learn, XGBoost, SHAP  
##### **Key Skills**      - Data Cleaning, Feature Engineering, EDA, Regression Modeling, Model Evaluation, Explainability, Hypothesis Testing  

---

## Project Summary

This project focuses on predicting **Amazon delivery times** using machine learning to improve logistics efficiency and customer satisfaction.  
The dataset contains key operational parameters such as **traffic conditions, weather, distance, vehicle type, and agent performance metrics**.  

After cleaning and validating the data, several engineered features were added — including **distance between store and customer (via the Haversine formula)** and **time-based variables** like month, weekday, and order hour.  
Exploratory Data Analysis (EDA) revealed strong relationships between **distance, traffic intensity, and delivery time**, which were further validated using **hypothesis testing**.  

Machine learning models — including **Random Forest Regressor** and **XGBoost Regressor** — were implemented and evaluated using RMSE, MAE, and R² scores.  
Among these, **XGBoost** delivered the best performance, demonstrating its ability to capture non-linear patterns effectively.  

Finally, feature importance and SHAP analysis provided valuable interpretability, identifying **distance, traffic conditions, and agent ratings** as the most influential factors.  
This end-to-end solution not only predicts delivery duration accurately but also provides **data-driven insights for route optimization and workforce planning** in e-commerce logistics.

---

## Problem Statement

Accurately predicting delivery time is a critical challenge in e-commerce logistics.  
Factors such as **traffic congestion, weather variations, route distance, and delivery agent performance** contribute to unpredictable delivery durations.  

The problem this project addresses is:  
> **“How can we use data-driven modeling to accurately predict delivery times and identify the operational factors that most affect them?”**

By building predictive models and analyzing the underlying drivers of delivery delays, this project aims to help Amazon and similar companies **optimize delivery schedules**, **allocate resources efficiently**, and **enhance the customer experience** through reliable delivery time estimates.

---

## Workflow

1. **Import Libraries** – Setup environment with data science and visualization packages.  
2. **Dataset Loading** – Mount Google Drive and load the dataset into Colab.  
3. **Data Exploration** – Inspect data, handle missing values, and remove duplicates.  
4. **Feature Engineering** – Add distance, time, and interaction features for richer modeling.  
5. **EDA & Visualization** – Understand data trends with Seaborn and Plotly.  
6. **Hypothesis Testing** – Validate assumptions statistically.  
7. **Preprocessing** – Encode, scale, and split data into training/testing sets.  
8. **Model Implementation** – Train Random Forest and XGBoost regressors.  
9. **Model Evaluation** – Compare metrics (RMSE, MAE, R²) for performance assessment.  
10. **Feature Importance** – Use SHAP for model explainability.  
11. **Conclusion** – Interpret results and discuss improvements.

---

## Results

| Model              | RMSE  | MAE   | R²    |
|--------------------|-------|-------|-------|
| Random Forest      | —     | —     | —     |
| XGBoost Regressor  | Best  | —     | —     |

---

## Key Insights

- **Distance** and **Traffic conditions** are the strongest predictors of delivery time.  
- **Weekends** and **adverse weather** slightly increase delivery durations.  
- **Agent rating** shows measurable influence on overall delivery performance.  

---

## Future Improvements

- Integrate **real-time traffic and weather APIs** for live predictions.  
- Apply **Bayesian optimization** for hyperparameter tuning.  
- Deploy model using **Streamlit** or **Flask** for real-world use.  
- Extend model to include **delivery route optimization**.

---

## How to Run

1. Open the notebook in **Google Colab**.  
2. Mount your Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
3. Update dataset path inside the notebook:
   ```python
   DATA_PATH = "/content/drive/MyDrive/Amazon Delivery Project/amazon_delivery.csv"
4. Run all cells sequentially.

Dependancies:
   pip install pandas numpy matplotlib seaborn plotly scikit-learn xgboost shap

## Conclusion

This project demonstrates how data science and machine learning can be applied to real-world logistics to improve decision-making.
By predicting delivery times accurately and understanding influencing factors, companies can streamline operations, enhance customer experience, and reduce delays effectively.


