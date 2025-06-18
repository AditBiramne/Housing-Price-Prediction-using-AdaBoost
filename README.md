# 🏠 Housing Price Prediction using AdaBoost

This project demonstrates how to use the **AdaBoost Classification Algorithm** to predict housing prices based on various features like furnishing status, guestroom availability, air conditioning, and more.

## 📌 Overview

- Converts categorical data into numerical format using custom mappings  
- Splits the dataset into training and testing sets  
- Trains an `AdaBoostClassifier` from `scikit-learn`  
- Evaluates performance by comparing predictions with actual price categories  

> **Note:** This approach treats **price as a categorical target**. If you're predicting **continuous prices**, consider using `AdaBoostRegressor`.

## 📂 Dataset

- **Source:** `Housing.csv`
- **Features include:**
  - `furnishingstatus`
  - `guestroom`
  - `mainroad`
  - `basement`
  - `hotwaterheating`
  - `airconditioning`
  - `prefarea`
- **Target:** `price` (treated as categorical for this model)

## ⚙️ Technologies Used

- Python  
- NumPy  
- Pandas  
- scikit-learn  

## 🚀 How to Run

1. Install the required libraries:

    ```bash
    pip install pandas numpy scikit-learn
    ```

2. Run the script:

    ```bash
    python housing_adaboost.py
    ```

## 📈 Output

- The script prints the **prediction accuracy** (as a percentage) using `AdaBoostClassifier`.

## 📌 Future Improvements

- Use `AdaBoostRegressor` for more accurate **continuous value prediction**  
- Apply **feature scaling** (e.g., `StandardScaler`, `MinMaxScaler`)  
- Evaluate performance using **RMSE (Root Mean Square Error)** or **MAE (Mean Absolute Error)**  
