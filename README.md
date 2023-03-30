# Ex03-Univariate-Analysis
# Aim:

To read the given data and perform univariate analysis.

# Algorithm:

# Step 1:

Read the given Data

# Step 2:

Get the information about the data

# Step 3:

Get the data types of the each column

# Step 4:

Get the counts of unique values of each attribute in the dataset.

# Step 5:

Get the description of the data

# Step 6:

Perform graphical analysis and print the distribution of quantitative data using boxplots,countplots,Descriptive Statistics techniques and histograms for each columns in the dataset.

# Code:

import pandas as pd

import seaborn as sns

data1=pd.read_csv('/content/SuperStore.csv')

data1.head()

# statistical analysis

data1.info()

data1.dtypes

data1['Postal Code'].value_counts()

data1['Sales'].value_counts()

data1.describe()

# Graphical analysis

# 1)Box Plots

sns.boxplot(x="Postal Code",data=data1)

sns.boxplot(x="Sales",data=data1)

# 2)Count Plots

sns.countplot(x="Postal Code",data=data1)

sns.countplot(x="Sales",data=data1)

# 3)Descriptive Statistics techniques

sns.distplot(data1["Postal Code"])

sns.distplot(data1["Sales"])

# 4)Histograms

sns.histplot(x="Postal Code",data=data1)

sns.histplot(x="Sales",data=data1)

# Output:
<img width="886" alt="image" src="https://user-images.githubusercontent.com/87276633/228901275-42313dfa-7fa2-43d2-b18a-f07b8abd64d5.png">
<img width="280" alt="image" src="https://user-images.githubusercontent.com/87276633/228903359-e347bd2d-a204-4b9a-8ea6-3d5cd59afb49.png">
<img width="168" alt="image" src="https://user-images.githubusercontent.com/87276633/228901583-3bc1a2fb-0399-426b-b0ec-a0bc08cfb957.png">
<img width="275" alt="image" src="https://user-images.githubusercontent.com/87276633/228901799-63ca228b-6d1b-4292-9d01-9e24089bb475.png">
<img width="251" alt="image" src="https://user-images.githubusercontent.com/87276633/228901855-4c51aa3c-36e6-44a8-85e3-be2b53b9c7e7.png">
<img width="287" alt="image" src="https://user-images.githubusercontent.com/87276633/228908243-00e6c2b8-4192-49d6-b6be-9f3e39cb4be0.png">
<img width="320" alt="image" src="https://user-images.githubusercontent.com/87276633/228904166-33e7891f-7735-481f-8683-630cbe60254b.png">
<img width="321" alt="image" src="https://user-images.githubusercontent.com/87276633/228904231-c9311148-c6a2-4fe1-aefd-8454700f565c.png">
<img width="323" alt="image" src="https://user-images.githubusercontent.com/87276633/228904369-cf68eb1a-8c91-4366-866d-2fabaec8b2fa.png">
<img width="351" alt="image" src="https://user-images.githubusercontent.com/87276633/228904421-200a5b38-0483-464b-a6aa-6ece92d3717c.png">
<img width="414" alt="image" src="https://user-images.githubusercontent.com/87276633/228909359-9b179954-7292-450c-8ee0-cf1d7fe25bf0.png">
<img width="428" alt="image" src="https://user-images.githubusercontent.com/87276633/228907941-54025006-f13f-426f-a71b-518c50b08d94.png">
<img width="310" alt="image" src="https://user-images.githubusercontent.com/87276633/228904733-ad12f295-9a59-4bbc-803c-738f201f4d50.png">
<img width="308" alt="image" src="https://user-images.githubusercontent.com/87276633/228904825-f958eb33-2889-4f0d-b4f8-6d0f88d8caae.png">

# Result:

Thus the univariate analysis for the given data is performed successfully.






