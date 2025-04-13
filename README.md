# 🏠 House Price Analysis Pipeline

This repository provides a complete machine learning pipeline for analyzing and predicting house sale prices. The pipeline includes data loading, preprocessing, feature engineering, feature selection using Lasso regression, model training, and evaluation.

## 📦 Installation

Before running the code, install the required libraries using the following command:

```bash
!conda install -y -c conda-forge pandas numpy matplotlib seaborn scikit-learn -q
```

## 📁 Project Structure

- `HousePriceAnalysis` class: Handles the entire ML workflow from preprocessing to model evaluation.
- `dataset.csv`: Input dataset file (not included).
- `main block`: Demonstrates the usage of the pipeline with a CSV file.

## 🚀 How to Run

1. Place your house sales dataset in the working directory and name it `dataset.csv`.
2. Run the script. The pipeline will:
   - Preprocess the data
   - Engineer new features
   - Apply Lasso for feature selection
   - Find the optimal feature threshold
   - Train and evaluate a linear regression model

## 📊 Features Used

- Numeric: LotArea, GrLivArea, TotalBsmtSF, GarageArea, etc.
- Engineered: TotalBath, HouseAge, Quality_Area, Quality_Age
- Categorical: Alley, LotType, BldgType, HouseStyle, SaleType, SaleCondition

## 📈 Evaluation Metrics

- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

## 📉 Visualizations

- Correlation Matrix
- Feature Importance from Lasso
- Selected Feature Scatter Plots
- Model Performance Plots (Actual vs Predicted, Residuals)

## 📌 Notes

- Ensure your dataset is clean and named appropriately.
- Log transformations are applied to handle skewness.
- The pipeline uses `RobustScaler` and `OneHotEncoder` for scaling and encoding respectively.

---

**Author**: Mohammad Aghaee
**License**: MIT