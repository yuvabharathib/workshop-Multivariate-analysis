# workshop-Multivariate-analysis
# Aim
To perform Multivariate EDA on the given data set.

# Explanation 
Exploratory data analysis is used to understand the messages within a dataset. This technique involves many iterative processes to ensure that the cleaned data is further sorted to better understand the useful meaning.The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.

# Algorithm
# Step1
Import the built libraries required to perform EDA and outlier removal.

# Step2
Read the given csv file.

# Step3
Convert the file into a dataframe and get information of the data.

# Step4
Return the objects containing counts of unique values using (value_counts()).

# Step5
Plot the counts in the form of Histogram or Bar Graph.

# Step6
Use seaborn the bar graph comparison of data can be viewed.

# Step7
Find the pairwise correlation of all columns in the dataframe.corr()

# Step8
Save the final data set into the file.

# Types of bivariate analyis
1)Numerical & Numerical(Scatter plot)

2)Numerical & Categorical(Bar plot,Box plot,Dist plot)

# Code
```
Developed by : YUVABHARATHI.B
Registration Number : 212222230181
import pandas as pd
import numpy as py
import seaborn as sns
import matplotlib.pyplot as plt

df=pd.read_csv('FlightInformation (1).csv')
sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])
df.head()
df.info()
df.describe()
df.isnull().sum()
df.dtypes

sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])
sns.barplot(x=df['Dep_Time'],y=df['Price'],data=df)
df.corr()
```

Output
# Data Head:
![image](https://user-images.githubusercontent.com/113497404/229035838-ee4b9f93-18f8-4b2c-95d0-7b41932564a9.png)

# Data Information
![image](https://user-images.githubusercontent.com/113497404/229036009-f1570977-63c7-436e-97af-6b1a2ebfe616.png)

# Numerical & Numerical(Scatter plot)
![image](https://user-images.githubusercontent.com/113497404/229036119-35d5923a-ff0c-44d1-b32d-1527dc5d4480.png)

# Numerical & Categorical(Bar plot)
![image](https://user-images.githubusercontent.com/113497404/229036287-a4da1363-e6ef-401c-ac60-52c037479795.png)

# Non-Graphical method(correlation)
![image](https://user-images.githubusercontent.com/113497404/229036362-5fa07e95-68c7-4dc0-8b8a-fcb3f42a2887.png)

# Result
Thus we have performed Multivariate EDA on the given data set.

