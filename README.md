# 🏠 House Price Prediction

A machine learning project that predicts house prices from property features — area, bedrooms, bathrooms, age, location, and property type — using regression models built with scikit-learn.

## 📌 Project Overview

This project follows a structured 7-day ML workflow:

| Day | Task |
|---|---|
| 1 | Understand the data — load dataset, check missing values, visualize relationships |
| 2 | Data preparation — handle missing values, encode categorical variables, train-test split |
| 3 | Build Linear Regression from scratch (Normal Equation) |
| 4 | Train with scikit-learn's `LinearRegression` |
| 5 | Evaluate model — MAE, MSE, RMSE, R² |
| 6 | Improve model — Polynomial Features, Decision Tree, Random Forest |
| 7 | Interpret & present — coefficients, feature importance, insights |

## 📊 Dataset

- **300 property records**
- Features: `Area`, `Bedrooms`, `Bathrooms`, `Age`, `Location` (Rural / Suburb / City Center), `Property_Type` (House / Villa / Apartment)
- Target: `Price`

## 🎯 Results

| Model | MAE | R² Score |
|---|---|---|
| Linear Regression (sklearn) | ₹2,188,736 | 0.9406 |
| Linear Regression (from scratch) | ₹2,188,736 | 0.9406 |
| Polynomial Regression (deg 2) | ₹2,367,902 | 0.9290 |
| Decision Tree Regressor | ₹2,388,254 | 0.9324 |
| **Random Forest Regressor** | **₹1,483,832** | **0.9709** |

**Best Features:** Area, Location

The **Random Forest Regressor** is the best-performing model, explaining ~97% of the variance in house prices.

## 🛠️ Tech Stack

- Python 3
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
- Jupyter Notebook

## 📁 Repository Structure

```
house-price-prediction/
├── house_price_prediction.ipynb    # Full analysis & model notebook
├── house_data.csv                  # Dataset (300 records)
├── model_evaluation_report.md      # Detailed evaluation report & insights
├── requirements.txt                # Python dependencies
└── predictions_vs_actual.png       # Predictions vs Actual visualization
```

## 🚀 How to Run

```bash
git clone https://github.com/<your-username>/house-price-prediction.git
cd house-price-prediction
pip install -r requirements.txt
jupyter notebook house_price_prediction.ipynb
```

## 📈 Key Insights

- **Area** is the strongest predictor of price across all models.
- **Location** significantly impacts price — City Center > Suburb > Rural.
- Ensemble methods (Random Forest) outperform simple Linear Regression, indicating non-linear relationships in the data.
- The from-scratch Linear Regression implementation validated against scikit-learn's results, confirming correctness of the underlying math.

## 👤 Author

**Akshaya Venkatakrishnan**
MSc Data Science | Data Analysis Intern @ Cognifyz IT Solutions Pvt. Ltd.

## 📄 License

This project is open source and available for academic and educational use.
