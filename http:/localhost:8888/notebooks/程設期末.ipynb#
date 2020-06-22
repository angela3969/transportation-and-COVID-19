import pandas as pd
import matplotlib.pyplot as plt
import matplotlib.ticker as ticker
from IPython.core.pylabtools import figsize
import pylab as pl
plt.xticks(rotation =60)
Data=pd.read_csv("AirlineAndCase.csv")
Date=Data["日期"]
DailyEntry=Data["Entry"]
DailyExit=Data["Exit"]
CaseAddNum=Data["cases"]

Airline = plt.gca() 
Airline.plot(Date,DailyEntry,color="dodgerblue",label="總入境人數")
Airline.plot(Date,DailyExit,color="orange",label="總出境人數")

Airline.set_title("出入境人數與境外確診數之比較")
Airline.set_ylabel("出入境人數")
Airline.set_xlabel("日期")
plt.rcParams["font.sans-serif"] = ["Arial Unicode MS"] 

ticker_spacing =5
Airline.xaxis.set_major_locator(ticker.MultipleLocator(ticker_spacing))
plt.figure(figsize(40,10))

plt.show()
