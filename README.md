# 🚗 Car Insurance Subscription Prediction - Mini Project

This is a simple yet insightful machine learning mini-project focused on predicting whether a customer will subscribe to a car insurance product based on demographic, financial, and contact history features.

---

## 📌 Project Overview

**Goal:**  
Predict the likelihood of a customer subscribing to car insurance (`CarInsurance = 1` or `0`) using logistic regression, and interpret key influencing features.

This project is designed for educational purposes as part of a Data Science Bootcamp and demonstrates a streamlined machine learning workflow.

---

## 🧾 Dataset Description

The dataset contains customer information and interaction history, including:

- **Demographics:** `Age`, `Job`, `Marital`, `Education`
- **Financial Info:** `Balance`, `Default`, `HHInsurance`, `CarLoan`
- **Contact History:** `Communication`, `LastContactDay`, `LastContactMonth`, `NoOfContacts`, `DaysPassed`, `PrevAttempts`
- **Target Variable:** `CarInsurance` (1 = subscribed, 0 = not subscribed)

Missing values are present in several categorical columns, such as `Job`, `Education`, and `Communication`.

---

## 🧠 Methodology

1. **Data Preprocessing**
   - Dropped irrelevant columns: `Id`, `CallStart`, `CallEnd`, `Outcome`
   - Handled missing values by replacing with `'unknown'`
   - One-hot encoded categorical variables
   - Standardized numerical features

2. **Modeling**
   - Trained a **Logistic Regression** model on the processed training data
   - Evaluated using **accuracy**, **precision**, **recall**, and **F1-score**

3. **Interpretability**
   - Analyzed **feature importance** to identify key drivers of subscription

4. **Prediction**
   - Generated predictions on a test dataset
   - Saved predictions to `carInsurance_predictions.csv`

---

## 📊 Key Insights

- Job type, education level, and communication method had a strong influence on insurance subscription likelihood.
- Financial balance and number of previous contacts were also significant predictors.

---
