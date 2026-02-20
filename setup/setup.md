# 📊 Data Analysis Starter

This guide helps you load and inspect data quickly using Python.

### 🏃 Quick Start Command
To run this analysis, copy the code block below and run it in your Python environment. GitHub will provide a **Copy** button in the top-right corner:

```python
import pandas as pd

# Load a sample dataset
url = "[https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv)"
df = pd.read_csv(url)

# Display the first 5 rows and data types
print("--- Header Preview ---")
print(df.head())

print("\n--- Column Info ---")
print(df.info())