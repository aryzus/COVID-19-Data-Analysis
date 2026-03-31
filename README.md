# COVID-19-Data-Analysis
This project uses Python and Pandas to analyze COVID-19 cases, deaths, and recoveries.   Visualizations highlight daily trends, country comparisons, and recovery vs death analysis.





# COVID-19 Data Analysis

## Overview
This project uses Python and Pandas to analyze COVID-19 cases, deaths, and recoveries.  
Visualizations highlight daily trends, country comparisons, and recovery vs death analysis.

## Features
- Daily cases trend line chart
- Deaths vs recoveries comparison
- Top 10 countries by cases
- Cleaned dataset with missing values handled

## Tools
- Python
- Pandas, Matplotlib, Seaborn
- Kaggle COVID-19 dataset

## Files
- `covid_analysis.ipynb` → Jupyter Notebook
- `README.md` → Documentation






Starter Notebook (covid_analysis.ipynb)

import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load dataset
df = pd.read_csv("covid.csv")
df['date'] = pd.to_datetime(df['date'])

# Daily cases trend
plt.figure(figsize=(10,6))
sns.lineplot(x="date", y="cases", data=df)
plt.title("Daily COVID-19 Cases Trend")
plt.show()

# Deaths vs Recoveries
df_group = df.groupby("country")[["deaths","recoveries"]].sum().reset_index()
df_group.head(10).plot(x="country", kind="bar", figsize=(12,6))
plt.title("Top Countries - Deaths vs Recoveries")
plt.show()
