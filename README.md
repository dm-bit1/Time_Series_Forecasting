Time_Series_Forecasting

Background and Overview
This project was motivated by my interest in the stock market and machine learning predictions. The Mplfinance 
library was used a lot in this project to create custom visualizations of historical stock prices,
because it is designed for finacial assets. It provides better visuals for stock prices than Matplotlib. 
It generates stock charts similar to those used by popular websites, e.g. bigcharts.com, yahoofinance.com. 
Another thing I implemented is machine learning, because
of the it's powerful ability to predict. 
As it relates to machine learning, the PyTorch library has high-level 
models and it requires an understanding of how to train the models, test the models, use appropriate 
weights, use the right time steps in testing and training, normalization, optimizers, plotting the loss 
function, etc. All of those tasks were done in this project.

Machine Learning Methodology
The predictions used a custom LSTM in PyTorch in Python. The code used 2000 epochs and the model got 
more accurate as the number of epochs increased when tested. The train and test split used was 80% and 20%,
respectively. This means that 2023 included 250 trading days and 200 days were used to train the model
and 50 days were used to test the model. The test and actual values can be seen in a plot called NFLX stock in 2023
with blue and green lines. There is also a plot called Loss using RMSE that shows the loss after each 100
epochs which shows decline that resembles an exponential decay. This implies that the model trained 
a lot better with more epochs. There may be a diminishing return at some point as it relates to the number of epochs used.

Data Structure Overview
The historical stock data was obtained using the Yahoo Fiance API.
The data represents trading days with start = "2023-01-01", end = "2023-12-31". Then, it was wrangled using Pandas Dataframes. 
This was necessary preparation to training the machine learning models ultimately using a custom PyTorch LSTM I created and I used some source code to guide me through the machine
learning process. The column names are visible in a cell in the Jupyter Notebook.
There are plots which show several different time views to display different data granularity.
E.g. 1 year period with 1 day intervals, 5 day period with 1 minute intervals, 1 day period with 1 minute intervals, 

Executive Summary
The regression model was able to generate somewhat accurate stock price predictions. It slightly lagged behind on days
where there was a large fluctuation in price as is seen on in a plot. The model actually predicted lower
prices for most of the days which could indicate it was a bull market.

Recommendations

Credit

This link trained me on how to use an LSTM in PyTorch. 

https://machinelearningmastery.com/lstm-for-time-series-prediction-in-pytorch/
