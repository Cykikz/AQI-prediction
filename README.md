# 🌫️ Air Quality Index (AQI) Prediction using Machine Learning

This project uses machine learning to predict the **Air Quality Index (AQI)** based on various air pollutant features like PM2.5, PM10, CO, SO2, etc. It includes data preprocessing, model training, evaluation, and comparison using popular ML algorithms.

---

## 📂 Project Overview

The goal is to build a machine learning model that can **accurately predict AQI values** for given environmental pollutant levels. The project includes:

- Data loading and preprocessing
- Feature encoding using OneHotEncoder
- Dimensionality reduction with PCA
- Model training using:
  - Linear Regression
  - Random Forest Regressor
  - XGBoost Regressor
- Evaluation using RMSE (Root Mean Squared Error)
- ML pipeline for clean and reproducible code

---

## 🧠 Machine Learning Models Used

### 🔹 Linear Regression
- A simple model that finds the best-fit line.
- Works well when data has a linear relationship.

### 🔹 Random Forest Regressor
- Ensemble of decision trees.
- Handles noisy, missing, and non-linear data well.

### 🔹 XGBoost Regressor
- Gradient Boosting model, very accurate and efficient.
- Used in many real-world problems and Kaggle competitions.

---

## ⚙️ How It Works

1. **Train-Test Split**: Data is divided into training and testing sets.
2. **ColumnTransformer**: Applies OneHotEncoding only to categorical features like city.
3. **PCA** *(optional)*: Reduces dimensionality for better performance.
4. **Pipeline**: Combines preprocessing and model in one object for clean usage.
5. **Model Evaluation**: RMSE is used to compare how well each model performs.

---

## 📊 Dataset

The dataset contains air pollution readings from various cities and times. It includes:
- Features like `PM2.5`, `PM10`, `NO2`, `SO2`, `CO`, `O3`, and `City`
- Target label: `AQI`

(*The dataset is either uploaded directly in the notebook or read from a CSV file.*)

---

## 📦 Libraries Used

- `pandas` – data manipulation
- `numpy` – numerical operations
- `matplotlib`, `seaborn` – plotting and visualization
- `sklearn` – preprocessing, modeling, evaluation
- `xgboost` – advanced gradient boosting model

---

## 🧪 Evaluation Metric

### 🧮 Mean Squared Error (MSE)
\[
\text{MSE} = \frac{1}{n} \sum (y_{\text{true}} - y_{\text{pred}})^2
\]

### 📉 RMSE (Root MSE)
- RMSE = √MSE
- Lower RMSE = better model

---

## 🚀 How to Run

1. Clone the repo  
   ```bash
   git clone https://github.com/<your-username>/<repo-name>
   cd <repo-name>

📈 Results
The model performance was compared across:

Linear Regression (fast and simple)(only regression) (worst performance)

Random Forest (medium complexity and slower)(regression and classification) (good performance)

XGBoost (complex and slow ) ( regression and classification) (Best performance)

XGBoost gave the lowest RMSE, showing the best accuracy.

✅ Future Improvements
Collect more real-time AQI data

Add time-series forecasting for AQI

Deploy as a web app or Android app

🧑‍💻 Author
Harshit Bhatt

Machine Learning Enthusiast

Open to feedback and collaboration!
