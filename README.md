# 🏨 Hotel Cancellation Prediction

## 📌 Project Overview

It is crucial for hotels to minimize last-minute cancellations that leave rooms unoccupied. High cancellation rates can lead to significant revenue loss.

This project analyzes key features that influence customer cancellations, so hotel management can:
- Predict potential cancellations
- Refine booking policies
- Develop a predictive Machine Learning model to reduce losses due to cancellations

---

## 📊 Dataset

- **Size:** 83,293 rows × 33 columns  
- **Period:** July 2017 – August 2019  
- **Source:** Hotel booking records containing customer details, booking behavior, and cancellation status

---

## 🧹 Data Preprocessing

To ensure model reliability and data quality, the following preprocessing steps were applied:

- ✅ **Multicollinearity Study & Feature Engineering**
- ✅ **Duplicate Handling**
- ✅ **Missing Value Handling**
- ✅ **Outlier Treatment**

---

## 🧠 Machine Learning Models

The following classification models were trained and evaluated to predict cancellation status:

- Logistic Regression  
- Decision Tree  
- Random Forest  
- Linear SVM  
- K-Nearest Neighbors (KNN)

---

## 🧪 Model Evaluation

### 🎯 Key Metric: **Recall (for class 1 = Cancelled)**

> Recall is prioritized to reduce **false negatives** (i.e., missed cancellations), which are more costly than false positives.

| Model              | Recall (Class 1) |
|-------------------|------------------|
| Logistic Regression | ~0.70            |
| Decision Tree       | **0.78**         |
| Random Forest       | **0.78** ✅       |
| K-Nearest Neighbors | ~0.76            |
| Linear SVM          | ~0.71            |

- **Random Forest** achieved the best balance between performance and generalization.
- Despite some overfitting across models, **Random Forest** remained the most reliable.

---

## 📈 Insights & Recommendations

### 1. 📅 **Seasonality & External Events**
- Booking volumes peak between **August to October**.
- Cancellations also spike during this period.
- Hotels should consider flexible but controlled policies during peak months.

### 2. 🌐 **Booking Channel & Behavior**
- **Online Travel Agencies (OTA)** and frequent booking changes are linked to higher cancellation rates.
- **Corporate** and **Direct** bookings are more stable.
- Suggestion: Incentivize stable channels and monitor frequent changers.

### 3. 💸 **Deposit Type & Cancellation Risk**
- **"No Deposit"** bookings show very high cancellation likelihood.
- Surprisingly, **"Non-Refundable"** also see notable cancellations.
- Suggestion: Consider partial deposits or stricter policies for "No Deposit" bookings.

### 4. ⏱️ **Lead Time Matters**
- Bookings with **long lead times** are significantly more likely to be canceled.
- Suggestion: Monitor long-lead bookings closely and offer flexible rebooking incentives.

---

