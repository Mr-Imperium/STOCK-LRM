# STOCK-LRM
# Stock Price Prediction Using Linear Regression

This project predicts stock closing prices using a Linear Regression model based on historical stock data. The model is trained on selected features of the dataset to learn patterns and provide predictions for future stock prices.

## Project Overview
The project:
1. Loads and preprocesses stock exchange data.
2. Trains a Linear Regression model on stock price features.
3. Evaluates the model using Root Mean Squared Error (RMSE) and visualizes predicted vs. actual prices.
4. Provides a prediction for the next day's closing price.

## Dataset
The dataset used in this project is located at `/input/stock-exchange-data/indexProcessed.csv`. Key columns in the dataset include:
- **Date**: Date of the stock record
- **Open**: Opening price
- **High**: Highest price during the day
- **Low**: Lowest price during the day
- **Close**: Closing price (target for prediction)
- **Volume**: Volume of stocks traded

## Features and Target
The model uses the following features for prediction:
- `Open`
- `High`
- `Low`
- `Volume`

The target variable is:
- `Close`

## Requirements
To run this project, the following Python libraries are needed:
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

## Steps
1. **Data Loading**: Load the stock data and handle missing or invalid dates.
2. **Data Preprocessing**: 
   - Convert date strings to `DateTime` objects.
   - Drop rows with missing values.
   - Standardize feature values using `StandardScaler`.
3. **Train-Test Split**: Split the data into training (80%) and testing (20%) sets.
4. **Model Training**: Train a Linear Regression model on the training data.
5. **Evaluation**: Calculate the RMSE to assess model performance and visualize predictions against actual prices.
6. **Prediction**: Predict the next day's closing price based on the most recent data.

## Usage
1. Clone the repository and navigate to the project folder.
2. Place your stock data CSV file in the `/input/stock-exchange-data/` folder with the filename `indexProcessed.csv`.
3. Run the Jupyter notebook or execute the script in a Python environment to train the model and make predictions.

## Results
The model outputs the following:
- **Root Mean Squared Error (RMSE)**: Measures model accuracy.
- **Plot of Actual vs Predicted Prices**: Visual comparison of predicted prices against the actual prices for the test data.
- **Next Day Prediction**: Predicted closing price for the following day.

## Example Output
- **RMSE**: Displays the RMSE of the model.
- **Plot**: Shows actual and predicted closing prices.
- **Next Day Predicted Price**: Displays the predicted closing price for the next trading day.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

