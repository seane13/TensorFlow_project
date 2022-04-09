# project2
AlgoTrading

## Manual Algorythm -vs- Machine learning Algorythm for stock trading¶

The goal of this project is to compare a simple stock trading algorythm to a TensorFlow machine learning algorythm.

### Manual Algorythm 

The manual algo analyzes a stock over the course of the past year to determine the best entry and exit points moving forward with a shorter term long only strategy. In the manual algo, I will use 2 technical analysis indicators (Bollinger Bands and Exponential Moving Averages) to determine entry and exit points. I will then visualize and backtest my algo.

### TensorFlow Algorythm

Building the model consisted of determining the best features, scaler, and Tensor parameters. I then backtested the ML model and compared to the Manual model

### Automatic Order

Finally, I set up the Alpaca Trade API order to enter and exit trades when I run the program.

## imports and installs

import os
import requests
import pandas as pd
from pandas.tseries.offsets import DateOffset
import numpy as np
from dotenv import load_dotenv
import alpaca_trade_api as tradeapi
from alpaca_trade_api.rest import REST, TimeFrame
from alpaca_trade_api.entity_v2 import BarsV2
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import MinMaxScaler, StandardScaler
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import LSTM, Dense, Dropout
from finta import TA
from sklearn import svm
from sklearn.metrics import classification_report
import hvplot.pandas
from pathlib import Path
import matplotlib.pyplot as plt
from numpy.random import seed
from tensorflow import random
%matplotlib inline

### Setting these options will allow for reviewing more of the DataFrames
pd.set_option("display.max_rows", 2000)
pd.set_option("display.max_columns", 2000)
pd.set_option("display.width", 1000)


## Conclusion

Both models have proven to be profitable. The manual model uses fewer trades but, has a higher ROI.
The TensorFlow model is more active while producing more profit in less time. 

Both models require a mix of art and science to fine tune.