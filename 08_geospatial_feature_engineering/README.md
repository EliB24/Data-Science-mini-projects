# California Housing Prices - Prediction with Geospatial Feature Engineering
The project demonstrates the complete development process for a machine learning model used to predict housing prices. Geospatial analysis is used as part of the project
The key goal is to demonstrate how taking geographic factors into account can improve the accuracy of a model that works with tabular data

---

## Project Overview

The dataset includes the following feature groups:

**Numerical features**
- Longitude and latitude
- Housing median age
- Total rooms and bedrooms
- Population and households
- Median income

**Categorical features**
- Ocean proximity

**Geospatial features (engineered)**
- Distances to major cities (Los Angeles, San Francisco, San Diego, Sacramento)
- Neighborhood density within multiple radii
- Regional clusters derived from spatial coordinates

The target variable is:

- median_house_value - median house price in a given area

### Methods and Techniques

The project demonstrates the following machine learning concepts:

- Data exploration and visualization
- Feature engineering with geospatial data
- Coordinate reference system (CRS) transformation
- Distance-based and density-based spatial features
- Universal preprocessing with *Pipeline* and *ColumnTransformer*
- Model comparison using:
  - Random Forest
  - XGBoost
- Model evaluation using:
  - Single train–validation split
  - K-Fold cross-validation (MAE and RMSE)
 
---

## Files Included

- **08_geospatial_feature_engineering.ipynb** - main Jupyter Notebook 
- **housing.csv** - training dataset
- **README.md** - project description

---

## Technologies Used

- **Python 3**  
- **pandas** - data manipulation
- **NumPy**
- **scikit-learn** - preprocessing, pipelines, models, cross-validation
- **matplotlib** - visualization
- **GeoPandas** - geospatial processing
- **XGBoost** - gradient boosting model
- **Jupyter Notebook / JupyterLab**

---

## Results

- Adding geospatial features leads to a clear improvement in prediction accuracy
- Cross-validation confirms that the improvement is stable across different data splits
- XGBoost outperforms Random Forest when trained on geo-enhanced features
- The final model achieves lower MAE and RMSE compared to the baseline

---

## How to Run

1. Open `08_geospatial_feature_engineering.ipynb` in Jupyter Notebook or JupyterLab  
2. Make sure all required libraries are installed
3. Place `housing.csv` in the same directory
4. Run the cells from top to bottom

---

### Notes

The target variable has an upper cap, which creates censored values in the dataset  
This limitation comes from the data itself and is considered during result interpretation
