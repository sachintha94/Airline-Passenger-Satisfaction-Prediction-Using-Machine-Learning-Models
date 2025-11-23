# Airline Passenger Satisfaction Prediction Using Machine Learning

This project analyzes an airline passenger satisfaction dataset and builds multiple machine learning models to predict whether a passenger is **satisfied** or **neutral/dissatisfied** based on demographic, service-level, and travel-related factors.  
The task includes data preprocessing, exploratory analysis, model development, and performance evaluation.

---

## 📦 Project Overview

The goal of this project is to:

- Load and preprocess the provided **train** and **test** datasets  
- Explore factors correlated with passenger satisfaction  
- Train multiple AI models  
- Compare model performances using:
  - Accuracy  
  - Precision  
  - Confusion Matrix  

The best-performing model will be selected for the final evaluation.

---

## 📁 Dataset Description

Two CSV files were provided:

- `airline_train.csv`
- `airline_test.csv`

### 📝 Key Features
The dataset includes passenger details such as:

- Gender  
- Customer Type (Loyal / Disloyal)  
- Type of Travel (Personal / Business)  
- Travel Class (Eco, Eco Plus, Business)  
- Flight distance  
- Service ratings (Wi-Fi, Check-in, Online boarding, Food & drink, Cleanliness, etc.)  
- Delay information  
- Satisfaction label (Satisfied / Neutral or Dissatisfied)

Dataset summary extracted from analysis:

| Detail | Train | Test |
|--------|-------|------|
| Rows | 103,904 | 25,976 |
| Columns | 25 | 25 |
| Missing Values | 310 | 83 |
| Missing Values Removed | 103,594 rows | 25,893 rows |

Label Encoding Example:

