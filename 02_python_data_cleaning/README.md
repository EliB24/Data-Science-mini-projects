# Cafe Sales Data Cleaning 

This project demonstrates how to clean and prepare a messy real-world sales dataset using Python.
The original data contains missing values, invalid entries, and inconsistent formats.
The goal of this project is to turn raw cafe transaction data into a clean, analysis-ready dataset.

---

## Project Overview

In this project, I worked with a cafe sales dataset that includes:

- Item names
- Quantity sold
- Price per unit
- Total spent
- Payment method
- Location
- Transaction date

The main focus is data cleaning and preparation, not modeling or prediction.
Key tasks include:

- Converting columns to correct data types
- Handling missing and invalid values
- Restoring values using logical relationships between columns
- Filling missing quantities using median statistics
- Separating usable and non-usable records
- Checking and reporting overall data quality

---

## Files Included

- **02_python_data_cleaning.ipynb** — main Jupyter Notebook with all cleaning steps

- **dirty_cafe_sales.csv** — raw input dataset

- **README.md** — project description

---

## Data Cleaning Summary

During the cleaning process:

- Invalid text values like "ERROR" and "UNKNOWN" are replaced with missing values
- Numeric columns are safely converted to numbers
- Missing prices and totals are restored using mathematical relationships
- Missing quantities are filled using median values at different grouping levels
- Rows that cannot be reliably restored are identified and kept separate
- Quantity is fully restored, while some categorical fields remain partially missing

All decisions are made to avoid unrealistic assumptions and preserve data integrity.

---

## Technologies Used

- **Python 3**
- **pandas**
- **NumPy**
- **Jupyter Notebook / JupyterLab**

 ---

## How to run
1. Open the `.ipynb` file in Jupyter Notebook or JupyterLab  
2. Run all cells sequentially  


