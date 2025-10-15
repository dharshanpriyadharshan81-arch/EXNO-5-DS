# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
 import pandas as pd
import matplotlib.pyplot as plt
import numpy as np


data = pd.DataFrame({
    'Year': [2018, 2019, 2020, 2021, 2022],
    'Sales': [150, 200, 250, 300, 350],
    'Profit': [20, 30, 50, 60, 80],
    'Region': ['North', 'South', 'East', 'West', 'Central']
})


plt.figure(figsize=(8, 5))
plt.plot(data['Year'], data['Sales'], marker='o', label='Sales')
plt.plot(data['Year'], data['Profit'], marker='s', label='Profit')
plt.title('Sales and Profit Over Years')
plt.xlabel('Year')
plt.ylabel('Amount')
plt.legend()
plt.grid(True)
plt.show()


plt.figure(figsize=(8, 5))
plt.bar(data['Year'], data['Sales'], color='skyblue')
plt.title('Annual Sales')
plt.xlabel('Year')
plt.ylabel('Sales')
plt.show()

# Horizontal Bar Chart
plt.figure(figsize=(8, 5))
plt.barh(data['Region'], data['Sales'], color='orange')
plt.title('Sales by Region')
plt.xlabel('Sales')
plt.ylabel('Region')
plt.show()


plt.figure(figsize=(6, 6))
plt.pie(data['Sales'], labels=data['Region'], autopct='%1.1f%%', startangle=140)
plt.title('Sales Distribution by Region')
plt.show()


plt.figure(figsize=(8, 5))
plt.scatter(data['Sales'], data['Profit'], color='green')
plt.title('Profit vs Sales')
plt.xlabel('Sales')
plt.ylabel('Profit')
plt.grid(True)
plt.show()


plt.figure(figsize=(8, 5))
plt.hist(data['Sales'], bins=5, color='purple', edgecolor='black')
plt.title('Sales Distribution')
plt.xlabel('Sales')
plt.ylabel('Frequency')
plt.show()


plt.figure(figsize=(8, 5))
plt.boxplot([data['Sales'], data['Profit']], labels=['Sales', 'Profit'])
plt.title('Box Plot of Sales and Profit')
plt.show()


plt.figure(figsize=(8, 5))
plt.stackplot(data['Year'], data['Sales'], data['Profit'], labels=['Sales', 'Profit'], colors=['#1f77b4', '#ff7f0e'])
plt.title('Area Plot of Sales and Profit')
plt.xlabel('Year')
plt.ylabel('Amount')
plt.legend(loc='upper left')
plt.show()


plt.figure(figsize=(6, 5))
correlation = data[['Sales', 'Profit']].corr()
plt.imshow(correlation, cmap='coolwarm', interpolation='none')
plt.colorbar()
plt.xticks([0, 1], ['Sales', 'Profit'])
plt.yticks([0, 1], ['Sales', 'Profit'])
plt.title('Correlation Heatmap')
plt.show()

#output:
<img width="1034" height="593" alt="Screenshot 2025-10-15 140753" src="https://github.com/user-attachments/assets/85c69b29-7456-450e-949e-61cc7c898e79" />
<img width="1057" height="581" alt="Screenshot 2025-10-15 140819" src="https://github.com/user-attachments/assets/5fe745e1-f0ce-4e64-8867-c0dc664cfd5e" />
<img width="1058" height="590" alt="Screenshot 2025-10-15 140837" src="https://github.com/user-attachments/assets/3f85c48b-8e91-47ab-87d9-29b3a4b49c36" />
<img width="870" height="599" alt="Screenshot 2025-10-15 140847" src="https://github.com/user-attachments/assets/266fa3e2-cf66-4d85-ad0f-5d12e24a9aa0" />
<img width="1127" height="584" alt="Screenshot 2025-10-15 140900" src="https://github.com/user-attachments/assets/616ea5d1-fbf9-4823-af3c-9d3b0d44a97a" />
<img width="1052" height="595" alt="Screenshot 2025-10-15 140920" src="https://github.com/user-attachments/assets/d8d9285b-c97e-47e0-a165-87b8bb2e21c0" />
<img width="1052" height="595" alt="Screenshot 2025-10-15 140920" src="https://github.com/user-attachments/assets/8d251e60-11ea-40ff-9c8e-800cb15888a4" />
<img width="982" height="595" alt="Screenshot 2025-10-15 140958" src="https://github.com/user-attachments/assets/22b1d156-4a83-4b13-84e0-58fb7bd97e57" />
<img width="926" height="570" alt="Screenshot 2025-10-15 141014" src="https://github.com/user-attachments/assets/5266310e-cde5-43c7-b19c-f33fe7d7c24d" />

# Result:
The above code and output and result is To Perform Data Visualization using matplot python library for the given datas.
