# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 07-03-2025
### Name : Keerthana P

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
import pandas as pd
import matplotlib.pyplot as plt

df=pd.read_csv('bank_train.csv')
df.shape

df1=df.head(100)
df1
```

![image](https://github.com/user-attachments/assets/31a0cc34-2b1b-4234-ab8f-484bf1aebdac)

![image](https://github.com/user-attachments/assets/1cff6874-a509-4991-b63c-b6ecccce3335)




```
x=df1['precipitation']
y=df1['temp_max']

plt.figure(figsize=(10, 6))
plt.bar(x,y)
plt.title('Precipitation vs Max temp')
plt.xlabel('Precipitation')
plt.ylabel('Max temp')
plt.grid(True)
plt.show()

```





# OUTPUT:

![image](https://github.com/user-attachments/assets/80a121c6-3cb3-4618-a4d6-57f7a20669b9)







# RESULT:
Thus we have created the python code for plotting the time series of given data.
