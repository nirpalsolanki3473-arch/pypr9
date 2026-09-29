# 📊 Sales Data Analyzer & Visualization

A beginner-friendly **Python data analysis and visualization project** that allows users to load a CSV dataset, explore and clean data, perform calculations, generate statistics, create visualizations, and perform common Pandas and NumPy operations through an interactive menu-driven program.

---

## 🚀 Project Overview

**Sales Data Analyzer** is a menu-driven Python application built to practice and demonstrate important concepts of:

* Python
* Object-Oriented Programming (OOP)
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Data Cleaning
* Data Analysis
* Data Visualization

The project uses a `SalesDataAnalyzer` class to organize different data analysis operations into separate methods.

The user can load a CSV file and perform different operations without manually writing individual analysis commands every time.

---

## 🎯 Objectives

The main objectives of this project are:

* Load sales data from a CSV file.
* Explore the structure and contents of a dataset.
* Perform arithmetic operations on DataFrame columns.
* Handle missing values.
* Generate descriptive statistics.
* Sort, search, and filter data.
* Perform aggregate calculations.
* Perform group-by analysis.
* Create pivot tables.
* Combine multiple DataFrames.
* Convert Pandas columns into NumPy arrays.
* Generate different types of visualizations.
* Save generated visualizations as image files.
* Practice Python OOP concepts in a practical data-analysis project.

---

## 🛠️ Technologies Used

| Technology                | Purpose                                           |
| ------------------------- | ------------------------------------------------- |
| Python                    | Main programming language                         |
| Pandas                    | Data loading, cleaning, manipulation and analysis |
| NumPy                     | Numerical operations and array handling           |
| Matplotlib                | Data visualization                                |
| Seaborn                   | Statistical visualization                         |
| Jupyter Notebook / Python | Development environment                           |
| GitHub                    | Project hosting and version control               |

---

## 📦 Python Libraries

The project uses the following libraries:

```text
pandas
numpy
matplotlib
seaborn
```

Install the required libraries using:

```bash
pip install pandas numpy matplotlib seaborn
```

---

## 📂 Project Structure

A simple project structure can look like this:

```text
Sales-Data-Analyzer/
│
├── SalesDataAnalyzer.ipynb
├── dataset.csv
├── README.md
└── visualizations/
```

> The dataset filename can be different depending on the CSV file being analyzed.

---

## ✨ Features

### 1. Load Dataset

The program allows the user to enter the path of a CSV file.

The dataset is loaded using Pandas:

```python
pd.read_csv()
```

The loaded DataFrame is stored in:

```text
self.df
```

---

### 2. Explore Data

The project provides basic dataset exploration options:

* Display first 5 rows
* Display last 5 rows
* Display column names
* Display data types
* Display basic DataFrame information

Methods/functions used include:

```text
head()
tail()
columns
dtypes
info()
```

---

### 3. DataFrame Operations

The program allows arithmetic operations between two DataFrame columns.

Supported operations:

* Addition
* Subtraction
* Multiplication
* Division

For example:

```text
Column A + Column B
Column A - Column B
Column A * Column B
Column A / Column B
```

This helps demonstrate Pandas Series operations.

---

### 4. Handle Missing Data

The project provides options for handling missing values.

Available operations:

* Display rows containing missing values
* Fill missing values using the mean
* Drop rows containing missing values
* Replace missing values with a user-defined value

Pandas functions used include:

```text
isnull()
fillna()
dropna()
```

---

### 5. Descriptive Statistics

The program can generate statistical information about the dataset.

Available operations include:

* `describe()`
* Standard deviation
* Variance
* Percentile / Quantile

Functions used include:

```text
describe()
std()
var()
quantile()
```

---

### 6. Data Visualization

The project provides multiple visualization options using Matplotlib and Seaborn.

Supported charts include:

#### Bar Plot

Used to compare values between categories.

```text
plt.bar()
```

#### Line Plot

Used to visualize trends.

```text
plt.plot()
```

#### Scatter Plot

Used to show relationships between two numerical variables.

```text
plt.scatter()
```

#### Pie Chart

Used to display proportions.

```text
plt.pie()
```

#### Histogram

Used to understand the distribution of numerical data.

```text
plt.hist()
```

#### Stack Plot

