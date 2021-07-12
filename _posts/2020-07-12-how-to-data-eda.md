# Practicing Data EDA
## Table of Contents
1. [Missing Data](#missing-data)
2. 


<hr/>

### 1. Missing Data

<p>
  In order to process missing data, first you want to find it. Do the following in python shell.<br/>
  
- finding missing data: 1) import pandas and numpy (to install 'pip install pandas' in CLI-commandline interface-, same with numpy)<br/>
  2) if you have the dataset(named df in this article) ready, 
  
  ```{.python}
  len(df)-df.count             # you can either do this
  
  df.isnull()                  # or this (check if the data is missing
  df[df.isnull().any(axis=1)]  # and then show any line with missing data)
  ```

- replacing missing data
  
  ```
  df.replace
  df.fillna
  ```
  
  comes handy. <Keep in mind> if you want to replace the data in dataframe, give option: "inplace=True".
