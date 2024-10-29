# House price prediction challenge on Kaggle

Dataset can be found in here: https://www.kaggle.com/datasets/anmolkumar/house-price-prediction-challenge/data

Apply multi ML models for regression tasks including:

+ LinearRegression

+ Ridge

+ Lasso

+ DecisionTreeRegressor

+ RandomForestRegressor

+ KNeighborsRegressor

+ AdaBoostRegressor

+ GradientBoostingRegressor

This is the pipeline of feature engineering:

POSTED_BY: One-hot encode this categorical feature, as "Builder," "Owner," and "Dealer" .

UNDER_CONSTRUCTION, RERA, READY_TO_MOVE: These boolean features can be retained as-is or converted to integer values if not already (0 and 1)

BHK_NO.: This feature can be treated as numeric, but due to the wide range (1-20), some properties at higher values may be outliers.

BHK_OR_RK: One-hot encode this feature as it has only two values, "BHK" and "RK."

SQUARE_FT: Since it spans a wide range, log-transform this feature to normalize its distribution. Additionally, checking for extreme values or outliers could improve model performance.

TARGET (PRICE_IN_LACS): Log-transforming the target variable could make the distribution closer to normal if it is right-skewed

Evaluating metrics: MAE, MSE, RMSE, R^2
