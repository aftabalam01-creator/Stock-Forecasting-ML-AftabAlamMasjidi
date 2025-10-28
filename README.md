# Stock Market Forecasting Using Advanced Machine Learning Models  
**Barry University — Research by Aftab Alam Masjidi**

---

## Project Overview
This repository explores how machine learning can forecast stock market trends using both classical and ensemble regression models.  
The research compares 10 AI algorithms to identify which performs best under different data conditions.

Models used:
- Linear Regression  
- Ridge Regression  
- Lasso Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- Gradient Boosting Regressor  
- AdaBoost Regressor  
- Extra Trees Regressor  
- K-Nearest Neighbors (KNN)  
- XGBoost Regressor  

The current experiments focus on **Google (GOOG) stock data**, performing feature engineering, parameter tuning, and time-based evaluation to identify predictive efficiency.

---

## Methods & Feature Engineering
- Added **lagged features** (1-day and 2-day shifts) for all numerical columns.  
- Computed **rolling averages**, **exponential moving averages**, and **volatility indicators**.  
- Engineered features like *High–Low Range* and *Volume Volatility* for trend strength detection.  
- Optimized **hyperparameters** using `GridSearchCV` for model tuning.  
- Scaled data using `StandardScaler` to ensure balanced learning.

---

## Key Findings
- **Ridge Regression** produced the most stable and accurate results on smaller datasets (~200 rows).  
- The model’s regularization helped prevent overfitting, outperforming other complex models like XGBoost.  
- After feature tuning, the model achieved **R² ≈ 1.000** and near-zero MSE across all price columns.

---

## Visualizations
- Interactive Plotly charts compare actual vs predicted values for Open, High, Low, Close, and Volume.  
- Each model’s performance metrics (MSE and R²) are logged and exported as CSV for reproducibility.  

*(Sample visualization below)*  
![Workflow Diagram](A_flowchart_diagram_illustrates_stock_market_forec.png)

---

## Next Steps
- Apply models on **larger financial datasets** (e.g., S&P 500, NASDAQ).  
- Integrate **Natural Language Processing (NLP)** for sentiment-aware forecasting.  
- Analyze how textual signals (financial news, tweets, and headlines) affect model performance.

---

## Tech Stack
Python · Pandas · NumPy · Scikit-learn · XGBoost · Matplotlib · Plotly

---

## uthor
**Aftab Alam Masjidi**  
Senior Stamps Scholar · Barry University  
📧 [Contact via LinkedIn](https://www.linkedin.com/in/aftabalammasjidi)  
📅 Ongoing Research (2025)

---

## License
This project is licensed under the [MIT License](LICENSE).

