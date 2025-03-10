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
```p
import pandas as pd
import matplotlib.pyplot as plt

df=pd.read_csv('seattle-weather.csv')
df.shape

df1=df.head(100)
df1
```

![image](https://github.com/user-attachments/assets/31a0cc34-2b1b-4234-ab8f-484bf1aebdac)



![image](https://github.com/user-attachments/assets/1cff6874-a509-4991-b63c-b6ecccce3335)


```
df.info()
```


![image](https://github.com/user-attachments/assets/aada704d-fdfd-43bb-a53d-693eed627957)


```
df.describe()
```

![image](https://github.com/user-attachments/assets/4415ff5a-67e1-4342-b308-205e210aa691)


```p
x=df['precipitation']
y=df['temp_max']

plt.figure(figsize=(10, 6))
plt.bar(x,y)
plt.title('Precipitation vs Max temp')
plt.xlabel('Precipitation')
plt.ylabel('Max temp')
plt.grid(True)
plt.show()

```





# OUTPUT:

![image](https://github.com/user-attachments/assets/5f355d16-1e35-4654-9aae-c191f606fc24)








# RESULT:
Thus we have created the python code for plotting the time series of given data.
