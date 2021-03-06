# Bitcoin-Price-Prediction
Bitcoin Price Prediction using AI and yahoo Finance data

# Libraries
import re
import json
import csv
from io import StringIO
from bs4 import BeautifulSoup
import requests

# Data from Yahoo Finance - Daily 5 years 
btc_history = 'https://query1.finance.yahoo.com/v7/finance/download/BTC-USD?period1=1457222400&period2=1614988800&interval=1d&events=history&includeAdjustedClose=true'

# Parameters
params = {
    'range' : '5y',
    'interval' : '1w',
    'events' : 'history'
}

# show first 5 rows to check the output 
file = StringIO(response.text)
reader = csv.reader(file)
data = list(reader)
for row in data[:5]:
    print(row)
    
    
