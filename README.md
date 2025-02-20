# Big Basket Data Analysis

## Project Overview
The **Big Basket Data Analysis** project involves exploring and analyzing a dataset containing information about various products sold on Big Basket. The dataset includes details such as product names, categories, subcategories, brands, market prices, sale prices, ratings, and product descriptions.

The goal of this project is to gain insights into product sales, pricing trends, discounts, and customer ratings through data analysis techniques using **Python**.

---

## Dataset Information
The dataset contains **27,555 records** across **10 columns**:

- **index**: Unique identifier for each product
- **product**: Name of the product
- **category**: Main category under which the product is listed
- **sub_category**: Sub-category of the product
- **brand**: Brand name of the product
- **sale_price**: Selling price of the product
- **market_price**: Original market price of the product
- **type**: Further classification of the product
- **rating**: Customer rating of the product (1-5 scale)
- **description**: Detailed description of the product

---

## Steps Performed in Analysis

### 1. Data Loading
- The dataset is loaded into a **Pandas DataFrame** for analysis.
- `head()` function is used to view the first 12 records.

### 2. Data Exploration
- `describe()` is used to generate statistics such as mean, median, min, max, and standard deviation.
- `info()` function helps understand the structure and data types of each column.

### 3. Finding Most & Least Sold Products
- Used `value_counts()` to determine the most and least sold products.
- Identified that **Turmeric Powder** is the most sold product, while many products have been sold only once.

### 4. Category Analysis
- The most sold category is **Beauty & Hygiene**, while the least sold category is **Eggs, Meat & Fish**.

### 5. Discount Calculation
- A new column `Discount` is created to compute the difference between `market_price` and `sale_price`.
- Another column `Discount%` calculates the percentage discount.

### 6. Handling Missing Values
- Used `isna().sum()` to find missing values in columns.
- Missing values in `sale_price` were filled using `market_price` values.
- Missing ratings were interpolated using the `linear` method.

### 7. Identifying Outliers
- Used statistical methods to detect outliers in pricing and ratings.
- Outliers were treated by replacing them with mean values where necessary.

---

## Tools & Libraries Used
- **Python**
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Matplotlib & Seaborn**: Data visualization
- **Plotly**: Interactive visualizations

---

## Key Findings
- The most sold products belong to categories like **Beauty & Hygiene** and **Gourmet & World Food**.
- Significant price variations exist between `market_price` and `sale_price`, with some products receiving high discounts.
- Many products have missing ratings, which may impact customer buying decisions.
- Data cleaning and outlier treatment were necessary to ensure data integrity.

---

## Future Scope
- Build a predictive model to estimate product ratings based on price and category.
- Conduct sentiment analysis on product descriptions.
- Identify seasonal trends in product sales.

---


---

## Author
Gurpreet Singh Virk
*Data Enthusiast | Python Developer | Data Analyst*  


---

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

