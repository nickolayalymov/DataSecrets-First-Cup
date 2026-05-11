# 🛠 Technical Task & Dataset Description

## 🎯 Objective
The goal is to build a machine learning model to predict the probability (`apply_promo`) that a customer will use a given promo code. This is a **binary classification** task where the output must be a probability score.

## 📊 Evaluation Metric
*   **Primary Metric:** `ROC-AUC`
*   The model is evaluated based on its ability to rank customers by their likelihood of conversion.

## 💾 Dataset Structure
The provided data consists of several relational tables. 
> **Note:** Full datasets are excluded from this repository due to size and licensing. You can find data structures in `data/samples/`.

### 1. `orders.csv` (Historical Orders)
Contains the 10 most recent orders for each client prior to November.
*   `OrderUUId` / `ClientUUId`: Unique identifiers.
*   `ProductTotalPrice` / `MenuPrice`: Financial data.
*   `apply_promo`: Flag indicating if a promo code was used.

### 2. `mobile_events.csv` (App Behavior)
Mobile app activity logs for October.
*   `EventName`: Type of action (e.g., open app, add to cart).
*   `Platform`: iOS or Android.
*   `Timestamp`: Event time.

### 3. `clients_promo_october.csv` (Campaigns)
Details of promotional offers sent in October.
*   `OrderPrice`: Minimum order value for activation.
*   `Discount`: Reward value.
*   `OrderType`: Channel (1 = Delivery, 2/3 = Restaurant).

### 4. `train_target.csv` & `test.csv` (Target Data)
Promotional offers for November. 
*   `apply_promo`: **Target Variable** (1 if used, 0 otherwise).

## ⚡ Technical Constraints
*   **Time Limit:** 2.0 seconds for inference.
*   **Memory Limit:** 256 MB.

## 📤 Submission Format
A CSV file with a single column `apply_promo` containing predicted probabilities.