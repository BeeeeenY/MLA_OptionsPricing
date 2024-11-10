# MLA_OptionsPricing
 
## Project Overview
This project analyses and predicts options market data using a range of machine learning and deep learning models. By leveraging historical options data, the project explores patterns through exploratory data analysis (EDA) and implements multiple models for prediction, including the Black-Scholes-Merton (BSM) model, Support Vector Regression (SVR), Artificial Neural Networks (ANN) and Long Short-Term Memory (LSTM) networks.

## Project Structure
The project files and directories are organised as follows:


``` bash
├── ANN.ipynb
├── ANN_old.ipynb
├── Black_Scholes.ipynb
├── EDA
│   └── spx_eda.ipynb
├── LSTM.ipynb
├── MLAANN.ipynb
├── README.md
├── SVR_option_pricing.ipynb
├── daily-treasury-rates.csv
├── data
│   ├── SPX
│   └── SPX samples
├── df1_modified.csv
├── df2_modified.csv
├── df3_modified.csv
├── df4_modified.csv
├── df5_modified.csv
├── df6_modified.csv
├── df_concat_withBSMprice.csv
└── rf_rate_maturity_option_price.ipynb

```

## Contents
1. **Data**: The `data` folder contains six CSV files with historical options data, including fields like option types (calls and puts), strike prices, expiration dates, volatility, and open interest. These files are used across notebooks for training and evaluation.

2. **Notebooks**:
   - **EDA.ipynb**: Performs Exploratory Data Analysis (EDA) to visualise trends and summarise the dataset, including:
     - Data cleaning and preprocessing
     - Analysis of call and put volumes
     - Visualisations of volatility, open interest, and other key features
       
   - **ANN_Model.ipynb**: Implements an Artificial Neural Network (ANN) for prediction, This notebook includes:
     - Data preprocessing and normalisation
     - Hyperparameter tuning for SVR
     - Model architecture and training
     - Model evaluation metrics
       
   - **SVR_Model.ipynb**: Uses Support Vector Regression (SVR) to model the data, This notebook includes:
     - Data scaling
     - Model training and evaluation metrics
       
   - **BSM_Model.ipynb**: Implements the Black-Scholes Model (BSM) for option pricing. This notebook includes:
     - Calculation of option prices using the BSM formula
       
   - **LSTM_Model.ipynb**: Employs a Long Short-Term Memory (LSTM) neural network for time series prediction. This notebook includes:
     - Time series preparation and windowing
     - LSTM model training and tuning
     - Evaluation of model performance on future price predictions

## Installation and Requirements
To run this project locally, install the following libraries:

- Python 3.9 or later
- Jupyter Notebook Extension
- Required Python packages:
  
  ```bash

  pip install pandas numpy matplotlib seaborn scikit-learn tensorflow keras
