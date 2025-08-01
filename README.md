# PRODIGY_DS_01

## Task 1: Data Visualization (Bar Chart & Histogram)

In this task, I worked with the **World Bank Population Dataset** (provided by Prodigy Infotech) to visualize population data using Python.

### What I did
- Created a **Bar Chart** showing the **Top 10 most populated countries in 2020**.
- Created a **Histogram** showing the **distribution of populations across all countries in 2020**.

### Tools Used
- Python  
- Pandas  
- Matplotlib  
- Seaborn  

### Dataset
World Bank Population Dataset (`SP.POP.TOTL`)  
Source: [World Bank Open Data](https://data.worldbank.org/indicator/SP.POP.TOTL)

### Outcome
Through this task, I learned how to:
- Import and clean CSV data with Pandas.  
- Select specific columns (population in 2020).  
- Create meaningful visualizations (bar chart & histogram) with Matplotlib and Seaborn.  

### Example Code Snippet
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load dataset (skip first 4 rows as metadata)
df = pd.read_csv("API_SP.POP.TOTL_DS2_en_csv_v2_38144.csv", skiprows=4)

# Bar chart: Top 10 countries by population (2020)
top_countries = df[['Country Name', '2020']].sort_values(by='2020', ascending=False).head(10)
plt.figure(figsize=(10,6))
sns.barplot(x='2020', y='Country Name', data=top_countries, palette="viridis")
plt.title("Top 10 Countries by Population (2020)")
plt.xlabel("Population")
plt.ylabel("Country")
plt.show()

# Histogram: Distribution of populations (2020)
plt.figure(figsize=(8,6))
sns.histplot(df['2020'].dropna(), bins=30, kde=True, color="skyblue")
plt.title("Distribution of Country Populations (2020)")
plt.xlabel("Population")
plt.ylabel("Number of Countries")
plt.show()
