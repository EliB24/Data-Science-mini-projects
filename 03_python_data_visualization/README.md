# Sales Data Visualization
This project focuses on visual analysis and aims to explore and interpret sales data through visualization.
The main goal is to transform raw tabular data into clear and informative graphs that reveal patterns, trends, and relationships in the data.

---

## Project overview

The dataset contains information about customer orders, including:

- Order ID  
- Sales amount  
- Profit  
- Quantity  
- Product category and subcategory  
- Payment method  
- Order date  
- Location (state and city)

The goal of the project is to answer simple questions using visualization:

- How do sales and profit change over time?  
- Which categories and subcategories are the most popular?  
- Which states and cities generate the most orders?  
- How are payment methods distributed?  
- How are amount, profit, and quantity related?

There are the types of charts that are used to answer these questions:

- Line charts  
- Bar charts  
- Histograms with density plots  
- Pie charts  
- Heat maps  
- Correlation matrix

---

## Files Included

- **03_python_data_visualization.ipynb** — main Jupyter Notebook with all visualizations  
- **Sales Dataset.csv** — input dataset  
- **README.md** — project description  

---

## Technologies Used

- **Python 3**  
- **pandas** — data manipulation  
- **matplotlib** — basic plotting  
- **seaborn** — statistical visualizations  
- **Jupyter Notebook / JupyterLab**

---

## Key Insights from Visualizations

- **Category Distribution**
Orders are evenly distributed across categories, with a slight preference for furniture.
This is followed by office supplies and electronics, with little difference between categories. This indicates a diverse demand for products.
- **Sub-Category Distribution**
Orders are distributed across many subcategories, but no single subcategory stands out enough to account for the majority of the data.
- **State and City Distribution**
New York and California have the highest number of orders among the states.
At the city level, demand is distributed across many cities, without any extreme differences.
- **Payment Mode Distribution**
Payment methods are evenly distributed. Debit Card and Credit Card are the most common, followed closely by UPI.
COD and EMI are less frequent but still significant.
- **Sales & Profit by Category**
All three categories (electronics, furniture, and office supplies) show relatively similar sales and profit levels.
This may indicate that the business is balanced across categories and not dependent on any one of them.
- **Sales & Profit by Sub-Category**
Some products, such as tables, markers, and electronic games, generate much higher sales than others, while many subcategories remain in the middle range.
Profits typically grow along with the sales, but not to the same level for all products.
This shows that high sales do not always mean high profits and that some subcategories are more profitable than others.
- **Monthly Trends**
Sales and profits fluctuate significantly over time, with several sharp peaks.
Profits generally follow sales, but not proportionally, indicating a difference in margins between months.
- **Distributions (Histograms with KDE)**
The amount varies widely, but most orders are relatively small. Large amounts are less common.

Profits are mostly low, with only a few very high values. This creates a long "tail" on the right side of the graph.

The quantity is limited to a small range (1–20 units per order) and is distributed quite evenly, with no obvious peaks or dominant values.
- **Sales by State and Category**
Different states lead in different categories (Texas in Electronics, California in Furniture, New York in Office Supplies).
There is no single state dominating all categories.
- **Correlation Analysis**
Amount and Profit: moderate positive correlation (0.68).

Quantity and Amount, Quantity and Profit: near zero correlation.
Profit is driven by sales value rather than by the number of items sold.

---

## How to Run

1. Open `03_python_data_visualization.ipynb` in Jupyter Notebook or JupyterLab  
2. Make sure all required libraries are installed  
3. Run the cells from top to bottom  
