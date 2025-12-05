Clean raw warehouse inventory data and generate basic beginner-friendly visualizations to understand patterns in price, quantity, category, and warehouse distribution.

🧹 1. Data Cleaning Steps:-
The following steps were performed in Warehouse_cleaning.ipynb:
✔️ 1. Load the dataset
Used pandas.read_csv() to load messy_data.csv.
✔️ 2. Understand basic structure
df.head()
df.info()
df.describe()

Check column names:-
✔️ 3. Handle Missing Values
Identified missing values using:
df.isnull().sum()
Filled missing numeric values (Price, Quantity) using mean.
Filled missing text values (Category, Warehouse) using mode.

✔️ 4. Fix Data Types:-
Converted Price to float
Converted Quantity to integer
Ensured Warehouse and Category are strings

✔️ 5. Handle Duplicates:-
Checked duplicates
df.duplicated().sum()
Removed duplicates

✔️ 6. Clean Text Columns:-
Removed leading/trailing spaces
Converted categories to title case
Standardized warehouse codes

✔️ 7. Save the Cleaned Dataset
Exported using:-
df.to_csv("cleaned_data.csv", index=False)
📊 2. Visualizations (Beginner Friendly)
All graphs were plotted using Matplotlib.
📌 1. Bar Chart – Category vs Average Price
Shows which product category is most expensive.
📌 2. Line Chart – Price Trend by Product ID
Simple numeric comparison of product prices.
📌 3. Histogram – Price Distribution
To understand how prices are spread.
📌 4. Pie Chart – Warehouse Distribution
Shows data stored across different warehouses.

🛠️ 3. Technologies Used:-
Python 3
Pandas
Matplotlib
Jupyter Notebook

▶️ 4. How to Run This Project:-
Step 1 — Clone the Repository
git clone <your-repo-link>
Step 2 — Install Dependencies
pip install pandas matplotlib
Step 3 — Open the Notebook
jupyter notebook Warehouse_cleaning.ipynb
Step 4 — Run All Cells
The outputs will show cleaned data and graphs.

📝 5. Results:-
✔️ Cleaned dataset free of missing values, duplicates, and incorrect types
✔️ Simple visualizations to understand warehouse inventory
✔️ Beginner-friendly Python code for data cleaning
