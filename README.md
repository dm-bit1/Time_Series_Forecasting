# Time_Series_Forecasting
Introduction

I added this to the README file because I wanted a reason to write something in Nano in Git Bash.

This project was motivated by my interest in the stock market. There is a large community of day traders

and software is required to enable these traders to trade. This is a helpful activity in the context of the economy

because it provides liquidity to the markets. I became aware of the Mplfinance library which is designed for finacial

instruments. It is more targeted than Matplotlib itself to that end. I wanted to see how the charts that can be generated

using the library compare to websites frequently used by traders to view stock charts. E.g. bigcharts.com, yahoofinance.com.

Another thing I wanted to implement is machine learning because of the powerful forecasting it can generate. The accuracy of 

a model can be measured with a testing dataset. I wanted to gain some experience in applied machine learning using PyTorch which

is not an easy task. I researched some simple and effective methods of applied machine learning and decided I wanted to use

an LSTM in PyTorch. Why use an LSTM? Because, it uses a recurrent neural network under the hood. That means the network feeds data back into itself

in order to learn the patterns in the dataset over each epoch. In theory, it should perform superiorly for a regression task such as time series forecasting.

The normalization step in the machine learning was skipped because it was a simple example. In reality,

the normalization step could be important because it can remove patterns from the data which can reduce overfitting. This project was not 

an exercise in data science because there is no hypothesis to test against. It was an exercise in programming and applied machine

learning to gain some practice and familiarity.

Conclusion

The Mplfinance library turns out some pretty high quality candlestick plots with customizability. 

It compares pretty favorable to Bigcharts and Yahoo Finance. As it relates to machine learning, it is a

difficult discipline to master because of the complexity of machine learning algorithms. Even with the PyTorch

library that has high-level models, it still requires an understanding of how to train the models, test the models, 

use appropriate weights, use the right time steps in testing and training, normalization, optimizers, 

plotting the loss function, etc.
