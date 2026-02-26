# Revenue Leakage Risk Prediction

## Project Overview

This project builds a machine learning model to predict whether an e-commerce order is likely to result in revenue leakage.

Revenue leakage can happen due to delayed deliveries, cancellations, high shipping costs, or poor customer experience. The aim is to identify risky orders in advance so businesses can take corrective actions.

---

## Dataset

Olist Brazilian E-commerce Dataset (Kaggle)

It contains real order data including:

* Orders
* Customers
* Sellers
* Products
* Payments
* Reviews
* Delivery information

All tables were merged to create one dataset where each row represents a single order.

---

## Problem Statement

Predict a binary target:

**leakage_risk**

* 0 → Low risk
* 1 → High risk

The label was created using business rules based on delays, cancellations, freight cost, and review scores.

---

## Steps Followed

### Data Cleaning

* Removed duplicate records
* Handled missing values
* Converted date columns
* Selected relevant columns

### Data Integration

Multiple datasets were joined using keys like order_id, customer_id, and product_id.

### Feature Engineering

Created useful business features such as:

* Delivery time
* Delay compared to estimate
* Total order value
* Freight ratio (shipping cost vs product cost)
* Number of items in order
* Payment installments
* Customer region
* Review score
* Late delivery and non-delivery flags

### Modeling

Trained and compared:

* Logistic Regression
* Random Forest
* Gradient Boosting

### Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

Tree-based models performed best.

---

## Key Insights

Important factors influencing leakage risk include:

* Payment installment patterns
* Customer ratings
* High shipping cost relative to order value
* Delivery delays
* Order value

---

## Tools Used

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn
* Jupyter Notebook

---

## Author

Veda Shree S
B.Tech AIML — BMSIT&M
