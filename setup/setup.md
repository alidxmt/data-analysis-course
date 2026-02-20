import pandas as pd

# Load a sample dataset
url = "https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv"
df = pd.read_csv(url)

# Display the first 5 rows and data types
print("--- Header Preview ---")
print(df.head())

print("\n--- Column Info ---")
print(df.info())