Used to visualize how multiple values change over an x-axis.

```text
plt.stackplot()
```

#### Box Plot

Used to visualize the distribution of numerical data and identify potential outliers.

```text
sns.boxplot()
```

#### Heatmap

Used to visualize correlations between numerical columns.

```text
sns.heatmap()
```

---

### 7. Sort Data

The project allows the user to sort the DataFrame using a selected column.

The project uses:

```text
sort_values()
```

The current implementation sorts data in ascending order.

---

### 8. Search Data

The search feature allows the user to find rows where a selected column matches a specific value.

It uses Pandas filtering with a condition such as:

```text
DataFrame[column] == value
```

---

### 9. Filter Data

The filtering feature allows users to filter numerical data based on:

* Greater than
* Less than
* Equal to

For example:

```text
Sales > 500
Sales < 500
Sales == 500
```

This demonstrates Boolean filtering in Pandas.

---

### 10. Aggregate Operations

The project supports aggregation on a selected numerical column.

Available operations:

* Sum
* Mean
* Median

Functions used:

```text
sum()
mean()
median()
```

---

### 11. GroupBy Analysis

The project allows users to group data using a category column and perform calculations on a numerical column.

Supported calculations:

* Sum
* Mean
* Median

Example concept:

```text
Group by Category → Calculate Sales Mean
```

This demonstrates the Pandas:

```text
groupby()
```

function.

---

### 12. Pivot Table

The project provides a pivot-table feature using Pandas.

A user can select:

* Index
* Column
* Values

The project uses:

```text
pd.pivot_table()
```

This helps summarize data across multiple categories.

---

### 13. Multiple Subplots

The project creates multiple charts in a single figure using Matplotlib subplots.

The current implementation creates a `2 × 2` layout containing:

* Line plot
* Horizontal bar plot
* Bar plot
* Scatter plot

This demonstrates:

```text
plt.subplots()
```

---

### 14. Combine DataFrames

The project provides three ways to combine data:

#### Concatenation

Combines DataFrames vertically.

```text
pd.concat()
```

#### Join

Combines DataFrames based on their indexes.

```text
DataFrame.join()
```

#### Merge

Combines DataFrames using a common column.

```text
pd.merge()
```

---

### 15. NumPy Operations

The project also converts a selected Pandas column into a NumPy array.

It supports:

* Maximum value
* Minimum value
* Average value
* Indexing
* Slicing

NumPy functions/methods demonstrated include:

```text
np.array()
max()
min()
mean()
```

The project also demonstrates NumPy indexing and slicing.

---

### 16. Save Visualization

Generated plots can be saved using a user-provided filename.

Example:

```text
scatter_plot.png
```

The project uses:

```text
plt.savefig()
```

This allows users to save charts for later use.

---

## 🧭 Main Menu

The application provides the following menu:

```text
1. Load Dataset
2. Explore Data
3. Perform DataFrame Operations
4. Handle Missing Data
5. Generate Descriptive Statistics
6. Data Visualization
7. Sort
8. Search
9. Filter
10. Aggregate
11. Group By
12. Save Visualization
13. Pivot Table
14. Subplots
15. Add DataFrame
16. NumPy
17. Exit
```

---

## 🧱 OOP Concept Used

The project is organized using a Python class:

```text
SalesDataAnalyzer
```

The class contains different methods responsible for different operations.

Examples include:

```text
load_data()
explore_data()
operation()
missing()
Statistics()
Visualization()
sd()
sch()
flt()
agg()
gb()
ptable()
splot()
add()
nump()
```

The object is created using:

```text
SalesDataAnalyzer()
```

This structure makes the project easier to organize and extend.

---

## 🔄 Program Workflow

The general workflow of the application is:

```text
Start
  ↓
Create SalesDataAnalyzer Object
  ↓
Load CSV Dataset
  ↓
Explore Dataset
  ↓
Clean / Handle Missing Data
  ↓
Perform DataFrame Operations
  ↓
Analyze Data
  ↓
Generate Statistics
  ↓
Create Visualizations
  ↓
Save Visualization
  ↓
Continue Analysis or Exit
```

---

## 📊 Example Analysis Tasks

After loading a sales dataset, the application can be used for tasks such as:

