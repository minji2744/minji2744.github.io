# Practicing Data EDA
## Table of Contents (keep updating)
1. [Missing Data](https://minji2744.github.io/how-to-data-eda/#1-missing-data)
2. Duplicated Data
3. 
4. EDA Example (with kaggle Titanic)


<hr/>

### 1. Missing Data

  In order to process missing data, first you want to find it. Do the following in python shell.<br/>
  
- finding missing data <br/>
  1) import pandas and numpy (to install 'pip install pandas' in CLI-commandline interface-, same with numpy)<br/>
  2) if you have the dataset(named df in this article) ready, 
  
  ```
  len(df)-df.count             # you can either do this
  
  df.isnull()                  # or this (check if the data is missing
  df[df.isnull().any(axis=1)]  # and then show any line with missing data)
  ```

- replacing missing data <br/>
  Say, you want to replace NaN to ""(empty space).
  
  ```
  df.replace(np.nan, "", inplace=True)
  df.fillna("", inplace=True)
  ```
  
  Above methods come handy. Keep in mind. If you want to replace the data in dataframe, give option: "inplace=True".
  
<br/>
  
### 98. EDA Example (with kaggle Titanic)
* short description: predicting whether Titanic's passenger survived.
* How to: 

### 99. Examining each columns
