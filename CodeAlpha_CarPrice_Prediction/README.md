# 🚗 Car Price Prediction using Machine Learning

## 📌 Project Overview

This project focuses on building an **end-to-end car price prediction system** using machine learning techniques. The goal is to predict the **selling price of used cars** based on various car-related features such as year of manufacture, mileage, fuel type, transmission type, ownership history, and present showroom price.

The project follows a **real-world data science workflow**, starting from data understanding and exploratory analysis to model building, evaluation, and prediction.

---

## 🎯 Problem Statement

* Collect car-related features that influence resale value
* Train a **regression model** to predict car selling prices
* Perform **data preprocessing, feature encoding, and model evaluation**
* Use **Python libraries** like Pandas, Scikit-learn, and Matplotlib
* Understand the **real-world application** of machine learning in price prediction

---

## 🧰 Tools & Technologies

* **Python**
* **Pandas** – data manipulation
* **NumPy** – numerical operations
* **Matplotlib** – data visualization
* **Scikit-learn** – machine learning models & evaluation

---

## 📂 Dataset Description

The dataset contains information about used cars with the following columns:

| Feature       | Description                             |
| ------------- | --------------------------------------- |
| Car_Name      | Name of the car (not used for modeling) |
| Year          | Manufacturing year                      |
| Selling_Price | Target variable (price in lakhs)        |
| Present_Price | Original showroom price                 |
| Driven_kms    | Total kilometers driven                 |
| Fuel_Type     | Petrol / Diesel / CNG                   |
| Selling_type  | Dealer or Individual                    |
| Transmission  | Manual or Automatic                     |
| Owner         | Number of previous owners               |

---

## 🔍 Exploratory Data Analysis (EDA)

EDA was performed to understand relationships between features and selling price.

### Key Insights

### 📊 Selling Price Distribution

* The distribution is **right-skewed**
* Most cars fall in the **low to mid-price range**
* A few high-priced outliers represent premium vehicles

### 📈 Price vs Manufacturing Year

* Newer cars generally have **higher selling prices**
* Clear effect of **depreciation over time**
* Significant price variation within the same year

### 📉 Price vs Driven Kilometers

* **Negative relationship** between driven kilometers and selling price
* Cars with higher mileage tend to sell for lower prices
* Low-mileage cars show high price variability

### ⛽ Price by Fuel Type

* **Diesel cars** have the highest median resale price
* **Petrol cars** fall in the mid-range
* **CNG cars** are the cheapest and most consistent
* Premium outliers mainly appear in diesel and petrol categories

### ⚙️ Price by Transmission Type

* **Automatic cars** generally command higher resale prices
* Automatic segment shows higher variability and premium outliers
* Manual cars are mostly concentrated in lower price ranges

---

## 🧹 Data Preprocessing

* Dropped irrelevant column: `Car_Name`
* Encoded categorical features using **One-Hot Encoding**
* Split data into **training and testing sets**

---

## 🤖 Model Building

### Baseline Model: Linear Regression

* Used to establish a simple baseline
* Easy to interpret feature relationships

### Advanced Model: Random Forest Regressor

* Captures **non-linear relationships** and feature interactions
* Achieved significantly better performance

### Hyperparameter Tuning

* Applied **GridSearchCV** to find optimal parameters
* Selected the best-performing model using cross-validation

---

## 📏 Model Evaluation

The model was evaluated using standard regression metrics:

* **MAE (Mean Absolute Error)** – average prediction error
* **RMSE (Root Mean Squared Error)** – penalizes large errors
* **R² Score** – explains variance in selling price

### Final Performance (Best Model)

* **MAE ≈ 0.59**
* **RMSE ≈ 0.87**
* **R² ≈ 0.96**

➡️ Indicates a **strong and reliable prediction model**

---

## 🔍 Error Analysis

* Compared actual vs predicted prices
* Analyzed residual patterns
* Identified higher errors for premium-priced cars
* Confirmed the need for non-linear modeling

---

## 🔢 Making Predictions

The trained model can predict the selling price of a new car by providing inputs such as:

* Year
* Present price
* Driven kilometers
* Fuel type
* Transmission
* Selling type
* Ownership

Predictions are made after applying the **same preprocessing and encoding steps** used during training.

---

## 🌍 Real-World Applications

* Used-car resale platforms (Cars24, OLX Autos)
* Dealer pricing tools
* Loan & insurance valuation
* Market trend analysis

---

## ✅ Key Takeaways

* Start with simple models before moving to complex ones
* EDA is crucial for understanding data behavior
* Feature quality matters more than model complexity
* Random Forest effectively captures real-world pricing patterns

---

## 🚀 Future Improvements

* Add brand-level features if available
* Apply log transformations for skewed variables
* Try Gradient Boosting / XGBoost
* Deploy as a **Streamlit web app**

---

## 📌 Conclusion

This project demonstrates a **complete machine learning pipeline** for car price prediction, from data exploration to model deployment readiness. It reflects **real-world data science practices** and provides a strong foundation for further enhancements.

---

⭐ *If you find this project useful, feel free to star the repository!*

