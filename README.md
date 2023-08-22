# EXP-1-Plot-a-time-series-data
## AIM:
Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
## ALGORITHM:
1. Import the required packages like pandas and numpy

2. Read the data using the pandas

3. Calculate the mean for the respective column.

4. Plot the data according to need and can be altered monthly, or yearly.

5. Display the results.
## PROGRAM:
```
import matplotlib.pyplot as plt
import pandas as pd
df=pd.read_csv("Dataset.csv",parse_dates=["Date"],index_col="Date")
df.head()
df["2022-01"]
df["2022-01"].Close.mean()
df["2022-04-01":"2022-07-31"]
df.Close.resample('M').mean()
mean=df.Close.resample('M').mean().plot(kind="bar")
mean=df.Close.resample('Y').mean().plot(kind="bar")
```
## OUTPUT:
 ## FIRST FIVE ROWS: 
![image](https://github.com/swethamohanraj/EXP-1-Plot-a-time-series-data/assets/94228215/737ead23-b2ac-4325-bc15-dea95499990d)

## CALCULATING MEAN:
![image](https://github.com/swethamohanraj/EXP-1-Plot-a-time-series-data/assets/94228215/4a848290-1ab5-45c4-82ee-2c31205f942d)

## PLOTTING BAR GRAPH(MONTHLY):
![image](https://github.com/swethamohanraj/EXP-1-Plot-a-time-series-data/assets/94228215/fbf5823a-9155-45d6-a936-c2bb54b84c63)

## PLOTING BAR GRAPH(YEARLY):
![image](https://github.com/swethamohanraj/EXP-1-Plot-a-time-series-data/assets/94228215/bfbc6f55-ea6e-4c60-8b5f-dfce4b2d1678)

## RESULT:
Thus we have created the python code for plotting the time series of given data
