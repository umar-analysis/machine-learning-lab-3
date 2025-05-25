# machine-learning-lab-3
Objective
The objective of this lab is to gain a basic understanding of the Python libraries Pandas and NumPy, their features, and how to perform basic operations using them for data analysis and numerical computation.

Introduction
Pandas and NumPy are two of the most important Python libraries used for data science, analysis, and numerical computing.

NumPy (Numerical Python) is a fundamental package for numerical computations in Python. It provides support for arrays, matrices, and a collection of mathematical functions to operate on these data structures efficiently.

Pandas is built on top of NumPy and provides high-level data structures and methods designed to make data analysis fast and easy. Its primary data structures are Series (one-dimensional labeled array) and DataFrame (two-dimensional labeled data structure similar to tables in a database or Excel spreadsheets).

Materials and Tools
Python 3.x

Jupyter Notebook or any Python IDE (like VSCode, PyCharm)

Installed libraries: pandas, numpy

Procedure
Part 1: NumPy Basics
Import the NumPy library:



import numpy as np
Create NumPy arrays:


arr1 = np.array([1, 2, 3, 4, 5])
arr2 = np.array([[1, 2], [3, 4]])
Basic operations on arrays:


print(arr1 + 5)            # Add 5 to each element
print(arr2 * 2)            # Multiply each element by 2
print(np.sqrt(arr1))       # Square root of each element
print(np.mean(arr1))       # Calculate mean
print(arr1.shape)          # Shape of the array
Array slicing and indexing:


print(arr1[2:4])           # Elements from index 2 to 3
print(arr2[:, 1])          # All rows, column 1
Part 2: Pandas Basics
Import the Pandas library:

import pandas as pd
Create a Pandas Series:


data = pd.Series([10, 20, 30, 40, 50], index=['a', 'b', 'c', 'd', 'e'])
print(data)
Create a Pandas DataFrame:


data_dict = {
    'Name': ['Ali', 'Sara', 'John', 'Emma'],
    'Age': [25, 30, 35, 28],
    'City': ['Karachi', 'Lahore', 'Islamabad', 'Peshawar']
}

df = pd.DataFrame(data_dict)
print(df)
Accessing DataFrame elements:

print(df['Name'])          # Access a column
print(df.loc[1])           # Access row by label
print(df.iloc[2])          # Access row by position
Basic DataFrame operations:


print(df.describe())       # Summary statistics
print(df.head(2))          # First 2 rows
print(df.tail(2))          # Last 2 rows
Observations
NumPy arrays provide fast, efficient ways to handle numerical data.

Pandas DataFrames are ideal for handling and analyzing tabular data with labeled rows and columns.

Both libraries are highly optimized for data processing tasks and provide intuitive syntax for operations.

Conclusion
This lab introduced the basics of NumPy and Pandas, two essential libraries for data analysis and scientific computing in Python. Understanding these libraries helps simplify complex data manipulation tasks and prepares us for more advanced data science projects.
