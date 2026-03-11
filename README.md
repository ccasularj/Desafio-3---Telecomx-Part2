# 📊 Telecom X – Churn Analysis and Prediction

## 📌 Project Overview

Customer churn is a major challenge for subscription-based companies. Understanding why customers leave is essential to create effective retention strategies.

This project analyzes customer data from **Telecom X** to identify factors related to **customer churn** and build **machine learning models** capable of predicting which customers are more likely to cancel their services.

The project includes:

- Data cleaning and preparation
- Exploratory Data Analysis (EDA)
- Correlation analysis
- Predictive modeling
- Business insights and recommendations

---

# 🗂 Dataset

The dataset contains information about Telecom X customers, including:

- Customer demographics
- Contract type
- Services subscribed
- Payment methods
- Tenure (time as a customer)
- Monthly and total charges
- Churn status

The data used in this project was previously **cleaned and standardized in Part 1 of the challenge**, and exported as a CSV file.

---

# 🔧 Project Steps

## 1️⃣ Data Preparation

The following steps were performed:

- Loading the cleaned dataset
- Removing irrelevant columns (such as `customerID`)
- Encoding categorical variables using **One-Hot Encoding**
- Checking class balance for the **Churn** variable

---

# 📊 Exploratory Data Analysis (EDA)

Several analyses were conducted to understand customer behavior.

## Churn Distribution

We analyzed the proportion of customers who:

- Stayed with the company
- Cancelled their services

This helps identify whether the dataset is balanced or imbalanced.

---

## Churn by Categorical Variables

We explored how churn varies across categorical variables such as:

- Contract type
- Payment method
- Internet service
- Additional services

These analyses help identify **customer profiles with higher churn probability**.

---

## Churn by Numerical Variables

We also analyzed numerical variables such as:

- **Tenure (customer lifetime)**
- **Total charges**

Boxplots and scatter plots were used to compare customers who churned and those who remained.

---

# 🔍 Correlation Analysis

A **correlation matrix** was used to identify relationships between variables.

Special attention was given to variables that showed higher correlation with churn, as they may be important predictors for machine learning models.

Key relationships analyzed include:

- **Tenure vs Churn**
- **Total Charges vs Churn**

---

# 🤖 Predictive Modeling

The dataset was split into:

- **Training set:** 80%
- **Test set:** 20%

Two machine learning models were developed.

---

## 📈 Logistic Regression

Logistic Regression is a linear model commonly used for binary classification.

Because it is sensitive to feature scale, **data normalization (StandardScaler)** was applied.

---

## 🌳 Random Forest

Random Forest is an ensemble method based on multiple decision trees.

Advantages:

- Handles non-linear relationships
- Less sensitive to scaling
- Provides feature importance

---

# 📊 Model Evaluation

Models were evaluated using the following metrics:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

These metrics help evaluate not only overall accuracy but also the ability to correctly identify customers who will churn.

---

# 🔑 Key Insights

The analysis revealed important churn patterns:

- Customers with **shorter tenure** are more likely to churn
- **Month-to-month contracts** show higher churn rates
- Customers with **lower total charges** tend to cancel more frequently
- Certain **payment methods** are associated with higher churn

---

# 💡 Business Recommendations

Based on the analysis, the following strategies may help reduce churn:

- Encourage customers to adopt **long-term contracts**
- Create **loyalty programs for new customers**
- Offer **discounts or benefits for annual plans**
- Identify high-risk customers early and apply **retention strategies**

---

# 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

# 📁 Project Structure

```
telecom-churn-analysis
│
├── data
│   └── telecom_churn_clean.csv
│
├── notebooks
│   └── telecom_churn_analysis.ipynb
│
├── README.md
```

---

# 📈 Future Improvements

Possible improvements for future work:

- Hyperparameter tuning
- Testing additional models (XGBoost, Gradient Boosting)
- Handling class imbalance techniques
- Building a churn prediction dashboard

---

# 📚 Author

Developed as part of a **Data Science Challenge focused on churn analysis and machine learning modeling**.
