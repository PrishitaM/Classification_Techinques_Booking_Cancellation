# Classification_Techinques_Booking_Cancellation
Machine learning project to predict hotel booking cancellations using EDA, Logistic Regression, and Decision Tree models on INN Hotels data.
# 🏨 Hotel Booking Cancellation Prediction – INN Hotels

## 📌 Project Overview
This project aims to predict hotel booking cancellations using machine learning techniques.  
It helps **INN Hotels Group (Portugal)** identify bookings that are likely to be canceled in advance, enabling better revenue management and operational planning.

The project follows an end-to-end data science workflow including exploratory data analysis, data preprocessing, model building, evaluation, and final model selection.

---

## 🎯 Problem Statement
Hotel booking cancellations cause revenue loss and inefficient room utilization.  
This project focuses on:
- Identifying factors that influence booking cancellations
- Building predictive models to classify bookings as **Canceled** or **Not Canceled**
- Selecting the most effective model for deployment

---

## 📂 Dataset Description
The dataset contains booking-level information such as:
- Customer demographics and booking details
- Market segment and distribution channel
- Lead time and length of stay
- Average price per room
- Special requests and repeat guest information

**Target Variable:**  
`booking_status` (Canceled / Not Canceled)

---

## 🔍 Exploratory Data Analysis
Exploratory analysis was performed to understand booking patterns and cancellation behavior:
- Seasonal trends and busiest months
- Cancellation rates across market segments
- Impact of lead time, room price, repeat guests, and special requests
- Correlation analysis to examine multicollinearity

Key insight:  
Longer lead times, higher room prices, and certain booking channels show higher cancellation rates, while repeat guests have a much lower tendency to cancel.

---

## ⚙️ Data Preprocessing
- Verified that the dataset contains no missing values
- Identified outliers in numerical variables and retained them as they represent genuine customer behavior
- Removed non-informative identifiers
- Converted categorical variables using **one-hot encoding**
- Applied **train–test split** and **feature scaling**

---

## 🤖 Models Implemented

### Logistic Regression (Statsmodels)
- Checked multicollinearity using correlation analysis and Variance Inflation Factor (VIF)
- Removed statistically insignificant features based on **p-values**
- Determined the optimal classification threshold using **ROC curve analysis**
- Achieved approximately **81% accuracy** with good interpretability

### Decision Tree Classifier (Scikit-learn)
- Base Decision Tree model
- Pre-pruned Decision Tree to reduce overfitting
- Post-pruned Decision Tree for improved generalization

**Best Performing Model:**  
Post-pruned Decision Tree with approximately **88% accuracy** and balanced evaluation metrics.

---

## 📊 Model Evaluation Metrics
- Accuracy
- Precision
- Recall
- ROC–AUC Score

---

## 🏆 Final Outcome
The post-pruned Decision Tree model demonstrated the best overall performance and is recommended for predicting hotel booking cancellations effectively.

---

## 🛠️ Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Statsmodels  

---

## 🚀 Future Improvements
- Apply ensemble techniques such as Random Forest and XGBoost
- Handle class imbalance using resampling methods
- Deploy the model using a web application (Flask or Streamlit)
- Integrate real-time booking data

---

## 👩‍💻 Author
**Prishita Matreja**
