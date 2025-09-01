# Employee Attrition Prediction

## Project Overview
This project presents an intelligent machine learning model designed to predict **employee attrition**. By meticulously analyzing a complex, imbalanced dataset, the model identifies the **top 10 most influential features** that determine whether an employee will stay or leave, providing a robust, unbiased prediction.

---

## The Challenge
Working with real-world data is rarely simple. Our dataset presented a significant challenge: it was highly **imbalanced**, with 87% of employees showing no signs of attrition. This high bias could lead to a model that simply predicts "stay" every time, making it useless in practice.

The project's core challenge was to build a predictive model that could overcome this bias and accurately identify the small group of employees who might leave.

---

## Data Analysis & Feature Selection
Our analysis was a two-stage process to ensure the final model was both powerful and focused.

1.  **Initial Analysis:** We began by exploring a wide array of variables and performed a deep analysis to filter them down to **16 key features** that showed the strongest correlation with attrition. This involved extensive data study to understand what factors truly matter.
2.  **Model-Based Refinement:** We then used a **Random Forest Classifier** to dig deeper. By leveraging its feature importance capabilities, we precisely identified the **top 10 features** from our initial set that have the highest impact on an employee's decision to leave.

---

## The Solution: Building an Unbiased Model
To solve the data bias problem, we employed advanced techniques to ensure our model would not be misled by the imbalanced data.

- **SMOTE (Synthetic Minority Oversampling Technique):** We used SMOTE to create synthetic data points for the minority class (employees who left). This balanced the dataset, allowing our model to learn the patterns of both groups equally.
- **Standard Classifiers:** We built and tuned standard machine learning classifiers, trained on the balanced dataset, to accurately predict the **probability of an employee leaving or staying**.

---

## Key Achievements
This project isn’t just about a final number; it’s about the process. We successfully demonstrated the ability to:
- **Critically analyze and select features** from a large dataset.
- **Overcome data bias** using advanced techniques like SMOTE.
- **Build an unbiased, accurate model** to predict a critical business outcome.

---

## Tech Stack
- **Python 3.x**
- **Pandas, NumPy**
- **Scikit-learn**
- **Google Colab**
