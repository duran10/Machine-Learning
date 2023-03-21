# Short-Term Volatility Prediction for Hundreds of Stocks
This Jupyter Notebook contains a machine learning model that predicts short-term volatility for hundreds of stocks across different sectors, forecasting volatility over 10-minute periods. The dataset used for this project contains stock market data relevant to the practical execution of trades in the financial markets. In particular, it includes order book snapshots and executed trades, providing a uniquely fine-grained look at the micro-structure of modern financial markets.

## Model Architecture
The LGBM (Light Gradient Boosting Machine) regressor was used to predict volatility, and RandomizedSearchCV was used for hyperparameter tuning of the model. The metric used to evaluate the performance of the model was root mean squared percentage error, and a score of 0.23 was achieved.

## Improvements
In addition to the base model, several features were added to improve the accuracy of the predictions such as:

- Time-based features such as hour, minute, and day of the week
- Moving averages of various time periods
 
## Future Work
This project can be expanded by using more advanced machine learning algorithms, such as deep neural networks, to improve the accuracy of the predictions. Additionally, the dataset can be expanded to include more stock market data, such as news articles and social media sentiment, to further refine the model's predictions.

## Dependencies
- pandas
- numpy
- scikit-learn
- lightgbm
