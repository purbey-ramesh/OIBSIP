# House Price Prediction with Linear Regression

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white" alt="Python version" />
  <img src="https://img.shields.io/badge/Scikit--Learn-1.x-F7931E?logo=scikitlearn&logoColor=white" alt="Scikit-learn" />
  <img src="https://img.shields.io/badge/License-MIT-green" alt="MIT License" />
</p>

This project predicts house sale prices using the Ames Housing dataset and a linear regression model. It covers the full data science workflow, including data cleaning, feature engineering, EDA, model training, evaluation, and interpretation.

## Overview

The goal is to estimate property sale prices using housing attributes such as:

- house size and layout
- property quality and condition
- age and renovation history
- basement and garage availability
- neighborhood and locality effects

## Project Structure

```text
DataAnalytics-L2-PredictingHousePriceWithLinearRegression/
├── data/                          # dataset files
├── notebook/
│   └── Linear_Regression_HousePrice_Prediction.ipynb
├── screenshots/                  # charts and model outputs
└──  README.md
```

## Dataset

The project uses the Ames Housing dataset, which contains residential property features and sale prices.

## Features Engineering

To improve model quality and reduce redundancy, several engineered features were created, including:

- `Total SF`
- `Total Bath`
- `House Age`
- `Year Since Remod`
- `Has Garage`
- `Has Basement`
- `Has Fireplace`

These features compress overlapping raw information into more interpretable variables and help reduce multicollinearity.

## Workflow

1. Load the dataset
2. Handle missing values
3. Create engineered features
4. Encode categorical variables
5. Train a Linear Regression model
6. Evaluate using RMSE and R²
7. Compare actual vs predicted prices
8. Interpret coefficients and feature importance

## Technologies Used

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn

## Setup

Create a virtual environment and install the dependencies:

```bash
python -m venv .venv
source .venv/bin/activate   # macOS/Linux
.venv\Scripts\activate      # Windows
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Run the Project

Open the notebook and execute cells in order:

```bash
jupyter notebook notebook/Linear_Regression_HousePrice_Prediction.ipynb
```

Or use VS Code Notebook mode to run the analysis interactively.

## Model Evaluation

The model is evaluated using:

- RMSE: average absolute prediction error in dollars
- R²: proportion of variance explained by the model

## Results

The model performs reasonably well as a baseline approach for predicting house prices. Key drivers of value include:

- home size and overall usable space
- housing quality and condition
- presence of garage/basement amenities
- neighborhood/location effects
- age and renovation history

## Summary

This project demonstrates that careful preprocessing and feature engineering can make linear regression an effective baseline model for house price prediction. It also shows the importance of understanding feature relationships, avoiding redundancy, and interpreting the model in a real-world context.

## License

This project is licensed under the MIT License.
