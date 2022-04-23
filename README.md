# Automated Algorithmic Trading Bot with Machine Learning

This is the 2nd Project from our SMU Fintech Bootcamp.

  <p align="center">
  <img 
    width="700"
    height="337"
    src="https://i.postimg.cc/BQHD8T2c/algorithmic-trading-bot.jpg)](https://postimg.cc/BXZtk1YX"
  >
</p>

## What We're Creating
We are creating an automated algorithmic trading bot. We will use machine learning within the trading bot to buy and sell stocks based on different technical analysis indicators. We will also utilize the input function in python to ask our user which stock they would like to trade. We will backtest our algorithmic trading bot against historical market data.

## What is Algorithmic Trading?
Algorithmic trading is a process for executing orders utilizing automated and pre-programmed trading instructions to account for variables such as price, timing and volume. An algorithm is a set of directions for solving a problem. Computer algorithms send small portions of the full order to the market over time. ([Investopedia](https://www.investopedia.com/terms/a/algorithmictrading.asp#:~:text=Algorithmic%20trading%20is%20a%20process,to%20the%20market%20over%20time.))

## Usage & Installation
We will be working out of Jupyter Lab and importing the following libraries into our notebook:

 <p align="left">
  <img 
    width="500"
    height="300"
    src="https://i.postimg.cc/bwRZF78y/2022-04-23-1.png)](https://postimg.cc/TKp2KHpF"
  >

## Gathering Our Data
We begin by importing a csv file with a list of the S&P 500 companies, we will use this as a reference for our input question.

  
Next we will ask our user which stock they would like to trade from the S&P500, their answer must be in ticker format (eg. 'AAPL').
  [![image.png](https://i.postimg.cc/288LQpPs/image.png)](https://postimg.cc/QVwMDzNm) 
  

Their answer will then be used to tell our Alpaca API which stocks data to retrieve. Now we are ready to begin genrating our trading signals. 
  
## Generating Our Trading Signals
Next we will need to tell our trading bot when to buy, hold and sell. We will do this by generating trading signals using short-window and long-window SMAs with RSI values.
  [![Screen-Shot-2022-04-19-at-2-42-13-PM.png](https://i.postimg.cc/d1NPgyVm/Screen-Shot-2022-04-19-at-2-42-13-PM.png)](https://postimg.cc/G8D5y9YH)
  
We will plot our entry and exit points.
  [![image-1.png](https://i.postimg.cc/k4pzTPTT/image-1.png)](https://postimg.cc/342twV5G)
  
## Machine Learning Models
We will now use our two machine learning models to make predictions about our data. These models are the Support Vector Classifier (SVC) model and the AdaBoost model. 

The code to fit these models is pretty much the same but the results will vary as seen from our classification reports for each model. 
  
  [![Ada-Boost.png](https://i.postimg.cc/Xq3J8LhG/Ada-Boost.png)](https://postimg.cc/dkHwQ2Jw) 
  
  [![SVM.png](https://i.postimg.cc/kGnJ846W/SVM.png)](https://postimg.cc/sQNCC3J2)
  
By plotting our results we can see our actual returns vs our strategy returns. 
  
  ADA Plot:
  
[![Ada-Boost-Chart.png](https://i.postimg.cc/bYW8p3LQ/Ada-Boost-Chart.png)](https://postimg.cc/nM4N1Kyz)
  
  SVM Plot:
  
[![SVM-Chart.png](https://i.postimg.cc/Zn7LzW6c/SVM-Chart.png)](https://postimg.cc/RJttcVs6)
  
## Conclusion 
Our bot does its job properly. We did find that the AdaBoost machine learning method is much more accurate than the SVM method based on our precision and accuracy results that you can see in the classification report. This is the method we would recommend using for building your own algorithmic trading bot. 
  

## Contributors
[Omar Eid](https://github.com/ORE93)

[Alex Morales](https://github.com/Amora987)

[Thomas Cloud](https://github.com/beowulf888)

[James Tagapan](https://github.com/trekj)
