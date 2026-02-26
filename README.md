# 🚀 Revenue Leakage Risk Prediction — ML Project

## 📌 Overview

This project builds a Machine Learning model to predict **revenue leakage risk** in e-commerce orders using the Olist dataset (Brazilian e-commerce data).

Revenue leakage can occur due to delays, cancellations, high logistics costs, payment issues, or customer dissatisfaction.

The goal is to proactively identify high-risk orders so businesses can take preventive action.

---

## 📊 Dataset

**Source:** Olist E-commerce Dataset (Kaggle)

The dataset contains real transactional data including:

* Orders
* Customers
* Sellers
* Payments
* Reviews
* Products
* Logistics information

---

## 🧠 Problem Statement

Predict whether an order is at risk of causing revenue leakage based on operational and behavioral signals.

Target Variable:

**leakage_risk**

* 0 → Low risk
* 1 → High risk

---

## ⚙️ Project Pipeline

### 1️⃣ Data Cleaning

* Removed duplicates
* Handled missing values
* Converted timestamps
* Filtered useful columns

### 2️⃣ Data Integration

Merged multiple tables into one order-level dataset:

* Orders
* Customers
* Order Items
* Payments
* Reviews
* Sellers
* Products

Final dataset → **1 row = 1 order**

---

### 3️⃣ Feature Engineering

Created business-relevant features such as:

* Delivery time
* Delay vs estimated delivery
* Total order value
* Freight ratio
* Number of items & sellers
* Payment behavior
* Customer region
* Review score
* Cancellation / non-delivery flags

---

### 4️⃣ Target Creation

Defined revenue leakage risk using:

* Late deliveries
* High shipping cost
* Low ratings
* Cancellations
* Payment patterns

---

### 5️⃣ Modeling

Trained multiple models:

* Logistic Regression
* Random Forest ⭐
* Gradient Boosting

---

### 6️⃣ Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

---

### 7️⃣ Key Insights (Feature Importance)

Top drivers of revenue leakage risk:

* High number of payment installments
* Low review scores
* High freight ratio
* Delivery delays
* Order value patterns
* Late delivery indicators

---

## 📈 Results

Tree-based models achieved near-perfect performance due to strong predictive features engineered from operational data.

---

## 🛠️ Tech Stack

* Python
* Pandas & NumPy
* Scikit-learn
* Matplotlib & Seaborn
* Jupyter Notebook

---

## 🎯 Business Impact

This model can help e-commerce companies:

✔ Identify risky orders early
✔ Reduce cancellations and losses
✔ Improve logistics planning
✔ Enhance customer satisfaction
✔ Optimize pricing & shipping strategies

---

## 👩‍💻 Author

**Veda Shree S**
AIML Student — BMSIT&M

---

## ⭐ If you found this useful, please star the repository!
