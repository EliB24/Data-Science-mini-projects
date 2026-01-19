# House Prices - Decision Trees & Random Forest
The project demonstrates the basic principles of model training, validation, and the manifestations of underfitting and overfitting.
The main goal of the project is to demonstrate a basic understanding of machine learning before moving on to more complex processes.

---

## Project Overview

The dataset contains numerical features describing houses:

- Overall quality
- Living area
- Basement size
- Lot area
- Number of bedrooms and bathrooms
- Year built
- Garage capacity

Target:

- SalePrice - house price

The project explores:

- How a Decision Tree fits training data
- Why validation is necessary
- How underfitting and overfitting appear
- How hyperparameters affect model quality
- Why Random Forest improves over a single tree

---

## Files Included

- **04_ml_from_baseline_to_randomforest.ipynb** - main Jupyter Notebook 
- **house_prices_practice.csv** - input dataset  
- **README.md** - project description

---

## Technologies Used

- **Python 3**  
- **pandas** - data manipulation
- **scikit-learn** - DecisionTreeRegressor, RandomForestRegressor
- **Jupyter Notebook / JupyterLab**

---

## Key Insights

- A model evaluated only on training data can look perfect but generalize poorly
- Small trees underfit; very large trees overfit
- Validation MAE clearly shows the optimal model complexity
- Random Forest significantly reduces error by averaging many trees
- Ensemble methods are more stable and generalize better than a single tree

---

## How to Run

1. Open `04_ml_from_baseline_to_randomforest.ipynb` in Jupyter Notebook or JupyterLab  
2. Make sure all required libraries are installed  
3. Run the cells from top to bottom  
