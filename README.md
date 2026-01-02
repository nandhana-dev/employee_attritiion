# 📊 Employee Attrition Prediction

> **Predictive HR Analytics. SMOTE. Feature Importance.**
> A machine learning solution designed to identify high-risk attrition profiles and the key behavioral drivers behind employee turnover.

---

## 🎯 Project Overview
The primary challenge of this project was handling a significant **class imbalance (87% non-attrition)**. By implementing **SMOTE** and a **Random Forest** architecture, the model achieves a **ROC-AUC of 0.972**, providing highly reliable probability-based predictions for HR decision-making.



---

## 🛠️ Methodology & Technical Strategy

* **Class Imbalance Mitigation:** Utilized **SMOTE** (Synthetic Minority Oversampling Technique) to synthesize minority class samples, ensuring the model identifies "At-Risk" employees without bias.
* **Feature Optimization:** Reduced 33 raw variables to **16 refined features**, ultimately isolating the **Top 10 drivers** of turnover.
* **Algorithm Selection:** Benchmarked Logistic Regression and XGBoost; **Random Forest** was selected for its superior ability to capture non-linear relationships in HR data.

---

## 📈 Model Performance
| Metric | Score |
| :--- | :--- |
| **ROC-AUC (Cross-Validated)** | **0.972** |
| **Model Accuracy** | 0.80 |
| **Precision** | 0.26 |
| **Recall** | 0.15 |

---

## 💡 Top 10 Attrition Drivers
The model identified the following features as the most critical predictors of employee turnover:
1. **YearsWithCurrManager** (Managerial Relationship)
2. **Age** (Demographic Trends)
3. **NumCompaniesWorked** (Career Stability)
4. **YearsAtCompany** (Tenure)
5. **EnvironmentSatisfaction** (Work Culture)
6. **TotalWorkingYears** (Experience)
7. **JobSatisfaction** (Role Alignment)
8. **MonthlyIncome** (Compensation)
9. **YearsInCurrentRole** (Promotion Cycles)
10. **DistanceFromHome** (Commute Impact)


---

## 🛡️ License

**Copyright © 2025 Nandhana.** All rights reserved.  

Proprietary work. Unauthorized copying or distribution is prohibited. Inquiries: nandhanaprabhar231@gmail.com

---

## ⚙️ Technical Setup

### Prerequisites
* **Python 3.x**
* **Libraries:** `pandas`, `numpy`, `scikit-learn`, `imblearn`, `matplotlib`, `seaborn`

### Installation & Usage
```bash
# Clone the repository
git clone [https://github.com/nandhana-dev/employee-attrition.git](https://github.com/nandhana-dev/employee-attrition.git)
cd employee-attrition

# Install Dependencies
pip install pandas numpy scikit-learn imbalanced-learn matplotlib seaborn
```


## Running the Analysis 
1. Open the .ipynb file in Google Colab or Jupyter Notebook.

2. Ensure the dataset (Employee-Attrition.csv) is located in the root directory.
