# Data-Science-Analytics-Internship-Phase-II
Advanced Data Science internship projects covering classification with SHAP explainability, K-Means customer segmentation, XGBoost time series forecasting, and loan default risk modeling with business cost optimization. Built with Python in Google Colab.
This repository contains my work for the Advanced Internship Tasks assigned by DevelopersHub Corporation. Out of the 5 tasks, I completed 4 — covering classification with explainability, customer segmentation, time series forecasting, and risk modeling with business cost optimization.
All notebooks were developed in Google Colab using Python.

📂 Tasks Overview
TaskTitleType01Term Deposit Subscription PredictionClassification + XAI02Customer SegmentationUnsupervised Learning03Energy Consumption ForecastingTime Series04Loan Default Risk + Cost OptimizationRisk Modeling

✅ Task 01 — Term Deposit Subscription Prediction
📊 Dataset: Bank Marketing Dataset (UCI ML Repository)
The goal was to predict whether a customer would subscribe to a term deposit after a marketing call. I trained two models — Logistic Regression as a baseline and Random Forest for better performance — and compared them using a classification report and ROC curve.
The more interesting part was using SHAP to explain individual predictions. Instead of just knowing that the model predicted yes or no, SHAP showed why — which features pushed the prediction in which direction. Random Forest outperformed Logistic Regression by capturing non-linear patterns in the data.
🛠️ Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn, shap

✅ Task 02 — Customer Segmentation Using K-Means
📊 Dataset: Mall Customers Dataset
This task was about grouping customers based on Annual Income and Spending Score. I used the Elbow Method to find the optimal number of clusters (5), applied K-Means, and then used PCA to visualize the clusters in 2D.
Each cluster had a distinct behavioral profile, which I mapped to a marketing strategy:

💰 High Income, High Spending → premium products and loyalty programs
📈 High Income, Low Spending → upselling campaigns
⚠️ Low Income, High Spending → careful targeting, risk of over-spending
🏷️ Low Income, Low Spending → budget offers and discounts
🎯 Average profile → regular engagement and retention offers

🛠️ Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

✅ Task 03 — Energy Consumption Forecasting
📊 Dataset: PJME Hourly Energy Consumption Dataset
The task was to forecast energy usage using historical time-based data. I parsed the datetime index, then engineered features from it — hour of day, day of week, and month — and trained an XGBoost model on the first 80% of the data, testing on the remaining 20%.
Performance was evaluated using MAE and RMSE, and actual vs. predicted consumption was plotted side by side. A peak hour analysis also confirmed that energy usage spikes at predictable times during the day, which can help energy providers with demand planning.
🛠️ Libraries: pandas, numpy, xgboost, scikit-learn, matplotlib

✅ Task 04 — Loan Default Risk with Business Cost Optimization
📊 Dataset: Home Credit Default Risk Dataset
Standard default prediction using Logistic Regression — but the interesting part was the cost optimization step. Instead of treating all prediction errors equally, I assigned actual financial costs:

🔴 False Positive (approving a risky customer) → Rs. 10,000 loss
🟡 False Negative (rejecting a good customer) → Rs. 2,000 opportunity loss

Using these values, I calculated the total business cost at the default 0.5 threshold, then swept thresholds from 0.1 to 0.9 to find the point that minimized total cost. This shows that model performance and business impact are not the same thing — and the threshold matters a lot depending on what type of error you can afford.
🛠️ Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

⚙️ Stack
Python · Pandas · NumPy · Scikit-learn · XGBoost · SHAP · Matplotlib · Seaborn · Google Colab

🚀 How to Run
Open any .ipynb file in Google Colab, upload the required dataset when prompted, and run all cells. All libraries are pre-installed in Colab.

Muhammad Hasan
Data Science & Analytics Intern — DevelopersHub Corporation
