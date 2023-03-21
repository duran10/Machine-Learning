# Credit Default Prediction based on Monthly Customer Profile
This Jupyter Notebook contains code for predicting the probability that a customer does not pay back their credit card balance amount in the future based on their monthly customer profile. The target binary variable is calculated by observing 18 months performance window after the latest credit card statement, and if the customer does not pay due amount in 120 days after their latest statement date it is considered a default event.

## Data
The dataset used in this notebook contains aggregated profile features for each customer at each statement date. Features are anonymized and normalized, and fall into the following general categories:

D_* = Delinquency variables

S_* = Spend variables

P_* = Payment variables

B_* = Balance variables

R_* = Risk variables

## Prerequisites
- Python 3.6 or higher
- Jupyter Notebook
- pandas
- scikit-learn
- lightgbm
- BayesSearchCV

## Metrics
The evaluation metric for this notebook is the mean of two measures of rank ordering: Normalized Gini Coefficient and default rate captured at 4%. The default rate captured at 4% is the percentage of the positive labels (defaults) captured within the highest-ranked 4% of the predictions and represents a Sensitivity/Recall statistic.

For both of the sub-metrics, the negative labels are given a weight of 20 to adjust for downsampling. This metric has a maximum value of 1.0.

## Approach
The following steps were followed for building the model:

- Data Preprocessing
- Handling Imbalanced Data using SMOTE
- Training and Tuning the LightGBM Classifier Model with BayesSearchCV
- Evaluating the Model Performance using the above-mentioned Metrics

## Results
The overall evaluation metric value for the model is 0.71.

## Conclusion
In this notebook, we have demonstrated the use of LightGBM Classifier for predicting credit default based on monthly customer profiles. The achieved evaluation metric value of 0.71 indicates that the model has a moderate predictive power and can be used for credit risk assessment with some improvements. The anonymized and normalized features fall into several categories, including delinquency, spend, payment, balance, and risk variables. The model was hypertuned using BayesSearchCV, which is an effective method for optimizing model hyperparameters.
