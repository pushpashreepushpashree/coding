import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
import numpy as np
df = pd.DataFrame({
    "STATE": ["KARNATAKA", "DELHI", "HYDERABAD", "TAMIL NADU", "MAHARASHTRA"],
    "YEAR": [2012, 2015, 2014, 2006, 2018],
    "median_income": [1201, 15021,2013, 20133,2206]
})
plt.figure(figsize=(6,3))
sns.heatmap(df.set_index('STATE'),annot=True,cmap='viridis',fmt='g')
plt.title('heatmap')
plt.xlabel('year')
plt.ylabel('median_income')
plt.show()
