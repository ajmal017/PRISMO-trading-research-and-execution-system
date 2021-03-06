# PRISMO-trading-research-and-execution-system
Fully automated trading platform. Backtesting module created for efficient model testing and creation, execution system to trade the system live. Feel free to contact me with any questions !


# Live Execution System 
Built upon ib_insync (wrapper for interactive brokers API), allows multiple independent strategies to be run within a single TWS session.



![Alt text](executionPlatform.gif?raw=true "Title")


Note that the above is an example of the strategy running at the end of day, on a paper trading account with delayed market data. 

A GUI developed for strategy tracking and visualisation and test case verification.

![Alt text](execution.gif?raw=true "Title")


# Backtesting System
Platform to backtest strategies, with two main components:
  - Optimizer
  - Bias removed backtest

The optimizer is the 'efficient' code, that finds optimum parameters for the strategies being researched. The bias removal backtester tries to remove as much: look-ahead, survivorship and sample size bias. This is achieved via a multitude of methods, including monte carlo simulation, real-time trading simulation and AI to parse data from multiple sources. The code implements multiprocessing. It outputs a range of heuristics for model evaluation. Below is a sample of results generated by the bias removal system. 


![Alt text](results.jpg?raw=true "Title")

As so far, the strategies tested are:
  - LSTM forecasting spread of triplets
  - Kalman filter pairs 
  - HMM regeime detection models
  - Double EMA smoothing pairs
 
 

