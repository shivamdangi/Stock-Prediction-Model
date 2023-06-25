INFY Stock Price Prediction Program

This program uses machine learning to predict the future stock prices of INFY (Infosys Limited), an Indian multinational corporation that specializes in business consulting, information technology development, and outsourcing services.

Overview

The program uses historical stock price data (in CSV format) for INFY to train a linear regression model that can predict the future stock prices based on lagged values of the Close column. Specifically, the program creates a Lagged_Close column that contains the previous day’s closing price as a feature for the predictive model.

The program then splits the data into a training set and a testing set, with the last 100 days of data reserved for testing the model’s accuracy. The training set is used to fit a linear regression model using scikit-learn’s LinearRegression class, and the testing set is used to evaluate the model’s accuracy using the R-squared (R2) score.

Finally, the program plots the actual and predicted INFY stock prices for the testing set using matplotlib.

Dependencies

The program requires the following dependencies:

pandas
scikit-learn
matplotlib
These dependencies can be installed using pip:

pip install pandas scikit-learn matplotlib

Usage

To use the program, simply download or clone the repository and run the INFY_Stock_Price_Prediction.py file using Python:

python INFY_Stock_Price_Prediction.py
This will generate a plot of the actual and predicted INFY stock prices, along with the R-squared score of the model’s predictions.

Limitations

It’s worth noting that this program provides a simple example of using machine learning to predict stock prices, and is not intended for use in real-world trading or investment decisions. Additionally, the program uses lagged values of the Close column as the only feature for the predictive model, which may not be sufficient for accurate predictions. It’s recommended to incorporate additional features and use more sophisticated models for improved accuracy.

Note:

Do consider alongwith the linear regression model, an another attempt to predict the stock is done using moving average method which provided score of around 0.0013
, hence prreference to Linear Regression algorithm is given with score of 0.79
