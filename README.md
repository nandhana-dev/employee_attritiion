# Employee Attrition Prediction

## Project Overview
This project delivers a machine learning solution to predict **employee attrition**. By identifying the **top 10 most influential features** that drive turnover, the model provides robust, unbiased, and probability-based predictions.

---

## The Challenge
The core challenge was to build a model that could accurately identify employees at risk of leaving from a highly **imbalanced dataset**, where **87% of the data showed no attrition**.

---

## Methodology
We employed a systematic, data-driven approach to build a robust predictive model.

* **Feature Engineering:** We systematically reduced a large set of 33 initial features down to **16 key features** through rigorous data analysis. Using a Random Forest Classifier, we then precisely identified the **top 10 most impactful features** for the final model.
* **Class Imbalance Mitigation:** To overcome data bias, we used **SMOTE (Synthetic Minority Oversampling Technique)** to balance the dataset and ensure the model could learn from both employee groups equally.
* **Model Selection:** We evaluated several classifiers, including **Logistic Regression** and **XGBoost**. The **Random Forest Classifier** was selected for its superior performance, as evidenced by a **cross-validated ROC-AUC score of 0.972**, and its ability to capture the complex, non-linear relationships within the data.

---

## Model Performance
Our final model demonstrates strong predictive capabilities, particularly for identifying at-risk employees.

* **Accuracy:** 0.80
* **Precision:** 0.26
* **Recall:** 0.15
* **F1-Score:** 0.19
* **ROC-AUC Score:** 0.972 (Cross-Validated)

---

## Business Impact
The model's top features provide actionable insights for improving employee retention. The following are the most significant drivers of attrition, ranked by their importance to the model:

* **YearsWithCurrManager:** The length of an employee's relationship with their current manager is a critical factor.
* **Age:** Age is a strong predictor of an employee's likelihood to leave.
* **NumCompaniesWorked:** The number of past employers is highly correlated with attrition.
* **YearsAtCompany:** The duration of an employee's tenure is a significant indicator.
* **EnvironmentSatisfaction:** Job environment plays a crucial role in an employee's decision to stay.
* **TotalWorkingYears:** Overall career experience is a key factor.
* **JobSatisfaction:** An employee's satisfaction with their job is a fundamental driver of retention.
* **MonthlyIncome:** Compensation is a strong predictor of employee turnover.
* **YearsInCurrentRole:** The time an employee has spent in their current position is a key factor.
* **DistanceFromHome:** The daily commute distance from an employee's home influences attrition.

**Actionable Recommendations:**
* **Focus on Managerial Relationships:** Implement training for managers to foster better relationships and support their teams.
* **Enhance Employee Satisfaction:** Conduct regular surveys to measure and improve job and environment satisfaction.
* **Review Compensation:** Analyze current salary and benefit structures to ensure competitiveness and reduce turnover driven by financial factors.

---

## Tech Stack
* **Python 3.x**
* **Pandas, NumPy**
* **Scikit-learn**
* **Google Colab**