* Find the highest value in a numerical column.
* Find the minimum value.
* Calculate the average.
* Calculate the total sales.
* Calculate median sales.
* Find records above a specific sales value.
* Find records below a specific value.
* Group sales by category.
* Calculate average sales for each category.
* Sort records by sales.
* Search for a specific category.
* Analyze correlations between numerical columns.
* Create sales charts.
* Save charts as image files.

---

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Sales-Data-Analyzer.git
```

### 2. Open the project

Open the project folder in:

* VS Code
* Jupyter Notebook
* JupyterLab

### 3. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn
```

### 4. Run the project

If using Jupyter Notebook:

```text
Open SalesDataAnalyzer.ipynb
```

Run the notebook cells and start the program.

### 5. Load a CSV file

When the program asks:

```text
enter the path of the dataset (CSV file):
```

provide the path to your CSV dataset.

Example:

```text
sales.csv
```

---

## 🧪 Sample Dataset Columns

The project can work with a sales dataset containing columns such as:

```text
Date
Product
Category
Region
Quantity
Sales
Profit
```

The exact column names depend on the CSV file provided by the user.

---

## 📚 Concepts Practiced

This project combines several Python and data-analysis concepts:

### Python

* Variables
* Conditional statements
* Loops
* Functions
* Exception handling
* User input
* Classes and objects
* Methods

### Object-Oriented Programming

* Class
* Object
* Constructor
* Instance attributes
* Instance methods

### Pandas

* DataFrame
* Series
* CSV reading
* Data selection
* Filtering
* Sorting
* Missing-value handling
* Aggregation
* GroupBy
* Pivot tables
* Merge
* Join
* Concatenation

### NumPy

* Arrays
* Indexing
* Slicing
* Mathematical operations
* Aggregation

### Matplotlib

* Bar chart
* Line chart
* Scatter plot
* Pie chart
* Histogram
* Stack plot
* Subplots
* Saving figures

### Seaborn

* Box plot
* Heatmap

---

## 🎓 Learning Outcome

This project helped demonstrate how Python can be used for practical data analysis.

After completing the project, the user can practice:

* Loading real-world datasets
* Understanding DataFrames
* Cleaning missing data
* Performing calculations
* Filtering and sorting data
* Summarizing information
* Finding relationships between variables
* Creating visualizations
* Using NumPy with Pandas
* Applying OOP to a data-analysis application

---

## 🔮 Future Improvements

Possible improvements for future versions include:

* Add a graphical user interface.
* Add automatic data-type validation.
* Add better error handling for invalid column names.
* Add more visualization types.
* Add customizable chart titles and axis labels.
* Add automatic detection of numerical and categorical columns.
* Export analysis results to CSV or Excel.
* Add interactive dashboards.
* Add date-based sales analysis.
* Add automatic sales and profit reports.
* Improve input validation.
* Add unit tests.
* Separate the project into multiple Python modules.

---

## ⚠️ Current Limitations

This is an **MVP / learning project**, so some operations depend on the user entering valid column names and compatible data.

For example:

* Arithmetic operations require suitable numerical columns.
* Some filtering operations currently expect numerical input.
* Visualization options require appropriate column types.
* The CSV path must be valid.
* The dataset should contain columns suitable for the selected operation.

---

## 👨‍💻 Project Status

**Status:** MVP / Learning Project

The project is functional and demonstrates core Python data-analysis concepts. It can be extended with better validation, error handling, reporting, and a graphical interface.

---

## 📌 Key Highlights

```text
✔ CSV Dataset Loading
✔ Data Exploration
✔ Data Cleaning
✔ Missing Value Handling
✔ Arithmetic Operations
✔ Descriptive Statistics
✔ Sorting
✔ Searching
✔ Filtering
✔ Aggregation
✔ GroupBy Analysis
✔ Pivot Tables
✔ DataFrame Concatenation
✔ DataFrame Join
✔ DataFrame Merge
✔ NumPy Operations
✔ Multiple Visualizations
✔ Subplots
✔ Correlation Heatmap
✔ Save Visualizations
✔ Object-Oriented Programming
```

---

## 📄 License

This project is created for **learning and educational purposes**.

You are free to use and modify the project for learning, practice, and personal projects.

# 👨‍💻 Author

**Nirpalsinh Solanki**
