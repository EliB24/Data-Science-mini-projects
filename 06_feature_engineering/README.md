# House Prices - Feature Engineering and Model Optimization
This project demonstrates a complex machine learning workflow for predicting housing prices.
The base model and preprocessing approach were taken from a previous project and expanded with additional feature engineering, clustering, and encoding strategies.
The main goal ofthis project is to show how iterative model improvement works in practice: starting with a solid foundation, analyzing features, and gradually adding more complex methods while tracking their actual impact on model performance.

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

### Modeling Strategy

1. Baseline
   - Tuned XGBoost regressor
   - Numerical features imputed with median
   - Numerical features imputed with median
   - Cross-validation used as the primary evaluation method (MAE)
2. Mutual Information analysis
   - Identification of the most informative features
   - Exploratory analysis
3. Feature engineering
   - Creation of aggregated and domain-based features (TotalSF, TotalBath, HouseAge)
   - Binary flags for important structural characteristics
   - Evaluation of feature impact using cross-validation
4. Clustering
   - Houses are grouped using KMeans based on size, quality, and structural characteristics
   - Each house is assigned to a cluster
   - The cluster label is added as a new categorical feature to the model
5. Encoding experiments
   - Comparison of One-Hot Encoding and hybrid approaches
   - High-cardinality categorical features handled separately
   - All experiments evaluated consistently using cross-validation

---

## Files Included

- **06_feature_engineering.ipynb** - main Jupyter Notebook 
- **train.csv** - training dataset
- **test.csv** - test dataset
- **README.md** - project description

---

## Technologies Used

- **Python 3**  
- **pandas** - data manipulation
- **NumPy**
- **scikit-learn** - preprocessing, pipelines, cross-validation, clustering
- **XGBoost** - gradient boosting model
- **seaborn / matplotlib** - visualization
- **Jupyter Notebook / JupyterLab**

---

## Results

- The tuned XGBoost baseline provides strong performance
- Feature engineering results in small but consistent improvements
- Clustering adds useful high-level structure and slightly improves generalization
- More complex encoding strategies do not always lead to better results.
- The final model combines engineered features with a stable preprocessing ppeline

---

## How to Run

1. Open `06_feature_engineering.ipynb` in Jupyter Notebook or JupyterLab  
2. Make sure all required libraries are installed
3. Place `train.csv` and `test.csv` in the same directory
4. Run the cells from top to bottom  
