# project2
AlgoTrading

## Manual Algorythm -vs- Machine learning Algorythm for stock trading¶

The goal of this project is to compare a simple stock trading algorithm to a TensorFlow machine learning algorythm.

### Manual Algorithm 

The manual algo analyzes a stock over the course of the past year to determine the best entry and exit points moving forward with a shorter term long only strategy. In the manual algo, I will use 2 technical analysis indicators (Bollinger Bands and Exponential Moving Averages) to determine entry and exit points. I will then visualize and backtest my algo.

### TensorFlow Algorithm

Building the model consisted of determining the best features, scaler, and Tensor parameters. I then backtested the ML model and compared to the Manual model


### Automatic Order

Finally, I set up the Alpaca Trade API order to enter and exit trades when I run the program.


### Summary

Both models have proven to be profitable. The manual model uses fewer trades but, has a higher ROI.
The TensorFlow model is more active while producing more profit in less time. 

Both models require a mix of art and science to fine tune.

### Conclusion
Although the algorithm is simple in nature, this project served as an introduction to TensorFlow and possibly a template for future projects.
