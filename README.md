# Data-Science-mini-projects
A collection of data science mini-projects covering Python fundamentals, data cleaning, EDA, ML basics, feature engineering, time series, geospatial features, and deep learning

## Projects

Each folder is a self-contained mini-project with its own README (and notebooks / code)

### Python & Data
- **[01_python_foundations](./01_python_foundations)** - Python basics: syntax, data structures, functions, small practice tasks
- **[02_python_data_cleaning](./02_python_data_cleaning)** - cleaning pipelines: missing values, outliers, type fixes, duplicates, basic validation
- **[03_python_data_visualization](./03_python_data_visualization)** - EDA & visualization: distributions, correlations, categorical plots, chart styling

### Machine Learning
- **[04_ml_from_baseline_to_random_forest](./04_ml_from_baseline_to_random_forest)** - baseline - improved models (e.g., linear/logistic models, trees, random forest), evaluation & comparison
- **[05_end_to_end_ml_pipeline](./05_end_to_end_ml_pipeline)** - end-to-end workflow: preprocessing, train/val/test split, pipelines, metrics, reproducibility
- **[06_feature_engineering](./06_feature_engineering)** - feature creation & selection: encoding, scaling, interactions, leakage checks, feature importance

### Time series & Geospatial
- **[07_time_series_linear_regression](./07_time_series_linear_regression)** - time series basics: lag features, train/test split by time, simple forecasting with regression
- **[08_geospatial_feature_engineering](./08_geospatial_feature_engineering)** - geospatial features: distances, clustering/regions, coordinate transforms, location-based features

### Classification (Non-linear) & Deep Learning
- **[09_nonlinear_classification](./09_nonlinear_classification)** - non-linear classifiers (e.g., trees/ensembles), decision boundaries, metrics, error analysis
- **[cnn_generalization_project](./cnn_generalization_project)** - CNN generalization: training, regularization, augmentation, confusion matrix & error analysis on image data

## Tech stack
- Python, Jupyter Notebook  
- NumPy, pandas  
- Matplotlib / (optionally) Seaborn  
- scikit-learn  
- (Deep learning) TensorFlow / Keras (project-dependent)


## Repository structure

This repo contains multiple independent mini-projects  
Most projects are kept simple and include only a notebook + a short README:  
- `project_name/`
- `project_notebook.ipynb`
- `README.md`


Some projects may also include additional folders:  
- `data/` - local datasets (often not tracked if large)
- `results/` - saved figures, metrics, model artifacts
- `requirements.txt` - project-specific dependencies
