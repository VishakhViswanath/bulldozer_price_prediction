# bulldozer_price_prediction - Machine Learning Project

## Overview

This project aims to predict the sale price of bulldozers using machine learning. The dataset is from the Kaggle **Blue Book for Bulldozers** competition, which contains sales data of bulldozers and their corresponding auction prices. The goal is to develop a machine learning model that can predict future sales prices based on the characteristics of the bulldozers and historical data from similar sales.

## Problem Definition

The objective is to predict the future sale price of a bulldozer based on its features and the prices of similar bulldozers sold previously. The model should minimize the **Root Mean Squared Logarithmic Error (RMSLE)** between the actual and predicted auction prices.

## Dataset

The dataset comes from the Kaggle **Blue Book for Bulldozers** competition. It includes the following three files:

- **train.csv**: Training set with data up to the end of 2011.
- **valid.csv**: Validation set with data from January 1, 2012, to April 30, 2012. Predictions are made on this set.
- **test.csv**: Test set (released after the competition ends), containing data from May 1, 2012, to November 2012.

You can find the dataset and more details on Kaggle:  
[Blue Book for Bulldozers Dataset](https://www.kaggle.com/c/bluebook-for-bulldozers/data)

## Evaluation Metric

The evaluation metric for this competition is **RMSLE** (Root Mean Squared Logarithmic Error), which measures the difference between the actual and predicted auction prices. The goal is to minimize this error.

For more information on the competition and evaluation criteria, check out the [Competition Overview](https://www.kaggle.com/c/bluebook-for-bulldozers/overview).

## Features

The dataset consists of several features that describe the bulldozers, including but not limited to:
- `MachineID`: Unique ID of the bulldozer.
- `YearMade`: The year the bulldozer was manufactured.
- `ProductSize`: Size of the bulldozer.
- `MachineHoursCurrentMeter`: Total number of machine hours.
- `auctioneerID`: ID of the auctioneer.
- `SalePrice`: Target variable (auction price).

For a detailed list of features, refer to the [Data Dictionary on Kaggle](https://www.kaggle.com/c/bluebook-for-bulldozers/data?select=Data+Dictionary.xlsx).

## Approach

1. **Data Cleaning & Preprocessing**:
   - Handle missing values, incorrect data types, and outliers.
   - Feature engineering to extract useful insights from the data.

2. **Data Visualization**:
   - Analyze the distribution of key features and their correlation with the sale price.
   - Visualize trends and patterns to understand the impact of different features on the target variable.

3. **Model Building**:
   - Use **Random Forest Regressor** to predict bulldozer sale prices based on the cleaned and preprocessed data.
   - Perform hyperparameter tuning using **GridSearchCV** to optimize model performance.

4. **Model Evaluation**:
   - The model achieved an **R² score of 0.88** and an **RMSLE of 0.31**, demonstrating strong predictive power in estimating the sale prices of bulldozers.

## How to Run the Code

@. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/bulldozer-price-prediction.git

    Follow the steps in the notebook to load the data, clean it, and build the machine learning model.

Results

    R² score: 0.88, indicating that the model explains 88% of the variance in the bulldozer sale prices.
    RMSLE: 0.31, reflecting a good fit and low error between the predicted and actual prices.

Conclusion

This project demonstrates the process of predicting the sale price of bulldozers using machine learning techniques. The Random Forest Regressor model performed well with an R² score of 0.88 and an RMSLE of 0.31, making it a reliable model for estimating bulldozer prices based on historical sales data. Future work could include experimenting with other algorithms and incorporating additional features for further optimization.

    Dataset provided by Kaggle's Blue Book for Bulldozers competition.
    Libraries used: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

   

