
# REGRESSION: Predict a Retail Store Daily Sales

# rossmann-store-sales

## Overview

* Predict Daily Sale for a retail store Rossman
* **Dataset: 1 million rows from Kaggle competition**

* **Machine Learning Models** 
* **XGBoost Regressor**
* Expand and modify from Jovian Data Science
* https://jovian.ai/learn/machine-learning-with-python-zero-to-gbms/lesson/gradient-boosting-with-xgboost
* **Expand: Data Visualization**
* **Modify: DayOfWeek Feature and Hyperparameter Tunning**
* Kaggle submission score is 0.146

## Visualization

![png](images/daily_sales_box.png)


![png](images/daily_sales_hist.png)


![png](images/customers_hist.png)


![png](images/sales_2013.png)


![png](images/sales_2014.png)


![png](images/sales_2015.png)


![png](images/sales_daysofmonth.png)


![png](images/sales_daysofweek.png)

## Models Prediction

#### Model 1: RMSE 1202.47

```
model1 = XGBRegressor(random_state=42, n_jobs=-1,n_estimators=1000, 
                      learning_rate=0.1, 
                      max_depth=10, 
                      subsample=0.5, 
                      colsample_bytree=0.5)

```


#### Model 2: RMSE  1324.47

```
model2 = XGBRegressor(random_state=42, n_jobs=-1,n_estimators=1000, 
                      learning_rate=0.25, 
                      max_depth=12, 
                      subsample=0.7, 
                      colsample_bytree=0.7)
```

#### Model 3: RMSE  1491.72 

```
model3 = XGBRegressor(random_state=42, n_jobs=-1,n_estimators=1000, 
                      learning_rate=0.5, 
                      max_depth=15, 
                      subsample=0.8, 
                      colsample_bytree=0.8)
```

#### Model 4: RMSE  1656.49 

```
model4 = XGBRegressor(random_state=42, n_jobs=-1,n_estimators=1000, 
                      learning_rate=0.75, 
                      max_depth=20, 
                      subsample=0.9, 
                      colsample_bytree=0.9)
```

#### Model 5: RMSE 1307.28

```
model5 = XGBRegressor(random_state=42, n_jobs=-1,n_estimators=1000, 
                      learning_rate=0.05, 
                      max_depth=10, 
                      subsample=0.3, 
                      colsample_bytree=0.3)
```
#### Model 6: RMSE  1282.54

```
model6 = XGBRegressor(random_state=42, n_jobs=-1,n_estimators=1000, 
                      learning_rate=0.05, 
                      max_depth=10, 
                      subsample=0.4, 
                      colsample_bytree=0.4)
```

#### Model 7: RMSE 1547.29

```
model7 = XGBRegressor(random_state=42, n_jobs=-1,n_estimators=1000, 
                      learning_rate=0.01, 
                      max_depth=10, 
                      subsample=0.5, 
                      colsample_bytree=0.5)
```

#### Model 8: RMSE  1211.96

```
model8 = XGBRegressor(random_state=42, n_jobs=-1,n_estimators=1000, 
                      learning_rate=0.05, 
                      max_depth=10, 
                      subsample=0.5, 
                      colsample_bytree=0.5)
```

#### Model 9: RMSE  1240.06

```
model9 = XGBRegressor(random_state=42, n_jobs=-1,
                      n_estimators=1000, 
                      learning_rate=0.2, 
                      max_depth=10, 
                      subsample=0.5, 
                      colsample_bytree=0.5)
```

#### Model 10: RMSE  1226.53

```
model10 = XGBRegressor(random_state=42, n_jobs=-1,
                      n_estimators=1500, 
                      learning_rate=0.09, 
                      max_depth=10, 
                      subsample=0.5, 
                      colsample_bytree=0.5)
```
