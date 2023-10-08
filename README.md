# PRODIGY_DS_01


import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load the CSV file into a Pandas DataFrame


df = pd.read_csv(r'C:\Users\Computers\Desktop\bank-full.csv', delimiter=';')

# Visualize the distribution of a categorical variable (e.g., 'marital')
sns.countplot(x='marital', data=df)
plt.title('Distribution of Marital Status')
plt.show()
# Visualize the distribution of a continuous variable (e.g., 'age') with a histogram
plt.hist(df['age'], bins=20, edgecolor='black')
plt.title('Distribution of Ages')
plt.xlabel('Age')
plt.ylabel('Count')
plt.show()
