# Discount Optimization
This repository contains a Jupyter Notebook that uses machine learning techniques to predict the quantities sold of products in an e-commerce business, and then applies a simulation that optimizes the best discount the company can choose based on dates and different discounts applied. The optimization is based on price elasticity, which is the ratio of the percentage change in quantity demanded of a product to the percentage change in price.

## Dataset
The dataset used in this project contains information about the sales of products in an e-commerce business. The dataset includes columns such as date, product ID, price, ratings and quantity sold.

## Libraries/Tools Used
- Pandas
- Scikit-learn
- Matplotlib
- Predicting Quantities Sold
- To predict the quantities sold, a Random Forest Regressor model was trained on the dataset. The model was trained on features such as date, price, ratings and product ID. After training the model, new columns were created with the predicted quantities sold.

## Discount Optimization
After predicting the quantities sold, the next step was to apply a simulation that optimizes the best discount the company can choose based on dates and different discounts applied. The optimization uses price elasticity to determine the best discount strategy. Price elasticity of demand is the ratio of the percentage change in quantity demanded of a product to the percentage change in price. The simulation iterates over different discount strategies and selects the one that results in the highest profit.

## Root Mean Squared Percentage Error
The root mean squared percentage error for this project was 0.21, which indicates that the model has a good level of accuracy in predicting the quantities sold.

## Conclusion
This project demonstrates how machine learning techniques can be used to predict quantities sold in an e-commerce business and optimize discount strategies based on price elasticity. The Jupyter Notebook provides a step-by-step guide to the process, making it easy to replicate and extend for other similar projects.
