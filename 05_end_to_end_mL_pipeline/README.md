# House Price Prediction - End-to-End ML Pipeline
This project illustrates the complete machine learning cycle for predicting real estate prices.
The main goal is to demonstrate an effective machine learning production process using the relevant methods from the scikit-learn library.

---

## Project Overview

The dataset contains information about residential properties, including:

- Overall quality of the house
- Living area
- Basement size
- Lot area
- Number of rooms and bathrooms
- Year built
- Garage information
- Categorical features such as zoning, neighborhood, and building type

The target variable is:

- SalePrice — final sale price of the house

The project includes the following concepts:

- How to create a universal preprocessing pipeline for numerical and categorical data?
- How does the Random Forest algorithm work with cross-validation?
- How can XGBoost be used to improve model accuracy when optimizing hyperparameters?  
- How can the best model be determined based on validation metrics?

---

## Files Included

- **05_end_to_end_pipeline.ipynb** - main Jupyter Notebook 
- **train.csv** - training dataset
- **test.csv** - test dataset
- **README.md** - project description

---

## Technologies Used

- **Python 3**  
- **pandas** - data manipulation
- **scikit-learn** - preprocessing, pipelines, cross-validation, Random Forest
- **XGBoost** - gradient boosting model
- **Jupyter Notebook / JupyterLab**

---

## Results

- Random Forest provides a solid foundation with stable MAE, verified through cross-validation
- XGBoost with tuned hyperparameters achieves a noticeably lower MAE
- The final model is selected based on cross-validation results and then trained on the full dataset
- The result is a clean table with IDs and predicted SalePrice, ready for further analysis

---

## How to Run

1. Open `05_end_to_end_pipeline.ipynb` in Jupyter Notebook or JupyterLab  
2. Make sure all required libraries are installed
3. Place `train.csv` and `test.csv` in the same directory
4. Run the cells from top to bottom  
