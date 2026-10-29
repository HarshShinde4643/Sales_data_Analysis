# Sales Data Analytics

## Project Overview
This project uses Python to analyze sales transactions, product categories, and customer demographics. It applies data inspection, data-quality checks, date formatting, exploratory data analysis (EDA), and visualizations to identify patterns in revenue and profit.

## Project Objective
The objective is to analyze sales data to understand:
- Customer age distribution
- Sales revenue distribution
- Product assortment across categories
- Revenue contribution by product category
- The relationship between unit price and profit
- Which product categories generate the most revenue

## Skills and Tools
- Python
- Pandas
- NumPy
- Data cleaning and preprocessing
- Missing-value and duplicate checks
- Exploratory Data Analysis (EDA)
- Data visualization with Matplotlib and Seaborn
- Business insight generation

## Dataset
The notebook loads three CSV files:

 `data/sales.csv` 
 `data/products.csv` 
 `data/customers.csv` 




## Project Workflow

### 1. Load the Data
Load the sales, products, and customers datasets using Pandas.

### 2. Inspect the Data
Review dataset shapes, column names, data types, and descriptive statistics.

### 3. Check Data Quality
- Check each dataset for missing values.
- Check for duplicated rows.
- The notebook records that no missing values or duplicate rows were found.

### 4. Format Dates
- Convert `customers.join_date` to datetime using `%Y-%m-%d`.
- Convert `sales.order_date` to datetime using `%d-%m-%Y`.

### 5. Exploratory Data Analysis and Visualizations


## Key Findings
The findings below reflect the interpretations written in the notebook:

- **Customer ages:** Customers span a broad age range, approximately 18–70 years, with an average age of about 44 years.
- **Sales revenue distribution:** Most transactions are described as generating lower-to-middle revenue, with high-revenue transactions occurring less frequently.
- **Product assortment:** Praline has the largest number of products in the catalog; Milk chocolate has the smallest.
- **Revenue share:** Praline contributes approximately 27.4% of revenue, followed by White chocolate at approximately 24.2%. Dark chocolate contributes approximately 20.7%, Truffle 15.0%, and Milk chocolate 12.7%.
- **Unit price and profit:** The notebook observes a generally positive relationship between unit price and profit. This is an association, not proof that increasing price alone causes profit to rise.
- **Category revenue comparison:** The bar chart compares total revenue by category; the tallest bar indicates the highest-revenue category.

## How to Run the Project

1. Clone or download this repository.
2. Ensure the project has the following structure:

   ```text
   .
   ├── Sales_Data_Analytics.ipynb
   ├── README.md
   └── data/
       ├── sales.csv
       ├── products.csv
       └── customers.csv
   ```

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

4. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `Sales_Data_Analytics.ipynb` and run the cells in order.

> If your notebook has a different filename, use that actual filename in the repository and when opening it.

## Limitations
- The notebook performs exploratory analysis and visualization; it does not train a predictive model.
- The scatter plot shows association between unit price and profit, not causation.
- The reported category revenue percentages should be interpreted as revenue contribution, not profit contribution.
- Business decisions should also consider costs, discounts, quantities, and profit margins.

## Conclusion
This project demonstrates a basic sales analytics workflow using Pandas, NumPy, Matplotlib, and Seaborn. It checks data quality, formats date columns, and visualizes customer ages, revenue distribution, product assortment, category revenue, and the relationship between unit price and profit. The results provide a starting point for further analysis of sales performance and profitability.
