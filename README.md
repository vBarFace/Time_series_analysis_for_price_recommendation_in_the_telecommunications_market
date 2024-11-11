# Time Series Analysis for Price Recommendation in the Telecommunications Market

## Overview

This project focuses on forecasting prices for a given product in the telecommunications market by applying different time series forecasting models. Various models were implemented and tested, including Recurrent Neural Networks (RNN), Long Short-Term Memory (LSTM) networks (univariate and multivariate), Gated Recurrent Units (GRU), ARIMA, SARIMA, and Facebook Prophet.

## Authors

- **André Reis Fernandes**  
  MSc. Computational Engineering  
  Department of Electronics, Telecommunications and Informatics  
  Email: [andre.fernandes16@ua.pt](mailto:andre.fernandes16@ua.pt)   

- **Gonçalo Jorge Loureiro de Freitas**  
  MSc. Computational Engineering  
  Department of Electronics, Telecommunications and Informatics  
  Email: [goncalojfreitas@ua.pt](mailto:goncalojfreitas@ua.pt)  

## Supervisor

- **Prof. Sónia Gouveia**  
  Email: sonia.gouveia@ua.pt [petia@ua.pt](mailto:petia@ua.pt)

## Abstract

This project implements and compares several time series forecasting models to predict prices in the telecommunications market. Models applied include:
- **RNN**
- **Univariate and Multivariate LSTM**
- **GRU**
- **ARIMA**
- **SARIMA**
- **Facebook Prophet**

The ARIMA(3, 1, 0) model or its SARIMA counterpart [(3, 1, 0), (0, 0, 0, 0), 'n'] was found to be the best performing model, with the following evaluation metrics:
- MAPE: 0.04
- MSE: 12.164
- MAE: 0.831 (ARIMA)
- MAPE: 0.04
- MSE: 12.174
- MAE: 0.833 (SARIMA)

## Models Used

### 1. Recurrent Neural Network (RNN)
RNNs are designed for time series data, where the model "remembers" previous inputs. The RNN learns from the previous outputs and uses them as input for the current step.


### 2. Long Short-Term Memory (LSTM)
LSTMs overcome the vanishing gradient problem of traditional RNNs, making them suitable for long-term sequence prediction.

#### Types of LSTM:
- **Vanilla LSTM**
- **Stacked LSTM**
- **Bidirectional LSTM**
- **CNN LSTM**
- **ConvLSTM**

The difference between univariate and multivariate LSTMs lies in the number of input variables used:
- **Univariate LSTM**: Uses a single variable as input.
- **Multivariate LSTM**: Uses multiple variables (e.g., prices from different companies).

### 3. Gated Recurrent Unit (GRU)
GRUs are a variation of LSTMs and are designed to solve the vanishing gradient problem. GRUs use reset and update gates to determine what information should be kept or discarded.

### 4. ARIMA
The ARIMA model is used for forecasting stationary time series data, combining Auto-Regressive (AR) and Moving Average (MA) models with an integration component (I) for non-stationary data.

### 5. SARIMA
SARIMA extends the ARIMA model to handle seasonality in the data, incorporating seasonal AR, MA, and differencing components.

### 6. Facebook Prophet
Prophet is a forecasting tool designed to handle seasonality and holidays. It is simple to use and allows for intuitive adjustments to model parameters.
