# Predicting House Prices With Linear Regression

## Project Overview

This project was developed as part of my **Data Analytics Internship — Level 2, Task 1**.

The objective is to predict residential property selling prices using machine learning regression algorithms and various property characteristics.

The project includes exploratory data analysis, data preprocessing, feature selection, Linear Regression modeling, performance evaluation and comparison with regularized regression techniques.

## Dataset

- **Source:** Kaggle
- **Dataset:** Ames Housing Dataset
- **Dataset Link:** https://www.kaggle.com/datasets/shashanknecrothapa/ames-housing-dataset
- **Target Variable:** `SalePrice` (or its equivalent after column standardization)

The Ames Housing dataset contains residential property information, including house size, overall quality, location, construction year and sale price.

The original modeling code uses features such as:

- Above-ground living area
- Overall house quality
- Basement area
- Garage capacity
- Number of bedrooms
- Number of bathrooms
- Lot area
- House age
- Neighborhood
- House style
- Central air conditioning

Column names are standardized where necessary to match the selected dataset.

## Technologies Used

- Python
- pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- KaggleHub
- Jupyter Notebook / Google Colab

## Project Workflow

### 1. Dataset Collection

- Downloaded the Ames Housing dataset from Kaggle using KaggleHub.
- Loaded the CSV file into pandas.
- Inspected dataset structure, columns and data types.

### 2. Exploratory Data Analysis

- Identified missing values and duplicate records.
- Calculated descriptive statistics.
- Examined the distribution of house prices.
- Analysed relationships between property attributes and sale prices.

### 3. Feature Engineering and Selection

Created a `HouseAge` feature using the construction year and year of sale.

Selected numerical and categorical features based on their potential association with house prices.

### 4. Data Preprocessing

- Handled missing numerical values using median imputation.
- Handled missing categorical values using mode imputation.
- Applied One-Hot Encoding to categorical variables.
- Applied StandardScaler to numerical predictors.

### 5. Correlation Analysis

Created a correlation heatmap to identify numerical features associated with the target variable, `SalePrice`.

### 6. Train-Test Split

Divided the dataset into:

- 80% training data
- 20% testing data

### 7. Model Development

Trained the following regression algorithms:

1. Linear Regression
2. Ridge Regression
3. Lasso Regression

Linear Regression serves as the primary model, while Ridge and Lasso provide additional regularized comparisons.

### 8. Model Evaluation

Evaluated regression performance using:

**Mean Squared Error (MSE)**

Measures the average squared difference between actual and predicted prices.

**Root Mean Squared Error (RMSE)**

Measures prediction error in the same unit as house prices.

**R² Score**

Measures how much variation in house prices is explained by the model compared with a mean-prediction baseline.

### 9. Residual Analysis

Analysed prediction errors using:

- Actual vs Predicted Price Scatterplot
- Residual vs Predicted Price Plot
- Residual Distribution
- Absolute Error Plot

### 10. Coefficient Analysis

Examined positive and negative Linear Regression coefficients to understand how selected property characteristics are associated with predicted selling prices.

## Visualizations

- House Price Distribution
- House Price Boxplot
- Correlation Heatmap
- Living Area vs Sale Price
- Average Sale Price by Overall Quality
- Average Sale Price by Neighborhood
- Actual vs Predicted Prices
- Residual Plots
- Regression Coefficient Chart
- Model RMSE Comparison

## Results

The project compares three regression algorithms using predictive performance metrics.

**Replace the placeholders after running the notebook:**

| Model | MSE | RMSE | R² |
|---|---|---|---|
| Linear Regression | TBD | TBD | TBD |
| Ridge Regression | TBD | TBD | TBD |
| Lasso Regression | TBD | TBD | TBD |

The model with the lowest test RMSE is reported in the notebook. A more rigorous model selection process would tune hyperparameters through training-set cross-validation.

## How to Run

1. Clone or download the repository.
2. Install the dependencies.

```bash
pip install kagglehub pandas numpy matplotlib seaborn scikit-learn
```

3. Open the Jupyter Notebook or Google Colab.
4. Run the dataset-loading section.
5. Verify and standardize the dataset column names.
6. Execute the remaining notebook cells in sequence.

## Output Files

- `house_price_predictions.csv`
- `linear_regression_coefficients.csv`
- `house_price_model_comparison.csv`

## Conclusion

The project demonstrates how supervised machine learning can be applied to residential property price prediction.

Exploratory analysis, feature engineering and regression modeling help identify patterns in housing data. Model evaluation and residual analysis provide insights into prediction accuracy and model limitations.

## Future Improvements

- Hyperparameter tuning using GridSearchCV
- Cross-validation
- Additional feature engineering
- Random Forest and Gradient Boosting regression
- House price prediction web application

## Author

**K Shivaram Goud**  
Data Analytics Intern  
B.Tech — Artificial Intelligence and Machine Learning