# Ex03-Univariate-Analysis
# Aim:
  To read the given data and perform the univariate analysis with different types of plots.

# Explanation:
 Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for  univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# Algorithm
# Step1
 Read the given data.

# Step2
 Get the information about the data.

# Step3
 Remove the null values from the data.

# Step4
 Mention the datatypes from the data.

# Step5
 Count the values from the data.

# Step6
 Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program:
```
Developed by : D.R.Vinuthna
Registration Number : 212221230017

```
```
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)

```
# Output
###  DATA 
 ![output](https://github.com/VINUTHNA-2004/Ex03-Univariate-Analysis/blob/main/1.png?raw=true)

### DATA HEAD 
 ![output](https://github.com/VINUTHNA-2004/Ex03-Univariate-Analysis/blob/main/2.png?raw=true)

### DATA INFORMATION
 ![output](https://github.com/VINUTHNA-2004/Ex03-Univariate-Analysis/blob/main/3.png?raw=true)

### DATA DESCRIBE
 ![output](https://github.com/VINUTHNA-2004/Ex03-Univariate-Analysis/blob/main/4.png?raw=true)

### DATA NULL VALUES
 ![output](https://github.com/VINUTHNA-2004/Ex03-Univariate-Analysis/blob/main/5.png?raw=true)

### DATA'S DATATYPES
 ![output](https://github.com/VINUTHNA-2004/Ex03-Univariate-Analysis/blob/main/6.png?raw=true)

### DATA'S VALUECOUNT
  ![output](https://github.com/VINUTHNA-2004/Ex03-Univariate-Analysis/blob/main/7.png?raw=true)

### BOXPLOT
 ![output](https://github.com/VINUTHNA-2004/Ex03-Univariate-Analysis/blob/main/8.png?raw=true)

### COUNTPLOT
 ![output](https://github.com/VINUTHNA-2004/Ex03-Univariate-Analysis/blob/main/9.png?raw=true)

### DISTRIBUTION PLOT
 ![output](https://github.com/VINUTHNA-2004/Ex03-Univariate-Analysis/blob/main/10.png?raw=true)

### HISTOGRAM PLOT
 ![output](https://github.com/VINUTHNA-2004/Ex03-Univariate-Analysis/blob/main/11.png?raw=true)
 
# Result
 Thus we have read the given data and performed the univariate analysis with different types of plots.
