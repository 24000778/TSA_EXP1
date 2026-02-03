# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 02/02/2026
### 212224040319

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

df=pd.read_csv('/content/Tesla Dataset.csv')
df.shape

df1=df.head(100)
df1

```

<img width="746" height="707" alt="image" src="https://github.com/user-attachments/assets/c1e97c2c-e11a-4964-ac87-eab52dabfa3d" />

```

df.info()

```

<img width="772" height="373" alt="image" src="https://github.com/user-attachments/assets/879a5234-d581-4712-9db3-1e005786ab9c" />

```

df.describe()

```

<img width="376" height="274" alt="image" src="https://github.com/user-attachments/assets/4b28673b-49b1-4cfd-bb83-4b6a60b397ef" />

```

x=df1['Date']
y=df1['Open']

plt.figure(figsize=(10,6))
plt.bar(x,y)
plt.grid(True)
plt.title('Date vs Open')
plt.xlabel('Date')
plt.ylabel('Open')
plt.show()


```



# OUTPUT:


<img width="1155" height="707" alt="image" src="https://github.com/user-attachments/assets/d6817a29-0eb6-4856-a60d-e9aab1d1628f" />


    
    
This is not stationary





# RESULT:
Thus we have created the python code for plotting the time series of given data.
