# 🧠 Data Science & Analytics Internship – Advanced Tasks
**DevelopersHub Corporation**

This repository contains 4 out of 5 advanced tasks completed as part of the **Data Science & Analytics Internship at DevelopersHub Corporation**. Each task covers an advanced area of data science including explainable AI, unsupervised learning, time series forecasting, and risk modeling with business cost optimization using Python.

---

## ✅ Tasks Overview

---

### 📌 Task 1 — Term Deposit Subscription Prediction

| **Dataset** | Bank Marketing Dataset (UCI Machine Learning Repository) |
|---|---|
| **Objective** | Predict whether a bank customer will subscribe to a term deposit as a result of a marketing campaign |

**Approach:**
* Loaded and explored the dataset using `.info()`, `.describe()`, and `.value_counts()`
* Visualized key features: age distribution, job type, and contact method vs. subscription outcome
* Encoded all categorical features using **Label Encoding**
* Trained two classification models — **Logistic Regression** (baseline) and **Random Forest**
* Evaluated using **Confusion Matrix**, **F1-Score**, and **ROC Curve**
* Applied **SHAP** values to explain individual model predictions *(Explainable AI — XAI)*

**Key Libraries:** `pandas` `numpy` `scikit-learn` `matplotlib` `seaborn` `shap`

---

### 📌 Task 2 — Customer Segmentation Using Unsupervised Learning

| **Dataset** | Mall Customers Dataset |
|---|---|
| **Objective** | Cluster customers based on spending habits and propose tailored marketing strategies for each segment |

**Approach:**
* Conducted full **EDA** — explored income vs. spending score and gender distribution
* Scaled features using **StandardScaler** to ensure equal contribution to clustering
* Used the **Elbow Method** to determine the optimal number of clusters *(K = 5)*
* Applied **K-Means Clustering** to segment customers into 5 distinct groups
* Used **PCA** to reduce dimensions and visualize clusters in 2D
* Proposed data-driven **marketing strategies** for each cluster:

| **Cluster** | **Profile** | **Strategy** |
|---|---|---|
| 0 | High Income, High Spending | Premium products & loyalty programs |
| 1 | Low Income, Low Spending | Discounts & budget-friendly offers |
| 2 | High Income, Low Spending | Upselling through targeted campaigns |
| 3 | Low Income, High Spending | Careful targeting — high risk segment |
| 4 | Average Customers | Regular engagement & retention offers |

**Key Libraries:** `pandas` `numpy` `scikit-learn` `matplotlib` `seaborn`

---

### 📌 Task 3 — Energy Consumption Forecasting

| **Dataset** | PJME Hourly Energy Consumption Dataset |
|---|---|
| **Objective** | Forecast short-term energy usage using historical time-based patterns |

**Approach:**
* Parsed datetime index and set it as the time series reference
* Engineered time-based features: **hour of day**, **day of week**, and **month**
* Split data chronologically — 80% training, 20% testing
* Trained an **XGBoost Regressor** to predict energy consumption
* Evaluated model performance using **MAE** and **RMSE**
* Plotted **actual vs. predicted** energy usage for visual comparison
* Conducted **Peak Hour Analysis** to identify highest demand periods

**Evaluation Metrics:**

| **Metric** | **Description** |
|---|---|
| MAE | Mean Absolute Error — average prediction error |
| RMSE | Root Mean Squared Error — penalizes larger errors more heavily |

**Key Libraries:** `pandas` `numpy` `xgboost` `scikit-learn` `matplotlib`

---

### 📌 Task 4 — Loan Default Risk with Business Cost Optimization

| **Dataset** | Home Credit Default Risk Dataset |
|---|---|
| **Objective** | Predict loan default likelihood and optimize the decision threshold based on cost-benefit analysis |

**Approach:**
* Cleaned dataset by filling missing values with **column medians**
* Encoded categorical features using **Label Encoding**
* Trained a **Logistic Regression** model for binary default classification
* Visualized results using a **Confusion Matrix** heatmap
* Defined real financial costs for each type of prediction error:

| **Error Type** | **Scenario** | **Cost** |
|---|---|---|
| False Positive | Approving a risky customer | Rs. 10,000 loss |
| False Negative | Rejecting a good customer | Rs. 2,000 opportunity loss |

* Swept decision thresholds from **0.1 to 0.9** to find the optimal cutoff that minimizes total business cost

**Key Libraries:** `pandas` `numpy` `scikit-learn` `matplotlib` `seaborn`

---

## 🛠️ Technologies Used

| **Tool** | **Purpose** |
|---|---|
| Python 3.x | Core programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computations |
| Matplotlib & Seaborn | Data visualization |
| Scikit-learn | Machine learning models and evaluation |
| XGBoost | Gradient boosting for time series forecasting |
| SHAP | Explainable AI — model interpretability |
| Google Colab | Cloud-based development environment |

---

## 🚀 How to Run

All notebooks were developed using **Google Colab**. To run them:

1. Open **Google Colab**
2. Click **File → Upload Notebook** and select any `.ipynb` file
3. Upload the required dataset when prompted
4. Click **Runtime → Run All**

✅ All required libraries come pre-installed in Google Colab — no additional setup needed.

---

## 👤 Author

**Muhammad Hasan**
Data Science & Analytics Intern — DevelopersHub Corporation

This repository was created as part of a structured internship program to build advanced, practical data science skills.
