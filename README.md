# 🧠 Stock Market Forecasting Using Advanced Machine Learning Models  
**Barry University — Research by Aftab Alam Masjidi**

---

## 🧩 Abstract  
This research explores the use of machine learning and neural architectures to forecast short-term stock price movements by leveraging **representation learning**, **temporal dependencies**, and **uncertainty quantification**.  
By systematically comparing classical and ensemble regressors with deep neural models (MLP, RNN), the project demonstrates how predictive intelligence can extract stable signals from noisy data.  
The study establishes a methodological foundation for applying similar predictive frameworks to **cyber threat forecasting**, aligning with MBZUAI’s mission to advance trustworthy and human-centric AI systems.

---

## 📘 Overview  
The repository evaluates the effectiveness of **supervised regression algorithms** in modeling dynamic and volatile time-series data.  
Ten algorithms were benchmarked across metrics of stability, interpretability, and drift-awareness to assess their suitability for adaptive prediction tasks.

**Models Implemented:**  
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

The experiments were conducted on **Google (GOOG)** stock data, incorporating advanced feature engineering, multi-horizon evaluation, and representation-aware tuning to identify models that balance generalization and explainability.

---

## ⚙️ Methodology & Feature Engineering  
- Designed **lag-based temporal embeddings** (1- and 2-day shifts) to capture sequential dependencies.  
- Computed **rolling and exponential moving averages** to model momentum across multiple time scales.  
- Introduced **volatility and dispersion indicators** such as *High–Low Range* and *Volume Volatility* for signal strength.  
- Performed **hyperparameter optimization** with `GridSearchCV` and **cross-validated drift detection**.  
- Standardized data with **feature normalization** for balanced training and faster convergence.  
- Implemented prototype neural architectures — **Multi-Layer Perceptron (MLP)** and **Recurrent Neural Networks (RNN)** — to analyze non-linear and temporal relationships.  

These steps provided a multi-layered perspective on how **feature representation and uncertainty calibration** impact predictive robustness.

---

## 📊 Results & Insights  
- **Ridge Regression** achieved the most consistent and interpretable performance on smaller datasets (~200 samples), maintaining robustness under regularization.  
- Simpler models outperformed complex ensembles (e.g., XGBoost) in low-data regimes, reaffirming the trade-off between bias, variance, and interpretability.  
- After fine-tuning, Ridge Regression achieved **R² ≈ 1.000** and near-zero **MSE** across all financial attributes (*Open, High, Low, Close, Volume*).  
- The study highlights how **model simplicity, calibrated uncertainty, and representation stability** enable reliable predictions in non-stationary environments.

---

## 📈 Visualization & Evaluation  
- Interactive **Plotly** dashboards visualize actual vs predicted values.  
- Comparative plots display **MSE**, **R²**, and **feature importance** distributions for interpretability.  
- All model metrics are stored in reproducible `.CSV` logs for transparency and evaluation tracking.

*(Sample visualization below)*  
![Workflow Diagram](Actual%20Vs%20Predicted.jpeg)

---

## 🚀 Next Steps  
- Scale experiments to **multi-sector financial datasets** (S&P 500, NASDAQ).  
- Integrate **Transformer-based temporal encoders** and **Graph Neural Networks (GNNs)** to enhance relational and sequential learning.  
- Extend cross-domain transfer to **predictive cybersecurity**, applying identical learning principles to model **threat drift**, **anomaly detection**, and **behavioral forecasting** in cyber telemetry.  
- Evaluate **explainable AI (XAI)** techniques to strengthen interpretability and human-trust in predictive defense systems.

---

## 💻 Tech Stack  
Python · Pandas · NumPy · Scikit-learn · XGBoost · TensorFlow · Matplotlib · Plotly  

---

## 👨‍💻 Author  
**Aftab Alam Masjidi**  
Senior Stamps Scholar · Barry University  
📧 [Contact via LinkedIn](https://www.linkedin.com/in/aftabalammasjidi)  
📅 Ongoing Research (2025)

---

## 🧾 License  
This project is licensed under the [MIT License](LICENSE).
