# 🛒 Product Return Prediction System

A machine learning project that predicts whether a customer will return a product based on order, customer, and delivery data from a real e-commerce dataset (Olist Brazilian E-commerce Public Dataset).

---

## 📌 Problem Statement

In e-commerce, high return rates impact profitability and logistics. This project aims to build a predictive model that identifies high-risk return orders before they occur, helping businesses:

- Reduce costs from unnecessary shipments
- Improve inventory and supply chain efficiency
- Take proactive action like better packaging or delivery experience

---

## 📂 Dataset

**Source:** [Olist E-commerce Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) (Kaggle)  
**Files Used:**
- `olist_orders_dataset.csv`
- `olist_order_items_dataset.csv`
- `olist_products_dataset.csv`
- `olist_order_reviews_dataset.csv`

---

## 🧠 Target Variable: `is_returned`

> **1** → Returned  
> **0** → Not Returned

---

## 🏗️ Features Used

| Feature               | Description                                      |
|-----------------------|--------------------------------------------------|
| `delivery_days`       | Time taken (in days) to deliver the product      |
| `late_delivery`       | Whether the product was delivered late (1/0)     |
| `product_category`    | Category of the product                          |
| `product_weight_g`    | Weight of the product in grams                   |
| `freight_value`       | Delivery cost charged                            |
| `price`               | Sale price of the product                        |
| `payment_type`        | Type of payment method                           |
| `review_score`        | User's rating of the product (1–5)               |
| `customer_state`      | Geographic region of the customer                |

---

## 🧪 Modeling Approach

- Initial model: **Random Forest Classifier**
- Train-test split: 80/20
- Performance evaluated using:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
- Feature importance plotted to understand key drivers of returns

---

## 📊 Business Actions Based on Results

Use this model to predict return likelihood in future orders and take preventive steps:

- Show alerts to customers before checkout.

- Offer different packaging or extra product details.

- Flag high-risk orders for manual review.

---

## 🚀 Future Improvements

1. **Model Tuning & Cross-Validation**  
   Improve model generalization with GridSearchCV or RandomizedSearchCV.

2. **Try XGBoost / LightGBM Models**  
   Evaluate advanced models for better performance.

3. **Deploy with Streamlit**  
   Build a simple UI for product managers to test the system interactively.

---
