# 🐼 Python Pandas DataFrame – Part 1

This repository contains my practice and learning work on **Pandas DataFrames** in Python.

The goal of this repository is to build a strong foundation in Pandas by working with DataFrames, CSV datasets, indexing, selecting data, filtering, sorting, and basic data manipulation.

---

## 📌 About Pandas

**Pandas** is a powerful Python library used for **data manipulation and data analysis**.

It provides two major data structures:

- **Series** – One-dimensional labeled data
- **DataFrame** – Two-dimensional tabular data with rows and columns

This repository mainly focuses on **DataFrames**.

---

## 🎯 Purpose of This Repository

The main objectives of this repository are:

- Understand Pandas DataFrames
- Learn how to create DataFrames
- Work with CSV datasets
- Understand rows and columns
- Select and filter data
- Practice indexing and slicing
- Sort DataFrame data
- Create and modify columns
- Understand different data types
- Build practical Pandas problem-solving skills

---

## 📚 Topics Covered

### 1. DataFrame Basics

- Importing Pandas
- Creating a DataFrame
- Creating DataFrames from dictionaries
- Creating DataFrames from lists
- Understanding rows and columns
- Understanding DataFrame index

### 2. Data Inspection

Important methods and attributes:

```python
df.head()
df.tail()
df.shape
df.columns
df.index
df.dtypes
df.info()
```

These are useful for understanding the structure of a dataset before performing analysis.

---

### 3. Selecting Data

Practice with:

```python
df["column"]
df[["column1", "column2"]]
```

Selecting specific rows and columns from a DataFrame.

---

### 4. Indexing with `loc` and `iloc`

#### `loc`

Used for **label-based selection**.

```python
df.loc["row_label"]
```

#### `iloc`

Used for **integer-position-based selection**.

```python
df.iloc[0]
df.iloc[0:5]
```

---

### 5. Filtering Data

Filtering rows based on conditions:

```python
df[df["marks"] > 80]
```

Multiple conditions can also be used:

```python
df[(df["marks"] > 80) & (df["age"] < 25)]
```

---

### 6. Sorting Data

Sorting DataFrames:

```python
df.sort_values("marks")
```

Descending order:

```python
df.sort_values("marks", ascending=False)
```

Sorting by multiple columns:

```python
df.sort_values(
    ["city", "unit_price"],
    ascending=[True, False]
)
```

---

### 7. Creating and Updating Columns

Creating new columns from existing data:

```python
df["total_amount"] = df["quantity"] * df["unit_price"]
```

Updating existing columns:

```python
df["marks"] = df["marks"] + 5
```

---

### 8. Working with Data Types

Checking data types:

```python
df.dtypes
```

Changing a column's data type:

```python
df["ID"] = df["ID"].astype("Int32")
```

---

### 9. CSV Data

The repository includes CSV data for practicing DataFrame operations.

Reading a CSV file:

```python
import pandas as pd

df = pd.read_csv("file.csv")
```

After loading the dataset, basic inspection can be performed using:

```python
df.head()
df.shape
df.columns
df.info()
```

---

## 🗂️ Repository Contents

```text
Python_Pandas_DataFrame_Part1
│
├── csv/
│   └── Dataset files
│
├── basic1.ipynb
│   └── Pandas DataFrame practice
│
└── README.md
```

---

## 🛠️ Technologies Used

- Python 🐍
- Pandas 🐼
- Jupyter Notebook
- CSV

---

## 💻 Installation

Make sure Python is installed on your system.

Install Pandas:

```bash
python3 -m pip install pandas
```

For Jupyter Notebook:

```bash
python3 -m pip install notebook
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Then open:

```text
basic1.ipynb
```

---

## 🚀 Learning Approach

I am following a hands-on approach:

1. Learn the concept
2. Write the code myself
3. Practice with datasets
4. Solve problems
5. Debug errors
6. Repeat the concepts
7. Build stronger DataFrame manipulation skills

The focus is on **writing code and solving problems rather than only reading theory**.

---

## 📈 Learning Roadmap

This repository is part of my Python Data Science learning journey.

```text
Python
   ↓
NumPy
   ↓
Pandas Series
   ↓
Pandas DataFrame
   ↓
Data Cleaning
   ↓
Data Analysis
   ↓
Matplotlib
   ↓
Seaborn
   ↓
SQL
   ↓
Machine Learning
```

---

## 🎯 Future Topics

After completing DataFrame fundamentals, I plan to continue with:

- Data Cleaning
- Missing Values
- GroupBy
- Aggregation
- Merge
- Join
- Concatenation
- Pivot Tables
- Date & Time
- Advanced Data Analysis
- Matplotlib
- Seaborn
- SQL
- Machine Learning

---

## 👨‍💻 Author

**Prathmesh Surwase**

Computer Engineering Student | Python | Pandas | Data Science & Machine Learning

---

## ⭐ Repository

GitHub:

`Python_Pandas_DataFrame_Part1`

If you find this repository useful, feel free to ⭐ the repository.

---

### 🐼 Keep Learning, Keep Practicing, Keep Building!

> **Consistency + Practice + Problem Solving = Strong Data Science Foundation**
