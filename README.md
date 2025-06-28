# 🏘️ Predicting Airbnb Listing Prices in Melbourne

This data science project aims to develop machine learning models that accurately predict Airbnb listing prices in Melbourne, Australia. The analysis was conducted as part of a university assignment and submitted to a Kaggle competition.

## 📌 Objective

- Build predictive models to estimate listing prices.
- Apply feature engineering to improve model performance.
- Evaluate and compare different regression techniques.
- Submit predictions to Kaggle and track RMSE performance.

## 📁 Dataset

- Source: Provided via Kaggle competition platform.
- Size: ~10,000+ listings.
- Features: Property type, host status, amenities, location, reviews, etc.

## 🔍 Methodology

### 1. Exploratory Data Analysis (EDA)
- Investigated distribution of target variable (`price`)
- Visualised geographic distribution of listings using latitude and longitude
- Analysed missing values and data quality

### 2. Feature Engineering
- Cleaned string-based numerical features
- Created new features from `amenities`, `host_verifications`, `location`, `description`, and `neighbourhood_overview`
- Imputed missing values using suitable methods for each column
- Encoded categorical variables (top N values + “other” class)

### 3. Model Building
- **Random Forest Regressor** (Baseline)
- **XGBoost Regressor**
- **LightGBM Regressor**
- All models trained with cross-validation and tuned for optimal RMSE

## 📊 Results

| Model                  | CV RMSE (log(price)) |
|------------------------|----------------------|
| Random Forest          | 0.4228               |
| XGBoost                | 0.4208               |
| LightGBM               | 0.3986               |

> Final model: LightGBM Regressor with post-processing

## 🏆 Kaggle Submission

- Team Name: `BUSA8001_BroccoliSpace`
- Private Leaderboard RMSE: **111.981** (Top 10)
- Post-contest Individual Rebuild: **111.105 RMSE** (Improved performance)

## 🛠️ Tools Used

- Python (Pandas, NumPy, Scikit-Learn, XGBoost, LightGBM)
- Jupyter Notebook
- Matplotlib / Seaborn
- Kaggle API

## 👤 Author

Sulaiman Yusuf Zakaria 
Master of Business Analytics  
Macquarie University  

---

## 📎 License

This project is for educational purposes only and does not represent production-grade code. Data belongs to the original Kaggle competition provider.

