# Pandas in 10

**What is Pandas?** Pandas is built on top of two core Python libraries—matplotlib for data visualization and NumPy for mathematical operations. Pandas acts as a wrapper over these libraries, allowing you to access many of matplotlib's and NumPy's methods with less code. For instance, pandas' .plot() combines multiple matplotlib methods into a single method, enabling you to plot a chart in a few lines.
(credit: https://mode.com/python-tutorial/libraries/pandas/)

To manually store data in a table, create a DataFrame. When using a Python dictionary of lists, the dictionary keys will be used as column headers and the values in each list as columns of the DataFrame. (credit: https://pandas.pydata.org/)

- Dataframe - a 2-dimensional data structure that can store data of different types (including characters, integers, floating point values, categorical data and more) in columns. It is similar to a spreadsheet, a SQL table or the data.frame in R.

To handle pandas remember the following:

- Import the package, aka import pandas as pd

- A table of data is stored as a pandas DataFrame

- Each column in a DataFrame is a Series

- You can do things by applying a method to a DataFrame or Series

- Object Creation - By passing a list of values, letting pandas create a default integer index example:

s = pd.Series([1, 3, 5, np.nan, 6, 8])

s
Out[4]:
0    1.0
1    3.0
2    5.0
3    NaN
4    6.0
5    8.0
dtype: float64`
