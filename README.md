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

## Label Encoding Example:
Gender: {'Male':1, 'Female':0}
Customer Type: {'Loyal Customer':1, 'disloyal Customer':0}
Type of Travel: {'Personal Travel':1, 'Business travel':0}
Class: {'Eco Plus':1, 'Business':0, 'Eco':2}
Satisfaction: {'satisfied':1, 'neutral or dissatisfied':0}


---

## 🔧 Data Preprocessing

The following steps were performed:

- Drop missing values (Arrival Delay in Minutes)
- Encode categorical columns
- Scale or normalize numerical features where required
- Split dataset into input features (X) and output label (y)
- Prepare train/test sets based on provided files

---

## 🤖 Machine Learning Models Used

Four supervised learning models were implemented:

1. **Logistic Regression**
2. **Decision Tree Classifier**
3. **Random Forest Classifier**
4. **Support Vector Machine (SVM)**

Each model was evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-Score  
- Confusion Matrix  

---

## 📊 Model Performance Summary

| Model | Accuracy | Precision | Notes |
|-------|----------|-----------|-------|
| Logistic Regression | ~0.80 | 0.7412 | Good linear baseline |
| Decision Tree | ~0.95 | 0.9449 | Strong performance, fast |
| **Random Forest** | **0.9621** | **0.9704** | ⭐ Best model |
| SVM | ~0.65 | 0.6969 | Underperformed |

---

## 🏆 Best Performing Model: Random Forest

Random Forest achieved the **highest accuracy** and **best precision**, making it the optimal model for this prediction task.

Key influencing features identified:

- Online boarding  
- Inflight Wi-Fi service  
- Travel class  
- Type of travel  

---

## 📉 Confusion Matrices

![01](https://github.com/user-attachments/assets/cb6669e5-b5cd-4535-9f49-bb4e254f75bf)

![02](https://github.com/user-attachments/assets/394b2ef4-b4b7-44e1-8082-4aa16d94cdd7)

![03](https://github.com/user-attachments/assets/d624ebfb-2b71-4a82-8875-55d677c33d6d)

![04](https://github.com/user-attachments/assets/c6ff6d9c-2e75-46bc-8296-f6e7de4258e3)
