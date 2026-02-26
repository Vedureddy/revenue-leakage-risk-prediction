# Revenue Leakage Risk Prediction (E-commerce)

This project builds a machine learning model to predict the risk of revenue leakage in e-commerce orders using operational, pricing, delivery, and customer behavior data.

Revenue leakage can occur due to delayed deliveries, cancellations, high logistics cost, payment patterns, or poor customer experience. Identifying high-risk orders helps businesses take preventive actions and reduce losses.

---

## Problem Statement

E-commerce platforms handle thousands of orders daily. Some orders lead to financial loss due to:

* Delivery delays
* High shipping cost relative to product value
* Order cancellations or failures
* Low customer satisfaction
* Risky payment behavior

The goal is to predict whether an order is likely to result in revenue leakage.

---

## Dataset

This project uses the **Olist Brazilian E-commerce Dataset** from Kaggle.

🔗 https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

The dataset contains information about:

* Orders
* Customers
* Sellers
* Products
* Payments
* Reviews
* Delivery timelines

Raw CSV files are not included due to GitHub size limits.

---

## Project Workflow

### 1. Data Understanding

* Explored multiple relational tables
* Identified keys and relationships
* Examined missing values and duplicates

### 2. Data Cleaning

* Removed duplicates
* Handled missing values
* Converted timestamps
* Selected useful columns

### 3. Data Integration

* Aggregated multi-row tables to order level
* Merged all datasets into a single table
* Each row represents one order

### 4. Feature Engineering

Created business-relevant features such as:

* Delivery duration
* Delay vs estimated delivery
* Total order value
* Freight ratio
* Number of items and sellers
* Payment characteristics
* Customer region
* Review score
* Cancellation indicators

### 5. Target Creation

Defined a custom **Revenue Leakage Risk** label based on:

* Late delivery
* High shipping cost
* Low customer rating
* Undelivered or cancelled orders

### 6. Model Training

The following models were trained:

* Logistic Regression
* Random Forest
* Gradient Boosting

### 7. Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

### 8. Insights & Drivers

Feature importance analysis identified key drivers of revenue leakage risk.

---

## Key Findings

The most influential factors affecting leakage risk include:

* Number of payment installments
* Customer review score
* Freight cost relative to product value
* Delivery delays
* Order value
* Payment behavior

---

## Technologies Used

* Python
* Pandas & NumPy
* Scikit-learn
* Matplotlib & Seaborn
* Jupyter Notebook

---

## How to Run

1. Download the dataset from Kaggle
2. Place the CSV files in the project folder
3. Open the notebook (`ML Project.ipynb`)
4. Run all cells sequentially

---

## Future Improvements

* Hyperparameter tuning
* Cross-validation
* Real-time risk scoring
* Deployment as a web application
* Integration with business dashboards

---

## Author

Veda Shree S
Junior Data Analyst

---

## License

This project is for educational and research purposes only.
