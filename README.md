# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date:12/08/2025 

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
Name:Dhivya Dharshini B
Reg No: 212223240031
import pandas as pd
import matplotlib.pyplot as plt
file_path = 'gold_price_data.csv'
data = pd.read_csv(file_path)
data['Date'] = pd.to_datetime(data['Date'])
data.set_index('Date', inplace=True)
plt.figure(figsize=(10, 6))
plt.plot(data.index, data['Value'], label='Values', color='blue')
plt.title('Values over Date')
plt.xlabel('Date')
plt.ylabel('Values')
plt.grid(True)
plt.legend()
plt.show()
```










# OUTPUT:



<img width="1003" height="614" alt="image" src="https://github.com/user-attachments/assets/5b0d938b-84e5-41fb-9dee-c7f716feeee6" />



# RESULT:
Thus we have created the python code for plotting the time series of given data.
