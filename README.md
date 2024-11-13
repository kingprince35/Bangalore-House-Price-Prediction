# Bangalore House Price Prediction 🏠

Welcome to the **Bangalore House Price Prediction** project! This project aims to accurately predict housing prices in Bangalore, India, based on various features like location, number of bedrooms, bathrooms, square footage, and more. We implemented a regression model using machine learning to provide these predictions.

## 📜 Project Overview

Bangalore is a rapidly growing city, and understanding real estate trends is crucial. This project leverages a dataset of housing information to build a predictive model for house prices. By analyzing key factors like the total square footage, location, and the number of bedrooms, we aim to estimate the price of homes across different neighborhoods in Bangalore.

## 📁 Dataset

The dataset used in this project includes the following features:
- **Location:** Neighborhood or area within Bangalore.
- **Size:** Number of bedrooms (e.g., 2 BHK, 3 BHK).
- **Total Sqft:** Total square footage of the house.
- **Bath:** Number of bathrooms.
- **Price:** The price of the house (target variable).

## 🔍 Data Cleaning and Feature Engineering

To prepare the dataset for modeling, several preprocessing steps were taken:
1. **Handling Missing Values**: Dropped rows with missing values to ensure data integrity.
2. **Feature Engineering**:
   - Converted `size` into numerical values representing the number of bedrooms.
   - Created a `price_per_sqft` feature for better understanding of pricing trends.
3. **Dimensionality Reduction**: Reduced the number of unique locations by grouping smaller categories into an "other" category, simplifying the model.
4. **Outlier Removal**: Removed extreme outliers based on square footage per bedroom and price per square foot.

## ⚙️ Model Development

We implemented a **Linear Regression** model to predict house prices. The model was evaluated using:
- **Train-Test Split**: 80% training data and 20% testing data.
- **K-Fold Cross-Validation**: Performed cross-validation to assess the model's consistency.

The model achieved an **accuracy of approximately 87%**, providing reliable price predictions.

## 📈 Results and Visualization

The model was tested with sample inputs, and predictions were visualized using scatter plots to display price distributions across neighborhoods. Additional visualizations such as histograms showed the distribution of prices per square foot across various areas, providing deeper insights into the Bangalore housing market.

## 🚀 Getting Started

### Prerequisites

Make sure you have the following libraries installed:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn




