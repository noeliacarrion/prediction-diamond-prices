# Kaggle Competition - Diamond prices

### The goal of this competition is the prediction of the price of diamonds based on their characteristics.



- The dataset contains the following columns:
    - Carat
    - Cut
    - Color
    - Clarity
    - Depth
    - Table
    - x
    - y
    - z
    - Price

###  Feature Engineering

- Convert categorial calues to numerical (carat, cut color and clarity), creating my own dictionary with the values that I have considered.

- StandarScaler from Sklearn to standardize the numerical values.

- Drop columns which have high correlation.

- Create new columns based on the values. For example, the mean cut by depth or the mean cut by table, in order to have more information.

###  Models 

- Random Forest with GridSearch
- Gradient Boosting Regressor

I'm still working on the models and the idea es to improve the results, but until now, the best model has been **Random Forest** .

- r2: 0.98
- Square mean error: 563

### Next Steps

- Test other models such as H2O 
- Test Grid Search to find the best parameters
- More feature engineering
